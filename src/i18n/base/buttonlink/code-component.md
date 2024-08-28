```astro
---
interface Props {
  class?: string;
  [x: string]: any;
}

const defaulClass='default transition focus-visible:ring-2 ring-offset-2 ring-gray-200';
const { class: className= defaulClass, ...rest } = Astro.props;
---

<a {...rest} class={className}>
  <slot/>
</a>
```