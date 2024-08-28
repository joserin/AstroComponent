```css

<style>
    .container-hover{
        position: relative;
    }
    .default{
        font-size: 1rem;
        line-height: 1rem;
    }
    .hover-content{
        display: none;
    }
    .hover-element:hover + .hover-content{
        display: block;
        position: absolute;
    }
</style>
```