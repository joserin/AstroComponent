```astro
---
interface Props {
    value : number;
    class?: string;
    [x: string]: any;
}
const { value, class: className, ...rest } = Astro.props;
---
<div class="background-Bar">
    <div class:list={[className]} style={{ width: {value || 0}% }} {...rest}>
        <slot/>
    </div>
</div>
```