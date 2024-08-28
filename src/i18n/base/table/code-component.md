```astro

//Component Table
---
interface Props {
    class?: string;
    [x: string]: any;
}

const defaulClass='default';
const { class: className = defaulClass, ...rest } = Astro.props;
---

<table class={className} {...rest}>
    <thead>
        <slot name="thead"/>
    </thead>
    <slot/>
    <tfoot>
        <slot name="tfooter"/>
    </tfoot>
</table>

//Component Table Header
---
interface Props {
    head: any[];
    class?: string;
    [x: string]: any;
}

const defaulClass='default';
const { head, class: className = defaulClass, ...rest } = Astro.props;
---

<tr class={className} {...rest}>
    {
        head.map( (title: any) => <th>{title}</th>)
    }
</tr>

//Component Table Row
---
interface Props {
    count?:number;
    class?: string;
    [x: string]: any;
}
const defaulClass='default';
const { count = -1, class: className = defaulClass, ...rest } = Astro.props;
---

<tr class={className} {...rest}>
    {count > -1  && <th>{count}</th>}
    <slot/>
</tr>

//Component Table Column
---
interface Props {
    column?: any[];
    class?: string;
    [x: string]: any;
}
const { column=[], class: className, ...rest } = Astro.props;
---
{
    column.map( (element: any) => 
        <td class={className} {...rest}>
            {element}
        </td>
    )
}
    
//Component Table Footer
---
interface Props {
    footer: any[];
    class?: string;
    [x: string]: any;
}
const defaulClass='border-0';
const { footer, class: className = defaulClass, ...rest } = Astro.props;
---
<tr class={className} {...rest}>
    {
        footer.map( (title: any) => <th>{title}</th>)
    }
</tr>
```