```astro live

import CarouselButton from './CarouselButton.astro';

<CarouselButton class='flex flex-col w-[30rem]'>
    <img src="https://img.daisyui.com/images/stock/photo-1625726411847-8cbb60cc71e6.webp" 
        class="w-full h-60" alt="city day"/>
    <img src="https://img.daisyui.com/images/stock/photo-1609621838510-5ad474b7d25d.webp" 
        class="w-full h-60" alt="city night"/>
    <img src="https://img.daisyui.com/images/stock/photo-1414694762283-acccc27bca85.webp" 
        class="w-full h-60" alt="city forest"/>
    <img src="https://img.daisyui.com/images/stock/photo-1665553365602-b2fb8e5d1707.webp" 
        class="w-full h-60" alt="city town"/>
    <footer slot="button-move" class="flex w-full justify-center gap-5 list-buttons">
        <Button class='bg-blue-400 px-2 rounded-full hover:bg-blue-600'>1</Button>
        <Button class='bg-blue-400 px-2 rounded-full hover:bg-blue-600'>2</Button>
        <Button class='bg-blue-400 px-2 rounded-full hover:bg-blue-600'>3</Button>
        <Button class='bg-blue-400 px-2 rounded-full hover:bg-blue-600'>4</Button>
    </footer>
</CarouselButton>
```