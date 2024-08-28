```js

<script>
    const ratingContainer = document.getElementsByClassName('rating');
    if(ratingContainer){
        for(let i=0; i < ratingContainer.length; i++){
            const starInputs = ratingContainer[i].querySelectorAll('.mask');
            if(starInputs){
                starInputs.forEach((elementInputIndividual, index) => {
                    elementInputIndividual.addEventListener('click', () => {
                        if((elementInputIndividual as HTMLInputElement).checked){
                            for (let j = 0; j <= index; j++) {
                                console.log(j, elementInputIndividual, 'checked');
                                (starInputs[j] as HTMLInputElement).checked = true;
                            }
                        }else{
                            for (let j = index; j < starInputs.length; j++) {
                                console.log(j, elementInputIndividual, 'not checked');
                                (starInputs[j] as HTMLInputElement).checked = false;
                            }
                        }
                    });
                });
            }
        }
    }
</script>
```