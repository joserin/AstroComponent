```css

<style define:vars={{ selectColor }}>

    .rating input[type="checkbox"] {
        display: none;
    }

    .rating label {
    display: inline-block;
    width: 20px;
    height: 20px;
    color: rgb(135, 148, 148);
    cursor: pointer;
    }

    .rating input[type="checkbox"]:checked + label {
        color: var(--selectColor);
    }

    .rating input[type="checkbox"]:checked{
        color: rgb(135, 148, 148);    
    }
</style>
```