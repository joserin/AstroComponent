```astro live
---
interface Props {
  title?: string;
  class?: string;
  [x: string]: any;
}
 
const defaulClass='default';
const { title, class: className= defaulClass, ...rest } = Astro.props;
---

<main class:list={[className, 'accordion-content']}>
    <input class="peer input-style" type="radio" {...rest}/>
    <slot> {title}</slot>
    <div class='peer-checked:max-h-fit peer-checked:mt-5 element-container'>
      <slot name="content"/>
    </div>
</main>
```