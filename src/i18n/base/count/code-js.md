```js

<script>
    const countElement = document.getElementsByClassName("count");

    if(countElement){
        for(let i=0; i < countElement.length; i++){

            const countdownElement = countElement[i].querySelector(".countdown") as HTMLElement;
            const startString = countdownElement?.dataset.start;
            const endString = countdownElement?.dataset.end;
            const stepString = countdownElement?.dataset.step;
            const timeString = countdownElement?.dataset.time;

            if(startString && endString && stepString && timeString){

                let tiempoRestante: number = parseInt(startString);
                let intervalo: number;

                function actualizarContador(end:number, start: number, steps:number) {
                    if(start > end){
                        if(steps > 0) tiempoRestante-= steps;
                        else tiempoRestante--;
                    }else{
                        if(steps > 0) tiempoRestante+= steps;
                        else tiempoRestante++;
                    }

                    if (tiempoRestante < end && start > end) {
                        tiempoRestante = start;
                    }else if(tiempoRestante > end && start < end){
                        tiempoRestante = start;
                    }
                    countdownElement.textContent = tiempoRestante.toString();
                }
                intervalo = setInterval(actualizarContador, parseInt(timeString), parseInt(endString), parseInt(startString), 
                    parseInt(stepString));
            }
        }
    }
</script>
```