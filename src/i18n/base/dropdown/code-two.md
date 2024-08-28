```astro

import Dropdown from './Dropdown.astro';

<Dropdown tabindex="0">
    <button slot="boton" class="button-dropdown border border-blue-200 p-1">
        <p class="close-focus-out">click me</p>
    </button>
    <ul tabindex="0" class="bg-black w-40 text-sm p-3 flex flex-col gap-3">
        <li>My Information</li>
        <li>Profile</li>
        <li>Team</li>
        <li>Keyboard image</li>
        <li>Power level english</li>
    </ul>
</Dropdown>
```