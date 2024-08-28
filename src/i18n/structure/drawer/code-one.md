```astro live

import Drawer from './Drawer.astro';
import DrawerContent from './DrawerContent.astro';

<Drawer>
    <button class="px-1">left</button>
    <DrawerContent>
        <main class="w-80">
            display left
        </main>
    </DrawerContent>
</Drawer>
```