```astro live

import Card from './Card.astro';
import Button from './Button.astro';

<Card class="default flex-col rounded-xl bg-blue-700">
    <header slot="header" class="w-fit border border-black">
        <img class="w-56 h-56" src="/img-9.webp" alt="">
    </header>
    <div class="p-3 flex flex-col">
        <h4 class="font-semibold text-2xl">Title</h4>
        <p class="p-1">Description for this product</p>
    </div>
    <footer slot="footer" class="flex justify-end pr-2">
        <Button class="text-black bg-white hover:bg-blue-300 p-1 w-fit rounded-xl">Buy Now</Button>
    </footer>
</Card>
```