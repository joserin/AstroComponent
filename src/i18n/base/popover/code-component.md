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
<div class="relative element-popover">
    <slot name="boton-action">
        <button class="button-popover">
            {title}
        </button>
    </slot>
    <span class:list={[className, "popover-display", "hide"]} {...rest}>
        <slot/>
    </span>
</div>
```