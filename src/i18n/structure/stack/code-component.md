```astro live
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass='default';
const { class: className = defaulClass, ...rest } = Astro.props;
---

<div class:list={[className, 'stack']} {...rest}>
    <slot/>
</div>
```