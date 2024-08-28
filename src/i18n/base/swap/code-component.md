```astro 
---
interface Props {
    class?: string;
    [x: string]: any;
}

const { class: className, ...rest } = Astro.props;
---
<div {...rest} class:list={[className, 'swap-container']}>
    <input class="z-[1] peer" type="checkbox"/>
    <div class="peer-checked:hidden">
        <slot name="first-state"/>
    </div>
    <div class="hidden peer-checked:block">
        <slot name="second-state"/>
    </div>
</div>
```