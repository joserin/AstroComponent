```astro live
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaultClass='default';
const { class: className = defaultClass, ...rest } = Astro.props;
---
<div {...rest} class={className}>
    <slot/>
</div>
```