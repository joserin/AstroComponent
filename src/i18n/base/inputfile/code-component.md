```astro
---
interface Props {
    title?: string;
    class?: string;
    nameLabel:string;
    [x: string]: any;
}
const defaultClass='default';
const { title, nameLabel, class: className = defaultClass, ...rest } = Astro.props;
---
<label for={nameLabel}>
    <slot> {title} </slot>
</label>
<input class={className} {...rest} type="file" id={nameLabel}/>
```