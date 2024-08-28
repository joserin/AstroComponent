```astro

import RadialProgress from './RadialProgress.astro';

<RadialProgress value={10} strokeW={1} class='text-yellow-400'>
    <span class=" text-white">10%</span>
</RadialProgress>
<RadialProgress value={60} strokeW={2}>
    <span class=" text-white">60%</span>
</RadialProgress>
<RadialProgress value={90} strokeW={3} class='text-red-600'>
    <span class=" text-white">90%</span>
</RadialProgress>
```