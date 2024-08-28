```astro
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass="default peer-checked:bg-blue-600 after:bg-white peer-checked:after:bg-blue-300";
const {  class: className = defaulClass, ...rest } = Astro.props;
---

<label class="switch-container">
    <input type="checkbox" class="peer" {...rest}>
    <div class:list={[className, 'slider peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full']}></div>
</label>
```