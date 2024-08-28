```astro
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