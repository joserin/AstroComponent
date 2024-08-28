```astro live

import Modal from './Modal.astro';
import Button from './Button.astro';

<Modal>
    <Button slot="button-open" class="button-modal border p-1">abrir 3</Button>
    <div class="bg-green-200 p-2 relative">
        <header>
            <h5 class="text-2xl">Log in</h5>
            <span class="absolute w-fit right-0 top-0 p-1">
                <Button class="modal-close p-1 hover:bg-yellow-300 w-fit rounded-full">
                    <svg class="w-6 h-6 text-gray-800 dark:text-white" aria-hidden="true" 
                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" 
                            stroke-width="2" d="M6 18 17.94 6M18 18 6.06 6"/>
                    </svg>
                </Button>
            </span>
        </header>
        <div class="flex flex-col gap-3">
            <p>Press button cerrar to close</p>
        </div>
    </div>
</Modal>
```