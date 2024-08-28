```astro 
---
interface Props {
    start:number;
    end:number;
    step?:number;
    time?:number;
    class?: string;
    [x: string]: any;
}

const defaulClass='default';
const { start, end, step = 0, time=1000, class: className= defaulClass, ...rest } = Astro.props;
---

<div class:list={[className, "count"]}>
    <div class="countdown" {...rest} data-start={start} data-end={end} data-step={step} data-time={time}>{start}</div>
    <slot/>
</div>
```