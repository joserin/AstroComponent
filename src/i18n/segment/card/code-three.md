```astro live

import Card from './Card.astro';
import Button from './Button.astro';

<Card class="default flex-col bg-white rounded-xl text-black">
    <header slot="header" class="flex justify-center items-center">
        <img class="w-40 h-40 m-2" src="/img-9.webp" alt="">
    </header>
    <div class="p-3 flex flex-col w-full h-full">
        <div class="flex items-center gap-2 justify-center">
            <h4 class="font-semibold text-2xl">Title</h4>
            <Badge class="px-1 text-red-600 font-semibold rounded-xl">New</Badge>
        </div>
        <p class="p-1">description for this product</p>
    </div>
    <footer slot="footer" class="flex justify-center gap-2 items-end">
        <Button class=" bg-blue-300 hover:bg-blue-500 p-1 w-fit rounded-xl">Buy Now</Button>
    </footer>
</Card>
```