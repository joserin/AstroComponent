```astro

import Avatar from './Avatar.astro';
import ChatBubbles from './ChatBubbles.astro';
import Button from './Button.astro';

<section class="flex gap-1 justify-center m-1 h-60">
    <Avatar class='w-10 h-10'>
        <img class=" rounded-full" src="/img-2.webp" 
        alt="">
    </Avatar>
    <ChatBubbles class='flex flex-col bg-blue-300 p-3 w-[400px] rounded-xl gap-3'>
        <header class='flex gap-2'>
            <h3 class="font-bold">Boby dogs</h3>
            <span>1:30</span>
        </header>
        <main class='flex gap-5'>
            <Button class='w-10 h-10 hover:bg-red-400 rounded-xl'>
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-player-pause" 
                width="44" height="44" viewBox="0 0 24 24" stroke-width="1.5" stroke="#2c3e50" fill="none" 
                stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M6 5m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v12a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z" />
                    <path d="M14 5m0 1a1 1 0 0 1 1 -1h2a1 1 0 0 1 1 1v12a1 1 0 0 1 -1 1h-2a1 1 0 0 1 -1 -1z" />
                </svg>
            </Button>
            <picture>
                <svg aria-hidden="true" class="w-[145px] md:w-[185px] md:h-[40px]" viewBox="0 0 185 40" 
                fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect y="17" width="3" height="6" rx="1.5" fill="#6B7280" />
                    <rect x="7" y="15.5" width="3" height="9" rx="1.5" fill="#6B7280" />
                    <rect x="21" y="6.5" width="3" height="27" rx="1.5" fill="#6B7280" />
                    <rect x="14" y="6.5" width="3" height="27" rx="1.5" fill="#6B7280" />
                    <rect x="28" y="3" width="3" height="34" rx="1.5" fill="#6B7280" />
                    <rect x="35" y="3" width="3" height="34" rx="1.5" fill="#6B7280" />
                    <rect x="42" y="5.5" width="3" height="29" rx="1.5" fill="#6B7280" />
                    <rect x="49" y="10" width="3" height="20" rx="1.5" fill="#6B7280" />
                    <rect x="56" y="13.5" width="3" height="13" rx="1.5" fill="#6B7280" />
                    <rect x="63" y="16" width="3" height="8" rx="1.5" fill="#6B7280" />
                    <rect x="70" y="12.5" width="3" height="15" rx="1.5" fill="#E5E7EB"/>
                    <rect x="77" y="3" width="3" height="34" rx="1.5" fill="#E5E7EB"/>
                    <rect x="84" y="3" width="3" height="34" rx="1.5" fill="#E5E7EB"/>
                    <rect x="91" y="0.5" width="3" height="39" rx="1.5" fill="#E5E7EB"/>
                    <rect x="98" y="0.5" width="3" height="39" rx="1.5" fill="#E5E7EB"/>
                    <rect x="105" y="2" width="3" height="36" rx="1.5" fill="#E5E7EB"/>
                    <rect x="112" y="6.5" width="3" height="27" rx="1.5" fill="#E5E7EB"/>
                    <rect x="119" y="9" width="3" height="22" rx="1.5" fill="#E5E7EB"/>
                    <rect x="126" y="11.5" width="3" height="17" rx="1.5" fill="#E5E7EB"/>
                    <rect x="133" y="2" width="3" height="36" rx="1.5" fill="#E5E7EB"/>
                    <rect x="140" y="2" width="3" height="36" rx="1.5" fill="#E5E7EB"/>
                    <rect x="147" y="7" width="3" height="26" rx="1.5" fill="#E5E7EB"/>
                    <rect x="154" y="9" width="3" height="22" rx="1.5" fill="#E5E7EB"/>
                    <rect x="161" y="9" width="3" height="22" rx="1.5" fill="#E5E7EB"/>
                    <rect x="168" y="13.5" width="3" height="13" rx="1.5" fill="#E5E7EB"/>
                    <rect x="175" y="16" width="3" height="8" rx="1.5" fill="#E5E7EB"/>
                    <rect x="182" y="17.5" width="3" height="5" rx="1.5" fill="#E5E7EB"/>
                    <rect x="66" y="16" width="8" height="8" rx="4" fill="#1C64F2"/>
                </svg>
            </picture>
         </main>
        <footer>
            <p>send</p>
        </footer>
    </ChatBubbles>
</section>
```