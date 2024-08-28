```astro

import Badge from './badge.astro';

<Badge class=" rounded-xl bg-red-400 p-1 w-fit flex justify-center items-center">
    <svg class="w-5 h-5 text-gray-800 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" 
        width="24" height="24" fill="none" viewBox="0 0 24 24">
        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 11.917 
            9.724 16.5 19 7.5"/>
    </svg>
    <span>red</span>
</Badge>
<Badge class=" rounded-xl bg-blue-400 p-1 w-fit flex justify-center items-center">
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-4 h-4 stroke-current">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
    </svg>
    <span>blue</span>
</Badge>
<Badge class=" rounded-xl bg-pink-400 p-1 w-fit flex justify-center items-center">
    <span>pink</span>
    <Button class=" bg-transparent">
        <svg class="w-5 h-5 text-gray-800 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" 
            width="24" height="24" fill="none" viewBox="0 0 24 24">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 11.917 
                9.724 16.5 19 7.5"/>
        </svg>
    </Button>
</Badge>
<Badge class=" rounded-xl bg-purple-400 p-1 w-fit">
    <span>purple</span>
    <Button class=" bg-transparent">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-4 h-4 
            stroke-current">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12">
            </path>
        </svg>
    </Button>
</Badge>
```