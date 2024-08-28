```astro live

// Component Carousel
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaultClass="default";
const { class: className = defaultClass, ...rest } = Astro.props;
---
<picture class={className} {...rest}>
    <slot />
</picture>

// Component CarouselButton
---
interface Props {
    idPtrevButton?:string;
    idNextButton?:string;
    class?: string;
    [x: string]: any;
}

const defaulClass='aspect-video w-1/2';
const { idPtrevButton, idNextButton, class: className = defaulClass, ...rest } = Astro.props;
---
<section class:list={[className, 'carousel']}>
    <picture class="slides-container ">
        <slot/>
    </picture>
    <slot name="button-move">
        <button id={idPtrevButton} class='default-button left-0 button-before'>&#8249;</button>
        <button id={idNextButton} class='default-button right-0 button-after'>&#8250;</button>
    </slot>
</section>
```