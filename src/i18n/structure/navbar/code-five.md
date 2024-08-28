```astro live

import Navbar from './Navbar.astro';
import ButtonLink from './ButtonLink.astro';
import Dropdown from './Dropdown.astro';
import Avatar from './Avatar.astro';

<Navbar class=' bg-lime-100 flex justify-between w-full items-center p-1'>
    <ButtonLink url="" class='text-black text-xl font-bold hover:bg-lime-200 rounded-lg p-1'>
        Home
    </ButtonLink>
    <div class="flex justify-center items-center gap-2">
        <input class="p-1 bg-lime-500" type="search">
        <Dropdown>
            <Avatar slot="boton" class="button-dropdown cursor-pointer">
                <img class="close-focus-out w-10 h-10 rounded-3xl" 
                    src="https://daisyui.com/images/stock/photo-1534528741775-53994a69daeb.jpg" alt="">
            </Avatar>
            <ul class="w-40 p-1 flex flex-col gap-3 bg-black absolute right-0">
                <li>My Information</li>
                <li>Profile</li>
                <li>Watch out</li>
            </ul>
        </Dropdown>
    </div>
</Navbar>
```