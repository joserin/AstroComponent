```js

//Component Resizable Panel
<script>
    function makeResizable(selector: string) {
        document.querySelectorAll(selector).forEach(function (element) {
            const resizer = element.querySelector(".resizable__control") as HTMLElement;
            const minimum_size = 20;
            let original_width = 0;
            let original_height = 0;
            let original_x = 0;
            let original_mouse_x = 0;
            resizer?.addEventListener("mousedown", function (e:Event) {
                e.preventDefault();
                original_width = parseFloat(getComputedStyle(element, null).getPropertyValue("width").replace("px", "") );
                original_height = parseFloat(getComputedStyle(element, null).getPropertyValue("height").replace("px", ""));
                original_x = element.getBoundingClientRect().left;
                window.addEventListener("mousemove", resize);
                window.addEventListener("mouseup", stopResize);
            });

            function resize(e: any) {
                if (resizer?.classList.contains("resizable__control")) {
                    const width = original_width + (e.pageX - original_mouse_x);
                    if (width > minimum_size) {
                        (element as HTMLElement).style.width = width + "px";
                    }
                }
            }
            function stopResize() {
                window.removeEventListener("mousemove", resize);
            }
        });
    }
    makeResizable(".elemento");
</script>
```