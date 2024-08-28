```astro live

import Modal from './Modal.astro';
import Button from './Button.astro';

<Modal buttonText="open 4" class='modal-closeClick'>
    <div class='bg-white flex flex-col gap-3 p-5'>
        <header>
            <h5 class="text-2xl">title</h5>
        </header>
        <div>
            <p>Click outside to close</p>
        </div>
        <footer class="flex justify-end">
            <Button class="modal-close px-2 py-1 bg-slate-200 hover:bg-slate-300 w-fit" >cerrar </Button>
        </footer>
    </div>
</Modal>
```