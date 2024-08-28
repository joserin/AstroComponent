```astro
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass='default';
const { class: className = defaulClass, ...rest } = Astro.props;
---

<div class="tooltip">
    <main class:list={[className, "tooltipop"]}>
        <slot name="content">
            ????
        </slot>
    </main>
    <slot/>
</div>
```