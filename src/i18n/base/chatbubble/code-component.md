```astro
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass='default';
const { class: className = defaulClass, ...rest } = Astro.props;
---

<div {...rest} class={className}>
    <slot/>
</div>
```