```astro live

import Collapse from './Collapse.astro';

<section class="flex gap-1 justify-center items-center m-1 h-60">
    <Collapse>
        <button slot="boton" class='flex justify-between gap-2 collapse-Button p-2'>
            <p>This is a test</p>
            <picture class="icon-rotate">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" 
                    stroke-width="1.5" stroke="#2c3e50" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M15 12h3.586a1 1 0 0 1 .707 1.707l-6.586 6.586a1 1 0 0 1 -1.414 0l-6.586 -6.586a1 1 0 0 1 .707 
                        -1.707h3.586v-3h6v3z" />
                    <path d="M15 3h-6" />
                    <path d="M15 6h-6" />
                </svg>
            </picture>
        </button>
        <div class="w-96">
            segundo asalto: Lorem, ipsum dolor sit amet consectetur adipisicing elit. Optio debitis ratione, vel doloribus, 
            asperiores at harum repudiandae fuga quibusdam accusamus velit consequuntur! Quaerat cupiditate doloribus tempore 
            odio deserunt culpa asperiores.
        </div>
    </Collapse>
</section>
```