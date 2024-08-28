```astro live
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass='w-full h-full';
const { class: className= defaulClass, ...rest } = Astro.props;
---

<div {...rest} class:list={[className]}>
    <slot/>
</div>
```