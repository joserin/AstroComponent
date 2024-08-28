```astro

import Alert from './Alert.astro';

<section class="flex flex-col gap-5 justify-center items-center h-60">
  <Alert class='default text-red-400 font-semibold border-2 border-red-400 flex justify-center items-center'>
        <picture>
            <svg class="text-red-500 dark:text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" 
            width="24" height="24" fill="none" viewBox="0 0 24 24">
                <path stroke="currentColor" stroke-linecap="round" stroke-width="2" d="m6 6 12 12m3-6a9 9 0 1 
                1-18 0 9 9 0 0 1 18 0Z"/>
            </svg>
        </picture>
        <p>Error! Task failed successfully.</p>
        <Button class='px-2 py-1  hover:bg-red-200 rounded text-center transition focus-visible:ring-2 
        ring-offset-2 ring-gray-200 underline'>See</Button>
    </Alert>
</section>
```