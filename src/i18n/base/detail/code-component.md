```astro
---
interface Props {
    title?:string;
    class?: string;
    [x: string]: any;
}
const defaultClass='default';
const { title, class: className = defaultClass, ...rest } = Astro.props;
---

<details class={className} {...rest}>
    <slot name="title">
        <summary>{title}</summary>
    </slot>
    <slot/>
</details>

```