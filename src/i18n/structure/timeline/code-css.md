```css

/* Component Timeline*/
<style>
    ol{
        display: flex;
    }
</style>

/* Component Line Element*/
<style>
    li{
        position: relative;
    }
</style>

/* Component Line Content*/
<style>
    span{
        display: flex;
        align-items: center;
    }
    .default{
        background-color: white;
        display: none;
    }
    .horizontal{
        width: 100%;
        height: 0.125rem;
    }
    .vertical{
        height: 100%;
        width: 0.125rem;
    }
    @media (min-width: 640px) {
        .default {
            display: flex;
        }
    }
    @media (prefers-color-scheme: dark) {
        .default {
            background-color: black;
        }
    }
</style>
```