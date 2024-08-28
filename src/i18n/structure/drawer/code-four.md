```astro live

import Drawer from './Drawer.astro';
import DrawerContent from './DrawerContent.astro';
import DrawerLabel from './DrawerLabel.astro';

<Drawer id="menu" class='bg-red-500 rounded-full p-1'>
    <DrawerLabel identifier='menu'>
        <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" 
            stroke-width="1.5" stroke="#ffffff" fill="none" stroke-linecap="round" stroke-linejoin="round">
            <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
            <path d="M4 6l16 0" />
            <path d="M4 12l16 0" />
            <path d="M4 18l16 0" />
        </svg>
    </DrawerLabel>
    <DrawerContent class='text-black top-0 right-0 bg-white/80 w-fit h-full transform 
        translate-x-full peer-checked:-translate-x-0'>
        <div class="w-80">
            display bottom
        </div>
    </DrawerContent>
</Drawer>
```