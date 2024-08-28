```astro
---
interface Props {
    count: number;
    identify?: string;
    name: string;
    class?: string;
    [x: string]: any;
    selectColor?:string;
}

const defaulClass='flex';
const { selectColor = "rgb(255 255 0)", name, count, identify = 'one', class: className= defaulClass, ...rest} = Astro.props;
let emptyArray = new Array(count);

for (let i = 0; i < count; i++) {
    emptyArray[i] = i;
}
---
<div class:list={["rating", defaulClass]}>
    {
        emptyArray.map((index) =>
            <input type="checkbox" id={identify + index} class="mask" name={name} value={index}/>
            <label for={identify + index}>
                <slot/>
            </label>
        )
    }
</div>
```