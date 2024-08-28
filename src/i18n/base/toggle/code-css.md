```css

<style>
    .switch-container{
        position: relative;
        display: inline-flex;
        align-items: center;
        cursor: pointer;
    }
    div{
        position: relative;
        background-color: darkgray;
        border-radius: 9999px;
    }
    input{
        position: absolute;
        width: 100%;
        cursor: pointer;
        opacity: 0;
        overflow: hidden;
        clip: rect(0, 0, 0, 0);
        white-space: nowrap;
        border-width: 0;
    }
    .slider::after{
        content: '';
        position: absolute;
        top: 2px;
        inset-inline-start: 2px;
        border-radius: 9999px;
        transition-property: all;
        transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
        transition-duration: 150ms;
    }
    .default{
        width: 3rem;
        height: 1.5rem;
    }
    .default::after{
        width: 1.25rem;
        height: 1.25rem;
    }
</style>
```