```astro

import Detail from './Detail.astro';

<div class="bg-purple-800 w-fit flex h-fit">
    <Detail title='first' name="test">
        <ul class=" bg-purple-700 w-32 h-fit absolute text-sm p-1 mt-2 flex flex-col gap-3">
            <li>My Information</li>
            <li>Profile</li>
        </ul>
    </Detail>
    <Detail title='second' name="test">
        <ul class=" bg-purple-600 w-32 h-fit absolute text-sm p-1 mt-2 flex flex-col gap-3">
            <li>Pay</li>
        </ul>
    </Detail>
    <Detail title='third' name="test">
        <ul class=" bg-purple-700 w-32 h-fit absolute text-sm p-1 mt-2 flex flex-col gap-3">
            <li>Github</li>
            <li>Facebook</li>
        </ul>
    </Detail>
</div>

```