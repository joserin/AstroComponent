```astro live
import Card from './Card.astro';
import Button from './Button.astro';

<Card class="w-[30rem] h-60 rounded-xl shadow-xl flex overflow-hidden border">
    <header>
        <img class="w-60 h-full" src="/img-9.webp" alt="">
    </header>
    <div class="flex flex-col gap-2 p-3">
        <h4 class="font-semibold text-2xl">Movie!</h4>
        <p class="p-1">description for this product</p>
        <footer class="flex justify-center gap-2 items-end">
            <Button class=" bg-purple-600 hover:bg-purple-400 px-2 py-1 w-fit rounded-xl">Buy Now</Button>
        </footer>
    </div>
</Card>
```