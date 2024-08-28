```js

<script>
    const modal = document.getElementsByClassName("modal-content");

    if(modal){
        for(let i=0; i < modal.length; i++){
            const buttonsModalOpen = modal[i].querySelector('.button-modal');
            const modalCloseButtons = modal[i].querySelector('.modal-close');
            const modalCloseEsc = modal[i].querySelector('.modal-closeEsc');
            const modalCloseClick = modal[i].querySelector('.modal-closeClick');

            if(buttonsModalOpen){
                buttonsModalOpen.addEventListener("click", () => {
                    const targetModal = buttonsModalOpen.nextElementSibling;
                    targetModal?.classList.replace("hidden", "flex");
                });
            }

            function closeModalView(){
                const targetModal = buttonsModalOpen?.nextElementSibling;
                targetModal?.classList.replace("flex", "hidden");
            }

            if(modalCloseButtons){
                modalCloseButtons.addEventListener("click", () => {
                    closeModalView()
                });
            }
            if (modalCloseEsc) {
                modal[i].addEventListener('keydown', (event: any) => {
                    if (event.key === 'Escape') {
                        closeModalView()
                    }
                });
            }
            if (modalCloseClick){
                modalCloseClick.addEventListener('click', (event) => {
                    if ((event.target as HTMLElement).contains(modalCloseClick)) {
                        closeModalView()
                    }
                });
            }
        }
    }
</script>
```