```astro
//Component InputOtp
---
interface Props {
    class?: string;
    [x: string]: any;
}
const defaultClass='default';
const { class: className = defaultClass, ...rest } = Astro.props;
---
<input class:list={[className, 'input-select']} type="text" {...rest}/>

//Component InputOtpGroup
---
interface Props {
    count:number;
    class?: string;
    [x: string]: any;
}
const defaultClass='default border-y border-r';
const { count = 0, class: className = defaultClass, ...rest } = Astro.props;

let emptyArray = new Array(count);
for (let i = 0; i < count; i++) {
    emptyArray[i] = i;
}
---
<div class={'otp-container has-[:disabled]:opacity-50'}>
    {
        emptyArray.map(() =>
            <input class:list={[className, 'input-group first:rounded-l-md first:border-l last:rounded-r-md']} 
            type="text" {...rest}/>
        )
    }
</div>
```