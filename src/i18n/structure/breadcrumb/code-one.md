```astro live

import Breadcrumb from './Breadcrumb.astro';
import BreadcrumbLink from './BreadcrumbLink.astro';
import Beteewn from './Beteewn.astro';

<Breadcrumb>
    <BreadcrumbLink url="/">Home</BreadcrumbLink>
    <Beteewn/>
    <BreadcrumbLink url="/component/">Components</BreadcrumbLink>
    <Beteewn/>
    <BreadcrumbLink url="/component/Breadcrumbs/">Breadcrumbs</BreadcrumbLink>
</Breadcrumb>
```