```js

<script>
    const dropdown = document.getElementsByClassName("dropdown");

    function closeAllDropdowns(drop: any) {
        if(dropdown){
            for(let i=0; i < dropdown.length; i++){
                if(dropdown[i] !== drop){
                    const botonMenu = dropdown[i].querySelector('.button-dropdown');
                    const dropdownContent = dropdown[i].querySelector('.dropdown-content') as HTMLElement;
                    if(botonMenu && dropdownContent){
                        botonMenu.classList.toggle('active');
                        dropdownContent.style.display = "none";
                    }
                }
            }
        }
    }

    if(dropdown){
        for(let i=0; i < dropdown.length; i++){
            const botonMenu = dropdown[i].querySelector('.button-dropdown');
            const dropdownContent = dropdown[i].querySelector('.dropdown-content') as HTMLElement;
            const focus = dropdown[i].querySelector('.close-focus-out') as HTMLElement;
            
            if(botonMenu && dropdownContent){
                botonMenu.addEventListener('click', () =>{
                    botonMenu.classList.toggle('active');
                    if (dropdownContent.style.display === "block") {
                        dropdownContent.style.display = "none";
                    } else {
                        dropdownContent.style.display = "block";
                    }
                    closeAllDropdowns(dropdown[i]);
                });
            }
            if(focus){
                document.addEventListener('click', function(event) {
                    if (!dropdown[i].contains(event.target as Node)) {
                        dropdownContent.style.display = "none"
                    }
                });
            }
        }
    }
</script>
```