```js

<script>
    const collapseBoton = document.getElementsByClassName("collapse-Button");

    if (collapseBoton) {
        for(let i=0; i < collapseBoton.length; i++){
            const rotateIcon = collapseBoton[i].querySelector(".icon-rotate");
            const focus = collapseBoton[i].querySelector(".focus");
            const panel =collapseBoton[i].nextElementSibling as HTMLElement;

            collapseBoton[i].addEventListener("click", () =>{
                collapseBoton[i].classList.toggle("active");
                if(rotateIcon){
                    rotateIcon.classList.toggle("rotate-180");
                }
                if(panel){
                    if (panel.style.display === "block") {
                        panel.style.display = "none";
                    } else {
                        panel.style.display = "block";
                    }
                }
            });
            if(focus){
                collapseBoton[i].addEventListener("blur", () => {
                    collapseBoton[i].classList.remove("active");
                    if (panel) {
                        panel.style.display = "none";
                    }
                });
            }
        }
    }
</script>
```