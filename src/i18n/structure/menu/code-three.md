```astro live

import Menu from './Menu.astro';
import MenuElement from './MenuElement.astro';

<Menu>
    <MenuElement class='hover:bg-slate-300 p-1 rounded-xl'>
        <a href="">
            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24" 
                stroke-width="1.5" stroke="#000000" fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                <path d="M5 12l-2 0l9 -9l9 9l-2 0" />
                <path d="M5 12v7a2 2 0 0 0 2 2h10a2 2 0 0 0 2 -2v-7" />
                <path d="M10 12h4v4h-4z" />
            </svg>
        </a>
    </MenuElement>
    <MenuElement class='hover:bg-slate-300 p-1 rounded-xl'>
        <a href="">
            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24" 
                stroke-width="1.5" stroke="#000000" fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                <path d="M12 9h.01" />
                <path d="M11 12h1v4h1" />
                <path d="M12 3c7.2 0 9 1.8 9 9s-1.8 9 -9 9s-9 -1.8 -9 -9s1.8 -9 9 -9z" />
            </svg>
        </a>
    </MenuElement>
    <MenuElement class='hover:bg-slate-300 p-1 rounded-xl'>
        <a href="">
            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24" 
                stroke-width="1.5" stroke="#000000" fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                <path d="M6 18l0 -3" />
                <path d="M10 18l0 -6" />
                <path d="M14 18l0 -9" />
                <path d="M18 18l0 -12" />
            </svg>
        </a>
    </MenuElement>
</Menu>
```