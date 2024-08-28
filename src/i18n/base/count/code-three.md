```astro 

import Count from './Count.astro';

<section class="flex gap-1 justify-center items-center m-1 h-60">
    <Count start={7} end={1} time={30000} class='text-2xl bg-red-700 flex flex-col justify-center items-center'>
        <span class="bg-yellow-400">emi</span>
    </Count>
    <Count start={6} end={1} time={5000} class='text-2xl bg-red-500 flex flex-col justify-center items-center'>
        <span class="bg-yellow-400 w-full">ext</span>
    </Count>
    <Count start={5} end={1} time={1000} class='text-2xl bg-red-300 flex flex-col justify-center items-center'>
        <span class="bg-yellow-400">mil</span>
    </Count>
</section>
```