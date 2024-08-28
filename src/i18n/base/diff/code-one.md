```astro

import Diff from './Diff.astro';

<Diff class='w-[300px]'>
  <img slot="first-image" src="/img-2.webp" alt="color photo" />
  <img slot="second-image" src="/img-2.webp" alt="black and white" class="blur-sm cover-background"/>
</Diff>
```