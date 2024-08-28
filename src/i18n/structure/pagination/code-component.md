```astro live
---
interface Props {
    totalCount: number;
    currentUrl: string;
    currentPage: number;
    class?: string;
    [x: string]: any;
}

const defaultClass='flex gap-2 justify-center items-center';
const { currentUrl, class: className = defaultClass, totalCount, currentPage, ...rest} = Astro.props;
const pageAry = Array.from({ length: totalCount }, (_, i) => i + 1).filter((item) => item > currentPage - 3 && item < currentPage + 4,);
---

<nav {...rest} class:list={[className]}>
    {
        (currentPage > 1) && (
            <button id="prev">Prev</button>
        )
    }
    {
        totalCount > 1 && pageAry.map((i) => {
            let targetUrl = currentUrl;

            if(i > 1){
                targetUrl = currentUrl + (i.toString());
            }
            return (
                (i ===  currentPage )? (
                    <span class:list={['bg-blue-600 text-neutral-5 hover:text-neutral-50 button-page-style']}  aria-current="page">
                        {i}
                    </span>
                ) : (
                    <a href={targetUrl} class="button-page-style"> {i} </a>
                )
            );
        })
    }
    {
        (currentPage < 10) && (
            <button id="next">next</button>
        )
      }
</nav>

```