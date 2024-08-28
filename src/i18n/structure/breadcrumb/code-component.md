```astro live

//Component Breadcrumb
---
interface Props {
    class?: string;
    [x: string]: any;
}

const defaulClass='default';
const { class: className= defaulClass, ...rest } = Astro.props;
---
<div {...rest} class={className}>
    <slot/>
</div>

// Component BreadcrumbLink
---
interface Props {
    url: string;
    class?: string;
    [x: string]: any;
}
const defaulClass='p-1 m-1 flex';
const { url, class: className= defaulClass, ...rest } = Astro.props;
---
<a href={url} {...rest} class={className}>
    <slot/>
</a>
```