```astro live

import Modal from './Modal.astro';
import Button from './Button.astro';

<Modal buttonText='open' class="flex flex-col gap-5 p-5 rounded-xl transition-opacity duration-500">
    <div class='bg-white flex flex-col gap-3 p-3'>
        <header>
            <h5 class="text-2xl">Title</h5>
        </header>
        <div>
            <p>Press button cerrar to close</p>
        </div>
        <footer class="flex justify-end">
            <Button class="modal-close px-2 py-1 bg-slate-200 hover:bg-slate-300 w-fit" >cerrar </Button>
        </footer>
    </div>
</Modal>
```