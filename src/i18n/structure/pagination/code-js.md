```js

<script is:inline define:vars={{currentPage, currentUrl, totalCount}}>

    const prevButton = document.getElementById('prev');
    const nextButton = document.getElementById('next');

    prevButton?.addEventListener('click', () => {
        let page = currentPage
        if(page > 1){
            page--;
            window.location.href = currentUrl + String(page)
        }
    });
    nextButton?.addEventListener('click', () => {
        let page = currentPage
        if(page < totalCount){
            page++;
            window.location.href = currentUrl + String(page)
        }
    });
</script>

```