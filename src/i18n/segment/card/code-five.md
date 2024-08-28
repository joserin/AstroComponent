```astro live
import Carousel from './Carousel.astro';

<Card class="w-80 h-40 rounded-xl overflow-hidden shadow-xl p-3 border flex flex-col justify-between">
    <header class="flex items-center gap-2">
        <h4 class="font-semibold text-2xl">Title</h4>
    </header>
    <div class="w-fit">
        <p class="p-1">description for this product</p>
    </div>
    <footer class="flex justify-end gap-2 items-end">
        <Button class=" bg-lime-700 hover:bg-lime-500 px-2 py-1 w-fit rounded-xl">Buy Now</Button>
    </footer>
</Card>
```