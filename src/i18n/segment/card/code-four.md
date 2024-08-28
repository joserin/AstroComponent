```astro live

import Card from './Card.astro';
import Button from './Button.astro';

<Card class="relative w-fit rounded-xl overflow-hidden">
    <header slot="header" class="w-fit">
        <img class="w-96 h-72" src="/img-9.webp" alt="">
    </header>
    <div class="absolute top-0 left-0 w-full h-full bg-black bg-opacity-70 text-white p-10 flex flex-col">
        <div class="flex items-center gap-2">
            <h4 class="font-semibold text-2xl">Title</h4>
        </div>
        <p class="p-1 font-semibold">Description for this product</p>
        <footer class="flex justify-end gap-2 items-end m-7 py-10">
            <Button class=" bg-orange-700 hover:bg-orange-500 p-1 w-fit rounded-xl">Buy Now</Button>
        </footer>
    </div>
</Card>
```