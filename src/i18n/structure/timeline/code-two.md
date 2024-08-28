```astro 

import Timeline from './Timeline.astro';
import LineElement from './LineElement.astro';
import LineContent from './LineContent.astro';

<Timeline class='default w-fit justify-center'>
    <LineElement class='w-56'>
        <span>First Macintosh computer</span>
        <LineContent class='bg-red-600 horizontal'>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" 
            fill="currentColor" class="w-5 h-5">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 
                16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 
                10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z" clip-rule="evenodd" />
            </svg>
        </LineContent>
    </LineElement>
    <LineElement class='w-20'>
        <span>iMac</span>
        <LineContent class='bg-red-600 horizontal'>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" 
            fill="currentColor" class="w-5 h-5">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 
                0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 
                001.137-.089l4-5.5z" clip-rule="evenodd" />
            </svg>
        </LineContent>
    </LineElement>
    <LineElement class='w-20'>
        <span>iPod</span>
        <LineContent class='bg-blue-600 horizontal'>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" 
            fill="currentColor" class="w-5 h-5">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 
                0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0
                001.137-.089l4-5.5z" clip-rule="evenodd" />
            </svg>
        </LineContent>
    </LineElement>
    <LineElement class='w-20 '>
        <span>iPhone</span>
        <LineContent class='bg-blue-600 horizontal'>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" 
            fill="currentColor" class="w-5 h-5">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 
                0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 
                001.137-.089l4-5.5z" clip-rule="evenodd" />
            </svg>
        </LineContent>
    </LineElement>
    <LineElement class=' w-32'>
        <span>Apple Watch</span>
        <LineContent endLine={true}>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" 
            fill="currentColor" class="w-5 h-5">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 
                16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 
                10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z" clip-rule="evenodd" />
            </svg>
        </LineContent>
    </LineElement>
</Timeline>
```