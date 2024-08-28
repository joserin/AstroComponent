```astro live

import Menu from './Menu.astro';
import MenuElement from './MenuElement.astro';
import Button from './Button.astro';

<Menu class='bg-purple-300 flex flex-col gap-1 w-40'>
    <MenuElement>
        <Button class='w-full text-left rounded-lg bg-purple-400 hover:bg-purple-500 px-2 py-1'>
            Items 1
        </Button>
    </MenuElement>
    <MenuElement>
        <Button class='w-full text-left rounded-lg bg-purple-400 hover:bg-purple-500 px-2 py-1'>
            Items 2
        </Button>
    </MenuElement>
    <MenuElement>
        <Button class='w-full text-left rounded-lg bg-purple-400 hover:bg-purple-500 px-2 py-1'>
            Items 3
        </Button>
    </MenuElement>
    <MenuElement>
        <Button class='w-full text-left rounded-lg bg-purple-400 hover:bg-purple-500 px-2 py-1'>
            Items 4
        </Button>
    </MenuElement>
    <MenuElement>
        <Button class='w-full text-left rounded-lg bg-purple-400 hover:bg-purple-500 px-2 py-1'>
            Items 5
        </Button>
    </MenuElement>
</Menu>
```