```astro live

import Navbar from './Navbar.astro';
import ButtonLink from './ButtonLink.astro';
import Dropdown from './Dropdown.astro';

<Navbar class='flex justify-center w-fit items-center p-1 gap-5'>
    <Dropdown>
        <span slot="boton" class="button-dropdown">
            <p class="close-focus-out">Part one</p>
        </span>
        <ul class="w-36 p-3 text-sm flex flex-col gap-1 bg-yellow-500">
            <li>My Information</li>
            <li>Profile</li>
            <li>Watch out</li>
        </ul>
    </Dropdown>
    <Dropdown>
        <span slot="boton" class="button-dropdown">
            <p class="close-focus-out">Part two</p>
        </span>
        <ul class="w-36 p-3 text-sm flex flex-col gap-1 bg-blue-500">
            <li>Password</li>
            <li>Tools</li>
            <li>Help</li>
        </ul>
    </Dropdown>
    <ButtonLink url="" class='text-xl font-bold hover:bg-slate-300 rounded-lg p-1'>
        Home
    </ButtonLink>
</Navbar>
```