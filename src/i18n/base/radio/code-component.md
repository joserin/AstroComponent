```astro
---
interface Props {
    elements:string[];
    identify?: number;
    class?: string;
    [x: string]: any;
}
const defaulClass='radio-group';
const { identify = 0, elements, body, class: className = defaulClass, ...rest } = Astro.props;
---
<ul class:list={[className]}>
    {
        elements.map((element, index) =>
            <li>
                <input {...rest} type="radio" id={element + index + identify} value={element}/> 
                <label for={element + index + identify}>
                    {element}
                </label>
            </li>
        )
    }
</ul>
```