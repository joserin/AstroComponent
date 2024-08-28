```astro 

import Tab from './Tab.astro';
import TabHead from './Tab-head.astro';
import TabContent from './Tab-Content.astro';

<Tab class='flex relative w-full h-full'>
    <div class="flex flex-col gap-1 w-fit">
        <TabHead class=' hover:bg-yellow-600 p-1'>One</TabHead>
        <TabHead class='hover:bg-blue-700 p-1'>Two</TabHead>
        <TabHead class='hover:bg-red-700 p-1'>Three</TabHead>
    </div>
    <div class="w-full">
        <TabContent class='active bg-yellow-600 h-full'>
            <p>One upon a time</p>
        </TabContent>
        <TabContent class='deactive bg-blue-700 h-full'>
            <p>two time slash</p>
        </TabContentiv>
        <TabContent class='deactive bg-red-700 h-full'>
            <p>Three weeks ago</p>
        </TabContent>
    </div>
</Tab>
```