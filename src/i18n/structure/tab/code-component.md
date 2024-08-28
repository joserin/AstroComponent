```astro 

// Component Tab
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass='default';
const { header, body, class: className = defaulClass, ...rest } = Astro.props;
---

<div class:list={[className ,"element-tab"]}>
    <slot/>
</div>

// Component Tab Head
---
interface Props {
    class?: string;
    [x: string]: any;
}

const defaulClass='default';
const { class: className = defaulClass, ...rest } = Astro.props;
---

<button {...rest} class:list={[className, 'show-select']}>
    <slot/>
</button>


// Component Tab Content
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaulClass='deactive';
const { title, class: className = defaulClass, ...rest } = Astro.props;
---
<div {...rest} class:list={[className, 'tab-select']}>
    <slot/>
</div>
```