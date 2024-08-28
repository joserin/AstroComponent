```astro 
---
interface Props {
    daysInfo?:string[];
    monthsInfo?:string[];
    class?: string;
    [x: string]: any;
}
const defaultClass='default';
const daysDefault = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"];
const monthDefault = ["January", "February", "March", "April", "May", "June",
    "July", "August", "September", "October", "November", "December"];

const { class: className = defaultClass, daysInfo = daysDefault, monthsInfo = monthDefault,  ...rest } = Astro.props;
const  todayDate = new Date();
const  year = todayDate.getFullYear();
const  month = todayDate.getMonth();
---

<div class:list={["calendar default", className]}>
    <header>
        <button class='prev cursor-pointer p-1'>
            <slot name="beforeButton">
                <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" 
                    stroke-width="1.5" stroke="#000000" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M13 12h-10" />
                    <path d="M6 15l-3 -3l3 -3" />
                    <path d="M17 12a2 2 0 1 1 4 0a2 2 0 0 1 -4 0z" />
                </svg>
            </slot>
        </button>
        <div>
            <select class="month-input">
                {
                    monthsInfo.map((mes, index) => (
                        <option value={index} selected={index === month}>
                            {mes}
                        </option>
                    ))
                }
            </select>
            <input type="number" class="year-input w-20 text-center" min="0" value={year}/>
        </div>
        <button class="next cursor-pointer p-1">
            <slot name="AfterButton">
                <svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 24 24" 
                    stroke-width="1.5" stroke="#000000" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M11 12h10" />
                    <path d="M18 9l3 3l-3 3" />
                    <path d="M7 12a2 2 0 1 1 -4 0a2 2 0 0 1 4 0z" />
                </svg>
            </slot>
        </button>
    </header>
    <div>
        <section>
            <ul class="days flex flex-row justify-center">
                {
                    daysInfo.map(day => <span>{day}</span>)
                }
            </ul>
            <ul class="dates flex flex-row justify-center"></ul>
        </section>
    </div>
</div>

```