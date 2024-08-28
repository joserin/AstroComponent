```astro live

import Collapse from './Collapse.astro';

<section class="flex gap-1 justify-center items-center m-1 h-60">
    <div class="flex relative w-44 justify-center border-[1px] border-black">
        <Collapse class='p-1 absolute left-0'>
            <button slot="boton" class='flex justify-between gap-2 collapse-Button'>
                <picture class=" hover:bg-slate-500 bg-opacity-9">
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" stroke-width="1.5" stroke="#ffffff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                        <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                        <path d="M12 20h-6a2 2 0 0 1 -2 -2v-12a2 2 0 0 1 2 -2h6" />
                        <path d="M18 14v7" />
                        <path d="M18 3v7" />
                        <path d="M15 18l3 3l3 -3" />
                        <path d="M15 6l3 -3l3 3" />
                    </svg>
                </picture>
            </button>
            <div>
                <p>uno</p>
                <p>two</p>
            </div>
        </Collapse>
        <p>3 repositories</p>
    </div>
</section>
```