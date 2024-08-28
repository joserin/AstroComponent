```astro live

import Carousel from './Carousel.astro';

<Carousel class='default flex-col snap-y w-72 h-[25rem] aspect-auto'>
    <img src="/img-1.webp" 
        class="w-fit h-fit" alt="pineapple" />
    <img src="/img-2.webp" 
        class="w-fit h-fit" alt="lemon" />
    <img src="/img-3.webp" 
        class="w-fit h-fit" alt="nacelle" />
    <img src="/img-4.webp" 
        class="w-fit h-fit" alt="grapes" />
</Carousel>
```