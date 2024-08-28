```js

<script>
  const containers = document.querySelectorAll('.container');

  if(containers){
    containers.forEach(container => {
      const slider = container.querySelector('.slider');

      if (slider) {
        slider.addEventListener('input', (event) => {
          (container as HTMLElement).style.setProperty('--position', {(event.target as HTMLInputElement).value}%);
        });
      }
    });
  }
</script>
```