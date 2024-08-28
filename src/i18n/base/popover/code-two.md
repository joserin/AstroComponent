```astro

import Popover from './Popover.astro';

<Popover class='h-fit p-1'>
    <button slot="boton-action" class="button-popover">
        <svg xmlns="http://www.w3.org/2000/svg" class="icon pointer-events-none" width="30" 
        height="30" viewBox="0 0 24 24" stroke-width="1.5" stroke="#000000" fill="none" 
        stroke-linecap="round" stroke-linejoin="round">
            <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
            <path d="M12 4c4.29 0 7.863 2.429 10.665 7.154l.22 .379l.045 .1l.03 .083l.014 
            .055l.014 .082l.011 .1v.11l-.014 .111a.992 .992 0 0 1 -.026 .11l-.039 .108l-.036 
            .075l-.016 .03c-2.764 4.836 -6.3 7.38 -10.555 7.499l-.313 .004c-4.396 0 -8.037 
            -2.549 -10.868 -7.504a1 1 0 0 1 0 -.992c2.831 -4.955 6.472 -7.504 10.868 -7.504zm0 
            5a3 3 0 1 0 0 6a3 3 0 0 0 0 -6z" stroke-width="0" fill="currentColor" />
        </svg>
    </button>
    <div>
        <header>
            <h4>Title</h4>
            <p>this is a example</p>
        </header>
        <main class="flex flex-col justify-between p-1">
            <section class="flex justify-between gap-1 items-center">
                <span>Name</span>
                <input class="text-black p-1 border border-purple-300" type="text">
            </section>
            <section class="flex justify-between gap-1 items-center">
                <span>Age</span>
                <input class="text-black p-1 border border-purple-300" type="number">
            </section>
            <section class="flex justify-between gap-1 items-center">
                <span>Email</span>
                <input class="text-black p-1 border border-purple-300" type="email">
            </section>
        </main>
    </div>
</Popover>
```