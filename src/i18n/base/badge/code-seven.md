```astro

import Badge from './badge.astro';

<Button class="flex bg-slate-700 hover:bg-slate-400 p-2 rounded-xl gap-2 items-center justify-center">
    <p>Inbox</p>
    <Badge class=" bg-slate-500 rounded-lg p-1 text-sm font-semibold">+99</Badge>
</Button>
<Button class="flex bg-pink-700 hover:bg-slate-400 p-2 rounded-xl gap-2 items-center justify-center">
    <p>Inbox</p>
    <Badge class=" bg-pink-400 rounded-lg p-1 text-sm text-white font-semibold">+99</Badge>
</Button>
```