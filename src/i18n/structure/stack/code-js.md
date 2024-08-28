```js

<script>
    const elements = document.querySelectorAll('.stack > *');
    if( elements){
        const distance = 10;
        for(let i=0; i < elements.length; i++){
            const element = elements[i] as HTMLElement;
            element.style.position = 'absolute';
            element.style.top = (distance*i).toString()+'px';
        }
    }
</script>
```