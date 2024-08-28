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

<div class="dropdown">
    <slot name="boton">
        <button class="button-dropdown default-button">{title}</button>
    </slot>
    <div class:list={["dropdown-content", className]} {...rest}>
        <slot/>
    </div>
</div>
```