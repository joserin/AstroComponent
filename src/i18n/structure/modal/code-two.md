```astro live

import Modal from './Modal.astro';
import Button from './Button.astro';

<Modal class="flex flex-col gap-5 p-5 rounded-xl transition-opacity duration-500 modal-closeEsc">
    <Button slot='button-open' class="px-2 py-1 rounded-xl bg-red-300 hover:bg-red-500 button-modal">
        opened
    </Button>
    <div class='bg-white flex flex-col gap-3 p-5'>
        <header>
            <h5 class="text-2xl">Title</h5>
        </header>
        <div>
            <p>Press ESC key button to close</p>
        </div>
    </div>
</Modal>
```