```astro 
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass='default';
const { class: className = defaulClass, ...rest } = Astro.props;
---
<section>
    <span class="buttonToast">
        <slot name="toastButton" />
    </span>
    <span class="hidden">
        <div class:list={[className, 'toast']} {...rest}>
            <slot/>
        </div>
    </span>
</section>
```