```astro 

import Indicator from './Indicator.astro';
import IndicatorBadge from './IndicatorBadge.astro';

<Indicator>
    <IndicatorBadge class='-bottom-4 -left-10 bg-black px-1'>
        <span>write me</span>
    </IndicatorBadge>
    <div>
        <input class='border-2 border-slate-500 p-2' type="email" placeholder="your email address"/>
    </div>
</Indicator>
```