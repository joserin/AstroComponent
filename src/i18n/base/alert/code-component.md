```astro
---
interface Props {
    class?: string;
    [x: string]: any;
}

const defaultClass="default text-black bg-white";
const { class: className = defaultClass, ...rest } = Astro.props;
---

<div {...rest} class={className} role="alert">
    <slot/>
</div>
```