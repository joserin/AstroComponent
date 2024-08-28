```astro live
---
interface Props {
    title?:string;
    class?: string;
    [x: string]: any;
}

const defaulClass='default bg-purple-400 hover:bg-purple-600';
const { title, class: className = defaulClass, ...rest } = Astro.props;
---

<div class={className}>
    <slot name="boton">
        <button {...rest} class="collapse-Button px-2 py-1 w-fit h-fit">{title}</button>
    </slot>
    <main class="hidden overflow-hidden">
        <slot/>
    </main>
</div>
```