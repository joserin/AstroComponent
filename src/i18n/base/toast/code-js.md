```js
<script>
    const buttonOpenToast = document.getElementsByClassName('buttonToast');
    if(buttonOpenToast){
        for(let i=0; i < buttonOpenToast.length; i++){
            buttonOpenToast[i].addEventListener("click", ()=>{
                const openModal = buttonOpenToast[i].nextElementSibling as HTMLElement;
                
                if(openModal){
                    openModal.classList.remove("hidden");
                    openModal.classList.add("block");
                    setTimeout(() =>{
                        openModal.classList.remove("block");
                        openModal.classList.add("hidden");
                    }, 3000);
                }
            });
        }
    }
</script>
```