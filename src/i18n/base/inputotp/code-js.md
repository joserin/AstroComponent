```js

// Component InputOtp
<script>
    const input = document.getElementsByClassName('input-select');
    if(input) {
        for(let i=0; i < input.length; i++){
            const inputElement = input[i] as HTMLInputElement;
            inputElement.addEventListener('input', () => {
                if (inputElement.value.length > 1) {
                    inputElement.value = inputElement.value.slice(0, 1);
                }
            });
        }
    }
</script>

// Component InputOtpGroup
<script>
    const inputGroup = document.getElementsByClassName('otp-container');
    
    if(inputGroup) {
        for(let i=0; i < inputGroup.length; i++){
            const inputElementGroup = inputGroup[i] as HTMLInputElement;
            const imputElement = inputElementGroup.querySelectorAll('.input-group');
            
            if(imputElement){
                for(let j=0; j < imputElement.length; j++){
                    const elementInputIndividual = imputElement[j] as HTMLInputElement;
                    if(j === 0){
                        elementInputIndividual.focus();
                    }else{
                        elementInputIndividual.disabled = true;
                    }

                    elementInputIndividual.addEventListener('input', () => {
                        if (elementInputIndividual.value.length > 0 ) {
                            elementInputIndividual.value = elementInputIndividual.value.slice(0, 1);
                            const nextElement = imputElement[j+1] as HTMLInputElement;
                            if(nextElement){
                                elementInputIndividual.disabled = true
                                nextElement.disabled = false;
                                nextElement.focus()
                            }
                        }
                    });
                    elementInputIndividual.addEventListener('keydown', (e) =>{
                        if (elementInputIndividual.value.length === 0 && e.key === 'Backspace') {
                            const beforeElement = imputElement[j-1] as HTMLInputElement;
                            if(beforeElement){
                                elementInputIndividual.disabled = true;
                                beforeElement.disabled = false;
                                beforeElement.focus()
                                beforeElement.value = ''
                            }
                        }
                    });
                }
            }
        }
    }
</script>
```