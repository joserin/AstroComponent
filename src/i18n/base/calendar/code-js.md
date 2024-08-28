```js

<script>
    const monthInput = document.querySelector(".month-input");
    const yearInput = document.querySelector(".year-input");
    const dates = document.querySelector(".dates") as HTMLElement;
    const nextBtn = document.querySelector(".next");
    const prevBtn = document.querySelector(".prev");

    const currentDate = new Date();
    let selectedDate = new Date();
    let year = currentDate.getFullYear();
    let month = currentDate.getMonth();
    let aux = false;

    monthInput?.addEventListener("change", () => {
        month = (monthInput as HTMLSelectElement).selectedIndex;
        displayDates();
    });

    yearInput?.addEventListener("change", () => {
        year = Number((yearInput as HTMLInputElement).value);
        displayDates();
    });

    const updateYearMonth = () => {
        (monthInput as HTMLSelectElement).selectedIndex = month;
        (yearInput as HTMLInputElement).value = year.toString();
    };

    const handleDateClick = (e: any) => {
        const button = e.target;
        const datesList = button.parentElement as HTMLElement;
        const selectedButtons = datesList.querySelectorAll('.selected') as NodeListOf<HTMLElement>;

        selectedDate = new Date(year, month, parseInt(button.textContent));
        const isToday = currentDate.getDate() === selectedDate.getDate() && 
            currentDate.getFullYear() === selectedDate.getFullYear() && 
            currentDate.getMonth() === selectedDate.getMonth();

        if(isToday){
            aux = true;
        }
        
        if(selectedButtons){
            for (const selectedButton of selectedButtons) {
                console.log('before',aux)
                selectedButton.classList.remove('selected');
                if (Number(selectedButton.textContent) !== currentDate.getDate()) {
                    selectedButton.style.backgroundColor = '';
                }else{
                    if(aux){
                        selectedButton.style.backgroundColor = 'lightblue'
                    }else{
                        selectedButton.style.backgroundColor = ''
                    }
                    aux = false;
                }
            }
        }
        button.classList.add('selected');
        button.style.backgroundColor =  "red";
    };
    
    const createButton = (text: any, isDisabled = false, type = 0) => {

        const comparisonDate = new Date(year, month + type, text);
        const isToday = currentDate.getDate() === comparisonDate.getDate() && 
            currentDate.getFullYear() === comparisonDate.getFullYear() && 
            currentDate.getMonth() === comparisonDate.getMonth();

        const button = document.createElement("button");
        button.textContent = text;
        button.disabled = isDisabled;
        if(isDisabled){
            button.style.backgroundColor =  "lightgray";
            button.style.color = "gray";
        }
        if(isToday){
            button.style.backgroundColor =  "lightblue";
        }
        //button.classList.toggle("selected", selected);
        return button;
    };
    
    const displayDates = () => {
        
        updateYearMonth();
        dates.innerHTML = "";

        const lastOfPrevMonth = new Date(year, month, 0);

        for (let i = 0; i <= lastOfPrevMonth.getDay(); i++) {
            const text = lastOfPrevMonth.getDate() - lastOfPrevMonth.getDay() + i;
            const button = createButton(text, true, -1);
            dates.appendChild(button);
        }
        const lastOfMOnth = new Date(year, month + 1, 0);

        for (let i = 1; i <= lastOfMOnth.getDate(); i++) {
            const button = createButton(i, false);
            button.addEventListener("click", handleDateClick);
            dates.appendChild(button);
        }

        const firstOfNextMonth = new Date(year, month + 1, 1);

        for (let i = firstOfNextMonth.getDay(); i < 7; i++) {
            const text = firstOfNextMonth.getDate() - firstOfNextMonth.getDay() + i;

            const button = createButton(text, true, 1);
            dates.appendChild(button);
        }
    };

    nextBtn?.addEventListener("click", () => {
        if (month === 11) year++;
        month = (month + 1) % 12;
        displayDates();
    });

    prevBtn?.addEventListener("click", () => {
        if (month === 0) year--;
        month = (month - 1 + 12) % 12;
        displayDates();
    });

    displayDates();
</script>
```