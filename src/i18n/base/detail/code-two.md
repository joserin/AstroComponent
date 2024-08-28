```astro

import Detail from './Detail.astro';

<Detail class='w-36 flex flex-col'>
    <summary slot="title" class="border border-blue-200 text-xl bg-black p-1 w-full">
        click me
    </summary>
    <ul class="bg-black w-40 text-sm p-3 flex flex-col gap-3">
        <li>My Information</li>
        <li>Profile</li>
        <li>Team</li>
        <li>Keyboard image</li>
        <li>Power level english</li>
    </ul>
</Detail>

```