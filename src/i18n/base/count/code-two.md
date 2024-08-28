```astro 

import Count from './Count.astro';

<section class="flex gap-1 justify-center items-center m-1 h-60">
    <Count start={24} end={1} time={3600000} class='p-3 text-2xl flex'>h</Count>
    <Count start={59} end={0} time={60000} class='p-3 text-2xl flex'>m</Count>
    <Count start={59} end={0} time={1000} class='p-3 text-2xl flex'>s</Count>
</section>
```