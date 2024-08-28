```astro live
---
interface Props {
    buttonText?: string;
    class?: string;
    [x: string]: any;
}
const { buttonText, class: className, ...rest } = Astro.props;
---
<div class="modal-content">
    <slot name="button-open">
        <button class="button-modal">{buttonText}</button>
    </slot>
    <dialog class:list={["hidden modal-background", className]}>
        <slot/>
    </dialog>
</div>
```