```astro live

import Drawer from './Drawer.astro';
import DrawerContent from './DrawerContent.astro';
import DrawerLabel from './DrawerLabel.astro';

<Drawer id="drawer">
    <DrawerLabel identifier='drawer'/>
    <DrawerContent>
        <div class="w-80">
            display bottom
        </div>
    </DrawerContent>
</Drawer>
```