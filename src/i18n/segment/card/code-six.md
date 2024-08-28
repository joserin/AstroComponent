```astro live
import Card from './Card.astro';
import Button from './Button.astro';

<Card class="w-80 h-40 rounded-xl overflow-hidden shadow-xl p-3 bg-black text-center flex flex-col justify-center">
    <header class="flex items-center gap-2">
        <h4 class="font-semibold text-2xl text-white">Cookies!</h4>
    </header>
    <div>
        <p class="p-1 text-white">description for this product</p>
        <footer class="flex justify-center gap-2 items-end">
            <Button class=" bg-slate-600 hover:bg-slate-400 px-2 py-1 w-fit rounded-xl">Accept</Button>
            <Button class=" bg-slate-700 hover:bg-slate-500 px-2 py-1 w-fit rounded-xl">Cancel</Button>
        </footer>
    </div>
</Card>
```