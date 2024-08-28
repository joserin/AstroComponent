```astro
//Component Resizable
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass='default';
const { class: className= defaulClass, ...rest } = Astro.props;
---

<div class={className}>
    <slot/>
</div>

//Component Resizable Panel
---
interface Props {
    position?: 'side' | 'bottom';
    class?: string;
    [x: string]: any;
}

const defaulClass='resize-x bg-red-300 w-20 h-20';
const { position, class: className= defaulClass, ...rest } = Astro.props;
---

<div class="elemento">
    <slot/>
    {
        position !== undefined && <div class:list={[position, 'resizable__control']}></div>
    }
</div>
```