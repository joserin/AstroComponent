```astro live

import Drawer from './Drawer.astro';
import DrawerContent from './DrawerContent.astro';

<Drawer class='border border-white p-1'>
    <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" 
        stroke-width="1.5" stroke="#ffffff" fill="none" stroke-linecap="round" stroke-linejoin="round">
        <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
        <path d="M8 13v-8.5a1.5 1.5 0 0 1 3 0v7.5" />
        <path d="M11 11.5v-2a1.5 1.5 0 1 1 3 0v2.5" />
        <path d="M14 10.5a1.5 1.5 0 0 1 3 0v1.5" />
        <path d="M17 11.5a1.5 1.5 0 0 1 3 0v4.5a6 6 0 0 1 -6 6h-2h.208a6 6 0 0 1 -5.012 -2.7a69.74 69.74 
            0 0 1 -.196 -.3c-.312 -.479 -1.407 -2.388 -3.286 -5.728a1.5 1.5 0 0 1 .536 -2.022a1.867 1.867 
            0 0 1 2.28 .28l1.47 1.47" />
    </svg>
    <DrawerContent class="top-0 left-0 w-full h-fit transform -translate-y-full bg-black 
        shadow-lg peer-checked:translate-y-0">
        <main class="h-56">
            display top
        </main>
    </DrawerContent>
</Drawer>
```