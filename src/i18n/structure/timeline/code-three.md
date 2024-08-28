```astro

import Timeline from './Timeline.astro';
import LineElement from './LineElement.astro';
import LineContent from './LineContent.astro';

<Timeline class='w-fit flex-col'>
    <LineElement class='flex h-[50px]'>
        <LineContent class='bg-red-600 vertical absolute top-8 left-2'>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" 
            fill="currentColor" class="w-5 h-5">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 
                16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 
                10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z" clip-rule="evenodd" />
            </svg>
        </LineContent>
        <span class="text-sm flex items-center">First Macintosh computer</span>
    </LineElement>
    <LineElement class='flex h-[50px]'>
        <LineContent class='bg-red-600 vertical absolute top-8 left-2'>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" 
            fill="currentColor" class="w-5 h-5">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 
                16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 
                10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z" clip-rule="evenodd" />
            </svg>
        </LineContent>
        <span class="text-sm flex items-center">iMac</span>
    </LineElement>
    <LineElement class='flex h-[50px]'>
        <LineContent class='bg-blue-600 vertical absolute top-8 left-2'>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" 
            fill="currentColor" class="w-5 h-5">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 
                0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 
                001.137-.089l4-5.5z" clip-rule="evenodd" />
            </svg>
        </LineContent>
        <span class="text-sm flex items-center">iPod</span>
    </LineElement>
    <LineElement class='flex h-[50px]'>
        <LineContent class='bg-blue-600 vertical absolute top-8 left-2'>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" 
            fill="currentColor" class="w-5 h-5">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 
                16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 
                10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z" clip-rule="evenodd" />
            </svg>
        </LineContent>
        <span class="text-sm flex items-center">iPhone</span>
    </LineElement>
    <LineElement class='flex h-[50px]'>
        <LineContent endLine={true}>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" 
            fill="currentColor" class="w-5 h-5">
                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 
                0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 
                001.137-.089l4-5.5z" clip-rule="evenodd" />
            </svg>
        </LineContent>
        <span class="text-sm flex items-center">Apple Watch</span>
    </LineElement>
</Timeline>
```