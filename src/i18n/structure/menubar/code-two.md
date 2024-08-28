```astro live

import Menu from './Menu.astro';
import MenuElement from './MenuElement.astro';
import Dropdown from './Dropdown.astro';

<Menu class='bg-black flex flex-col text-sm text-white justify-center items-center'>
    <MenuElement class='p-1 w-fit h-full'>
        <Dropdown class='p-2' tabindex="0">
            <div slot="boton" class="button-dropdown">
                <p class="close-focus-out">Items 1</p>
            </div>
            <ul tabindex="0" class="bg-black border w-36 p-3 flex flex-col gap-3 absolute left-14">
                <li>My Information</li>
                <li>Profile</li>
            </ul>
        </Dropdown>
    </MenuElement>
    <MenuElement class='p-1 w-fit h-full'>
        <Dropdown class='p-2' tabindex="0">
            <div slot="boton" class="button-dropdown">
                <p class="close-focus-out">Items 2</p>
            </div>
            <ul tabindex="0" class="bg-black border w-36 p-3 flex flex-col gap-3 absolute left-14">
                <li>Pay</li>
                <li>Github</li>
            </ul>
        </Dropdown>
    </MenuElement>
    <MenuElement class='p-1 w-fit h-full'>
        <Dropdown class='p-2' tabindex="0">
            <div slot="boton" class="button-dropdown">
                <p class="close-focus-out">Items 3</p>
            </div>
            <ul tabindex="0" class="bg-black border w-36 p-3 flex flex-col gap-3 absolute left-14">
                <li>Facebook</li>
                <li>Team</li>
            </ul>
        </Dropdown>
    </MenuElement>
</Menu>
```