```astro 

//Component Timeline
---
interface Props {
    class?: string;
    [x: string]: any;
}
const { class: className, ...rest } = Astro.props;
---

<ol class={className} {...rest}>
    <slot/>
</ol>

//Component Line Element
---
interface Props {
    class?: string;
    [x: string]: any;
}
const { class: className, ...rest } = Astro.props;
---
<li class={className} {...rest}>
    <slot/>
</li>

//Component Line Content
---
interface Props {
    class?: string;
    endLine?:boolean;
    [x: string]: any;
}
const defaulClass="default horizontal";
const { endLine = false , class: className = defaulClass, ...rest } = Astro.props;
---
<span>
    <slot/>
    { 
        !endLine && <div class={className} {...rest}></div>
    }
</span>
```