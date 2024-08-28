```css

/* Component Drawer*/
<style>
    input{
        position: absolute;
        top: 0px;
        left: 0px;
        width: 100%;
        height: 100%;
        cursor: pointer;
        opacity: 0;
        z-index: 1;
    }
    div{
        position: relative;
    }
    .default{
        display: inline-block;
        padding: 0.5rem 0.25rem;
        background-color: rgb(163 163 163);
        border-radius: 0.5rem;
    }
    .default:hover{
        background-color: rgb(82 82 82)
    }
</style>
/* Component Drawer-Label */
<style>
    .default-background{
        position: fixed;
        width: 100%;
        height: 100%;
        background-color: rgb(0 0 0 / 0.5);
        z-index: 1;
        display: none;
        top: 0px;
        left: 0px;
    }
</style>

/*Component Drawer-Content */
<style>
    div{
        position: fixed;
        z-index: 99;
        transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
        transition-duration: 500ms;
    }
    .default{
        width: fit-content;
        height: 100%;
        left: 0px;
        top: 0px;
        background-color: black;
    }
</style>
```