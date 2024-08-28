```astro 
---
interface Props {
  values?:string[];
  title?: string;
  class?: string;
  [x: string]: any;
}
const defaulClass='focus:ring-blue-500 default';
const { title = 'Select', values = [], class: className= defaulClass, ...rest } = Astro.props;
---

<select {...rest} class={className}>
  <slot>
    {
      values.length > 0 &&  <option disabled selected>{title}</option>
    }
    {
      values?.map((element) =>
        <option value={element.toLowerCase()}>{element}</option>
      )
    }
  </slot>
</select>
```