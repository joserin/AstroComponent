```css

/* Component Resizable*/
<style>
    .default {
        min-height: 10rem;
        min-width: 10rem;
        background: #333;
        border: 3px solid #666;
        display: flex;
    }
</style>

/* Component Resizable Panel*/
<style>
    .elemento {
        position: relative;
        width: 100%;
    }

    .side {
        position: absolute;
        right: 0;
        top: 0;
        bottom: 0;
        width: 0.4rem;
        display: flex;
        cursor: col-resize;
        background-color: white;
    }
    .bottom {
        position: absolute;
        bottom: 0;
        height: 0.4rem;
        cursor: col-resize;
        background-color: white;
    }
</style>
```