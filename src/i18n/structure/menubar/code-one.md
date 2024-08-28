```astro live

import Menu from './Menu.astro';
import MenuElement from './MenuElement.astro';
import Dropdown from './Dropdown.astro';

<Menu class='flex gap-1'>
    <MenuElement>
        <Dropdown title='Name'>
            <ul class="bg-purple-300 w-36 p-2 flex flex-col gap-1 text-sm close-focus-out">
                <li>My Information</li>
                <li>Profile</li>
                <li>Pay</li>
            </ul>
        </Dropdown>
    </MenuElement>
    <MenuElement>
        <Dropdown title='More'>
            <ul class="bg-purple-300 w-36 p-2 flex flex-col gap-1 text-sm close-focus-out">
                <li>Github</li>
                <li>Facebook</li>
                <li>Team</li>
            </ul>
        </Dropdown>
    </MenuElement>
    <MenuElement>
        <Dropdown title='Information'>
            <ul class="bg-purple-300 w-36 p-1 flex flex-col gap-1 close-focus-out">
                <li>Keyboard image</li>
                <li>Power level english</li>
                <li>Exit</li>
            </ul>
        </Dropdown>
    </MenuElement>
</Menu>
```