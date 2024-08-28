```astro live

import Navbar from './Navbar.astro';
import ButtonLink from './ButtonLink.astro';
import Button from './Button.astro';

<Navbar class='flex justify-between bg-white w-full items-center px-3 py-1'>
    <picture class="border-2 flex items-center">
        <Button class='hover:bg-blue-100'>
            <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="20" height="20" viewBox="0 0 24 24" 
                stroke-width="1" stroke="#000000" fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                <path d="M4 6l16 0" />
                <path d="M4 12l16 0" />
                <path d="M4 18l16 0" />
            </svg>
        </Button>
    </picture>
    <ButtonLink url="" class='text-black text-xl font-bold hover:bg-slate-300 rounded-lg p-1'>
        Home
    </ButtonLink>
    <picture class="border-2 flex items-center">
        <Button class='hover:bg-red-100'>
            <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="20" height="20" viewBox="0 0 24 24" 
                stroke-width="1.5" stroke="#000000" fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                <path d="M5 12m-1 0a1 1 0 1 0 2 0a1 1 0 1 0 -2 0" />
                <path d="M12 12m-1 0a1 1 0 1 0 2 0a1 1 0 1 0 -2 0" />
                <path d="M19 12m-1 0a1 1 0 1 0 2 0a1 1 0 1 0 -2 0" />
            </svg>
        </Button>
    </picture>
</Navbar>
```