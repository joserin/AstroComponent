```astro
---
interface Props {
    class?: string;
    [x: string]: any;
}

const defaulClass='default';
const { class: className = defaulClass, ...rest } = Astro.props;
---

<div class:list={[className]}>
    <input {...rest} type="range" class="slider-style"/>
    <slot/>
</div>
```