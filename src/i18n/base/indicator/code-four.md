```astro 

import Indicator from './Indicator.astro';
import IndicatorBadge from './IndicatorBadge.astro';
import Button from './Button.astro';
import Card from './Card.astro';
import CardHeader from './CardHeader.astro';
import CardContent from './CardContent.astro';

<Indicator>
    <IndicatorBadge class='-bottom-4 -right-10 bg-white'>
        <Button>Next</Button>
    </IndicatorBadge>
    <div>
        <Card class="flex-flex-col justify-center items-center bg-purple-600 w-fit rounded-xl overflow-hidden">
            <CardHeader class="w-fit">
                <img class="w-64 h-52" alt="desk computer" src="/img-2.webp">
            </CardHeader>
            <CardContent class="p-3 flex flex-col">
                <h4 class="font-semibold text-lg">Blog title</h4>
                <p class="p-1">description for this product</p>
            </CardContent>
        </Card>
    </div>
</Indicator>
```