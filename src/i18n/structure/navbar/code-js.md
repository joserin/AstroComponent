```js

// Component CarouselButton
<script define:vars={{idPtrevButton, idNextButton}}>
    const carousel = document.getElementsByClassName("carousel");
    if(carousel){
        for(let i=0; i < carousel.length; i++){
            const Container = carousel[i].querySelector(".slides-container");
            const slider = carousel[i].querySelectorAll(".slides-container img");
            const botones = carousel[i].querySelectorAll(".list-buttons button");

            if(slider){
                const slideWidth = slider[0].clientWidth;

                if(botones.length > 0){
                    const goToImage = (index) => {
                        if (Container) {
                            Container.scrollLeft = index * slideWidth;
                        }
                    };
                    for(let j=0; j < botones.length; j++){
                        if(botones[j]){
                            botones[j].addEventListener("click", () => goToImage(j));
                        }
                    }
                }else{
                    const prevButton = document.getElementById(idPtrevButton);
                    const nextButton = document.getElementById(idNextButton);

                    if(nextButton){
                        nextButton.addEventListener("click", () => {
                            if (Container) {
                                Container.scrollLeft += slideWidth;
                            }
                        });
                    }
                    if(prevButton){
                        prevButton.addEventListener("click", () => {
                            if (Container) {
                                Container.scrollLeft -= slideWidth;
                            }
                        });
                    }
                }
            }
        }
    }
</script>
```