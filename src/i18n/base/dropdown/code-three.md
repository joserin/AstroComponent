```astro

import Dropdown from './Dropdown.astro';

<Dropdown>
    <button slot="boton" class="button-dropdown p-1">Information</button>
    <ul tabindex="0" class="bg-red-400 w-36 p-3 flex flex-col gap-2 right-0">
        <li>My Information</li>
        <li>Profile</li>
    </ul>
</Dropdown>
<Dropdown>
    <button slot="boton" class="button-dropdown p-1">Help</button>
    <ul tabindex="0" class="bg-green-400 w-fit p-3 flex flex-col gap-2 right-0">
        <li>Support</li>
        <li>Number</li>
        <li>Contact</li>
    </ul>
</Dropdown>
<Dropdown>
    <button slot="boton" class="button-dropdown p-1">Feedback</button>
    <ul tabindex="0" class="bg-blue-400 w-fit p-3 flex flex-col gap-2 right-0">
        <li>Time</li>
        <li>Advertising</li>
    </ul>
</Dropdown>
```