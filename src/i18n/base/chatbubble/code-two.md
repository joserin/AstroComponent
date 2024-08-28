```astro

import ChatBubbles from './ChatBubbles.astro';
import Avatar from './Avatar.astro';

<section class="flex gap-1 justify-center items-center m-1 h-60">
    <Avatar>
        <img class=" rounded-full" src="/img-1.webp" 
        alt="photo">
    </Avatar>
    <ChatBubbles class='flex flex-col bg-green-400 p-3 w-[400px] rounded-xl gap-3'>
        <header>
            <h3 class="font-bold">Bonnie Green</h3>
        </header>
        <div>
            <p>That's awesome. I think our users will really appreciate the improvements.</p>
        </div>
        <footer>
            <p>Delivered</p>
        </footer>
    </ChatBubbles>
</section>
```