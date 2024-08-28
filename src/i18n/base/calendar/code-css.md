```css

<style>
    .days, .dates {
        display: grid;
        grid-template-columns: repeat(7, 32px);
        gap: 10px;
        margin-block: 10px;
    }
    header{
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
    }
    .default{
        background-color: white;
        padding: 0.5rem;
        border: 1px solid black;
        color: black;
    }
    .today{
        background-color: aqua;
    }
</style>
```