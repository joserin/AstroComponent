```astro live

//Component Menu
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaultClass='default';
const { class: className = defaultClass, ...rest } = Astro.props;
---
<ul {...rest} class={className}>
    <slot/>
</ul>

//Component MenuElement
---
interface Props {
    class?: string;
    [x: string]: any;
}
const { class: className, ...rest } = Astro.props;
---
<li {...rest} class={className}>
    <slot/>
</li>
```