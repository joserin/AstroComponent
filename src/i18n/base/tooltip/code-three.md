```astro

import Tooltip from './Tooltip.astro';

<Tooltip class='bg-white top-[105%] left-16' >
    show tooltip on bottom
    <div slot="content">
        <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" 
        stroke-width="1.5" stroke="#ff2825" fill="none" stroke-linecap="round" stroke-linejoin="round">
            <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
            <path d="M15.349 5.349l3.301 3.301a1.2 1.2 0 0 1 0 1.698l-.972 .972a7.5 7.5 0 1 1 -5 
            -5l.972 -.972a1.2 1.2 0 0 1 1.698 0z" />
            <path d="M17 7l1.293 -1.293a2.414 2.414 0 0 0 .707 -1.707a1 1 0 0 1 1 -1h1" />
            <path d="M7 13a3 3 0 0 1 3 -3" />
        </svg>
    </div>
</Tooltip>
```