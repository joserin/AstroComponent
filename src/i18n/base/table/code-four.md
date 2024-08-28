```astro

import Table from './Table.astro';
import TableHeader from './TableHeader.astro';
import TableRow from './TableRow.astro';
import TableColumn from './TableColumn.astro';

<Table class='text-center w-96'>
    <TableHeader slot="thead" class='bg-white text-black' head={headFour}/>
    <tbody>
        {
            elements.map( (element: any, index) => {
                const isEven = index % 2 === 0;
                return(
                    <tr class={isEven ? 'bg-sky-700' : 'bg-sky-950'}>
                        <td>
                            <input type="checkbox" name={index.toString()} aria-label="input-table"/>
                        </td>
                        <TableColumn column={element}/>
                        <td>
                            <Button class='bg-red-700 px-2 py-1 hover:bg-red-500 text-sm rounded-full'>Details</Button>
                        </td>
                    </tr>
                )
            })
        }
    </tbody>
    <TableFooter slot="tfooter" class='bg-black text-white' footer={headFour}/>
</Table>
```