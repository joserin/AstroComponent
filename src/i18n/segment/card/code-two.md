```astro live

import Card from './Card.astro';
import Button from './Button.astro';

<Card class="default flex-col bg-blue-200 rounded-xl text-black">
    <header slot="header" class="w-fit">
        <img class="w-56 h-56" src="/img-9.webp" alt="">
    </header>
    <div class="p-3 flex flex-col">
        <div class="flex items-center gap-2">
            <h4 class="font-bold text-2xl">Title</h4>
            <Badge class="border-2 border-red-500 px-2 py-1 text-black font-semibold rounded-xl">New</Badge>
        </div>
        <p class="p-1">description for this product</p>
    </div>
    <footer slot="footer" class="flex justify-end pr-2">
        <div class="flex justify-end gap-2">
            <Badge class="border-2 border-black rounded-full p-1 bg-red-400">better</Badge>
            <Badge class="border-2 border-black rounded-full p-1 bg-yellow-400">bag</Badge>
        </div>
    </footer>
</Card>
```