```astro live

//Component Drawer
---
interface Props {
    class?: string;
    [x: string]: any;
}

const defaultClass="default";
const { class: className = defaultClass, ...rest } = Astro.props;
---

<div class={className}>
    <input class="peer" type="checkbox" {...rest}/>
    <slot/>
</div>

//Component Drawer-Label
---
interface Props {
    identifier:string;
    class?: string;
    [x: string]: any;
}
 
const defaultClass="default";
const { identifier, class: className = defaultClass, ...rest } = Astro.props;
---

<label for={identifier} class="default-background peer-checked:block"></label>
<slot>
    <span class={className}>onclick</span>
</slot>

//Component Drawer-Content
---
interface Props {
    class?: string;
    [x: string]: any;
}

const defaultClass="default transform -translate-x-full peer-checked:translate-x-0";
const { class: className = defaultClass, ...rest } = Astro.props;
---

<div class={className} {...rest}>
    <slot/>
</div>
```