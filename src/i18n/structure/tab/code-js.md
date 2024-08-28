```js

// Component Tab
<script>
    const tab = document.getElementsByClassName("element-tab");
    if(tab){
        for(let j=0; j < tab.length; j++){
            const boton = tab[j].getElementsByClassName("show-select");
            const cuerpo = tab[j].getElementsByClassName("tab-select");
            
            function closeAllDropdowns(drop: any) {
                if(boton){
                    for(let i=0; i < boton.length; i++){
                        if(boton[i] !== drop){
                            if(cuerpo[i]){
                                cuerpo[i].classList.remove('active');
                                cuerpo[i].classList.add('deactive');
                            }
                            boton[i].classList.remove('button-selected');
                        }else{
                            boton[i].classList.add('button-selected');
                        }
                    }
                }
            }
            if(boton && cuerpo){
                boton[0].classList.add('button-selected');
                for(let i=0; i < boton.length; i++){
                    boton[i].addEventListener("click", () =>{
                        if(cuerpo[i]){
                            cuerpo[i].classList.remove('deactive');
                            cuerpo[i].classList.add('active');
                        }
                        closeAllDropdowns(boton[i])
                    });
                }
            }
        }
    }
</script>
```