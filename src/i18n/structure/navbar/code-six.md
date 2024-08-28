```astro live

import Navbar from './Navbar.astro';
import Dropdown from './Dropdown.astro';
import Button from './Button.astro';
import ButtonLink from './ButtonLink.astro';
import Indicator from './Indicator.astro';
import IndicatorBadge from './IndicatorBadge.astro';

<Navbar class='flex justify-between w-full items-center p-1 bg-purple-400'>
    <picture class="flex items-center p-1">
        <Button class='hover:bg-purple-300'>
            <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="20" height="20" viewBox="0 0 24 24" 
                stroke-width="1" stroke="#000000" fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                <path d="M4 6l16 0" />
                <path d="M4 12l16 0" />
                <path d="M4 18l16 0" />
            </svg>
        </Button>
    </picture>
    <ButtonLink url="" class='text-black text-xl hover:font-bold hover:bg-purple-200 rounded-lg p-1'>
        Home
    </ButtonLink>
    <Dropdown class='p-1'>
        <Avatar slot="boton" class="button-dropdown cursor-pointer">
            <Indicator class='px-2 py-1 text-center bg-purple-300 rounded-lg hover:bg-purple-500'>
                <IndicatorBadge class='w-6 h-6 text-[0.6rem] rounded-full bg-purple-950 -top-2 -left-4'>
                    +99
                </IndicatorBadge>
                <div>
                    <svg xmlns="http://www.w3.org/2000/svg" class="close-focus-out rounded-3xl" width="20" 
                        height="20" viewBox="0 0 24 24" stroke-width="1" stroke="#000000" fill="none" 
                        stroke-linecap="round" stroke-linejoin="round">
                        <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                        <path d="M6 19m-2 0a2 2 0 1 0 4 0a2 2 0 1 0 -4 0" />
                        <path d="M17 19m-2 0a2 2 0 1 0 4 0a2 2 0 1 0 -4 0" />
                        <path d="M17 17h-11v-14h-2" />
                        <path d="M6 5l14 1l-1 7h-13" />
                    </svg>
                </div>
            </Indicator>
        </Avatar>
        <div class="w-40 p-2 flex flex-col gap-3 bg-black absolute right-0 bottom-0">
            <h3 class=" font-semibold text-xl">+99 items</h3>
            <span>cost $999</span>
            <Button class=' bg-slate-500'>view card</Button>
        </div>
    </Dropdown>
</Navbar>
```