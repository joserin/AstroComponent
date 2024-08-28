```astro

import Tab from './Tab.astro';
import TabHead from './Tab-head.astro';
import TabContent from './Tab-Content.astro';

<Tab>
    <header class="flex gap-3">
        <TabHead>One</TabHead>
        <TabHead>Two</TabHead>
        <TabHead>Three</TabHead>
    </header>
    <div class="w-full h-full overflow-hidden">
            <TabContent class='bg-yellow-600 h-full'>
                <p>One upon a time</p>
            </TabContent>
            <TabContent class='bg-blue-700 h-full'>
                <p>two time slash</p>
            </TabContentiv>
            <TabContent class='bg-red-700 h-full'>
                <p>Three weeks ago</p>
            </TabContent>
    </div>
</Tab>
```