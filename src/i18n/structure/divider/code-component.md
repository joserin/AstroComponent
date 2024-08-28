```astro live

//Component Divider
---
interface Props {
    class?: string;
    direction?: "horizontal" | "vertical"
    [x: string]: any;
}
const { direction ="vertical", class: className, ...rest } = Astro.props;
---
<div class="flex items-center">
    <div class={direction}>
        <div {...rest} class:list={[className]}></div>
        <slot/>
        <div {...rest} class:list={[className]}></div>
    </div>
</div>

//Component Divider
---
interface Props {
    class?: string;
    [x: string]: any;
}
const { class: className, ...rest } = Astro.props;
---
<span {...rest} class={className}>
    <slot> / </slot>
</span>
```