```astro
---
interface Props {
    title?: string;
    class?: string;
    [x: string]: any;
}
const defaultClass='default-circle';
const { title, class: className = defaultClass, ...rest } = Astro.props;
---
<div class={className}></div>
<slot>
    <p>{title}</p>
</slot>
```