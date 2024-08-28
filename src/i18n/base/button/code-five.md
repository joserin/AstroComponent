```astro 

import Button from './Button.astro';

<Button class="px-2 py-1 border-2 border-blue-100 active:bg-blue-300 
    hover:bg-blue-200 flex justify-center items-center rounded-lg">
    <span> Button Text </span>
    <svg class="w-[40px] h-[30px] text-white" aria-hidden="true" 
        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" 
        viewBox="0 0 24 24">
        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" 
        stroke-width="1.1" d="M20 12H8m12 0-4 4m4-4-4-4M9 4H7a3 3 0 0 0-3 
        3v10a3 3 0 0 0 3 3h2"/>
    </svg>
</Button>
```