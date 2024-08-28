```astro 
// Component Indicator
---
interface Props {
    class?: string;
    [x: string]: any;
}
const { class: className, ...rest } = Astro.props;
---
<div class:list={[className, "container-indicator"]} {...rest}>
    <slot/>
</div>

// Component Indicator-Badge
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaultClass='default';
const { class: className = defaultClass, ...rest } = Astro.props;
---
<span class={className} {...rest}>
    <slot/>
</span>
```