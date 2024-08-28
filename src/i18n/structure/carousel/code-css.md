```css

/*Component Carousel*/
<style>
    picture{
        position: relative;
        overflow: scroll;
    }
    .default{
        display: flex;
        scroll-snap-type: mandatory;
    }
    .default::-webkit-scrollbar { 
        display: none; 
    } 
</style>

/* Component CarouselButton*/
<style>
    section{
        display: flex;
        position: relative;
        overflow: hidden;
    }
    picture{
        display: flex;
        flex-direction: row;
        position: relative;
        overflow: scroll;
        scroll-behavior: smooth;
        width: 100%;
    }
    .slides-container::-webkit-scrollbar { 
        display: none; 
    }
    .default-button{
        position: absolute;
        top: 0px;
        bottom: 0px;
        margin: auto;
        background-color: rgb(68, 68, 68);
        width: 1.25rem;
        font-size: 1.25rem;
        line-height: 1.75rem;
        cursor: pointer;
        opacity: 0.5;
        transition-property: opacity;
        transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
        transition-duration: 150ms;
    }
    .default:hover{
        opacity: 0.7;
    }
    .default:focus{
        opacity: 0.9;
    }
</style>
```