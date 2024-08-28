```js

<script>
    const elementList = document.getElementsByClassName('element-popover');
    if(elementList){
        for(let i=0; i < elementList.length; i++){
            const botonPopover = elementList[i].querySelector('.button-popover');
            const popoverContent = elementList[i].querySelector('.popover-display') as HTMLElement;
            botonPopover?.addEventListener("click", ()=>{
                
                if(!popoverContent) return 0;
                popoverContent.classList.remove("hide");
                popoverContent.classList.add("show");
            });
            document.addEventListener("click", (event) => {
                if(!popoverContent) return 0;
                const targetElement = event.target as HTMLElement;
                if (event.target !== botonPopover && !popoverContent.contains(targetElement)) {
                    popoverContent.classList.add("hide");
                    popoverContent.classList.remove("show");
                }
            });
        }
    }
</script>
```