```astro live
---
interface Props {
  class?: string;
  [x: string]: any;
}

const defaulClass='default transition focus-visible:ring-2 ring-offset-2 ring-gray-200';
const { class: className = defaulClass, ...rest } = Astro.props;
---

<div {...rest}  class:list={['default-card',className]}>
  <slot name="header"/>
  <slot/>
  <slot name="footer"/>
</div>
```