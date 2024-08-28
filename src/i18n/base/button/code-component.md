```astro
---
interface Props {
  class?: string;
  [x: string]: any;
}
const defaultClass="default transition focus-visible:ring-2 ring-offset-2 ring-gray-200";
const { class: className = defaultClass, ...rest } = Astro.props;
---
<button {...rest} class={className}>
  <slot/>
</button>
```