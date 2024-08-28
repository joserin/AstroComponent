```astro 
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass='default';
const { class: className = defaulClass, ...rest } = Astro.props;
---
<div class={className} {...rest}>
    <slot/>
</div>
```