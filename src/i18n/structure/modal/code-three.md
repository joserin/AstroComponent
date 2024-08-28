```astro live

import Modal from './Modal.astro';
import Button from './Button.astro';

<Modal buttonText='abrir 2'>
    <div class="flex flex-col gap-5 bg-green-200 p-5">
        <header>
            <h5 class="text-2xl">Log in</h5>
        </header>
        <div>
            <p>Press button cerrar to close</p>
        </div>
        <footer class="flex justify-center">
            <Button class="px-2 py-1 bg-yellow-200 hover:bg-yellow-300 w-fit" >Agregar</Button>
            <Button class="modal-close px-2 py-1 bg-yellow-200 hover:bg-yellow-300 w-fit" >cerrar 2</Button>
        </footer>
    </div>
</Modal>
```