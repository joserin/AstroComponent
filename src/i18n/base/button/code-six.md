```astro 

import Button from './Button.astro';

<Button class="px-2 py-1 border-2 border-blue-100 active:bg-blue-300 
    hover:bg-blue-200 flex justify-center items-center rounded-lg font-semibold">
    <svg class="w-[30px] h-[25px] text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" 
    width="24" height="24" fill="currentColor" viewBox="0 0 24 24">
        <path fill-rule="evenodd" d="M13.135 6H15V3h-1.865a4.147 4.147 0 0 0-4.142 
            4.142V9H7v3h2v9.938h3V12h2.021l.592-3H12V6.591A.6.6 0 0 1 12.592 6h.543Z" clip-rule="evenodd"/>
        </svg>
    <span> Facebook </span>
</Button>
<Button class="px-2 py-1 border-2 border-blue-100 active:bg-blue-300 hover:bg-blue-200 
    flex justify-center items-center rounded-lg font-semibold">
    <svg class="w-[30px] h-[25px] text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" 
        width="24" height="24" fill="currentColor" viewBox="0 0 24 24">
            <path fill-rule="evenodd" d="M22 5.892a8.178 8.178 0 0 1-2.355.635 4.074 4.074 0 0 0 1.8-2.235 
            8.343 8.343 0 0 1-2.605.981A4.13 4.13 0 0 0 15.85 4a4.068 4.068 0 0 0-4.1 4.038c0 
            .31.035.618.105.919A11.705 11.705 0 0 1 3.4 4.734a4.006 4.006 0 0 0 1.268 5.392 4.165 
            4.165 0 0 1-1.859-.5v.05A4.057 4.057 0 0 0 6.1 13.635a4.192 4.192 0 0 1-1.856.07 4.108 
            4.108 0 0 0 3.831 2.807A8.36 8.36 0 0 1 2 18.184 11.732 11.732 0 0 0 8.291 20 11.502 
            11.502 0 0 0 19.964 8.5c0-.177 0-.349-.012-.523A8.143 8.143 0 0 0 22 5.892Z" clip-rule="evenodd"/>
    </svg>
    <span> Twitter </span>
</Button>
```