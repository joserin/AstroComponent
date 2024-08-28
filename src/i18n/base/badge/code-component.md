```astro
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass='default w-10 h-10 bg-blue-300';
const { class: className= defaulClass, ...rest } = Astro.props;
---
<div {...rest} class:list={[className]} >
    <slot/>
</div>
```