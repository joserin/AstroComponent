```astro

import Table from './Table.astro';
import TableHeader from './TableHeader.astro';
import TableRow from './TableRow.astro';
import TableColumn from './TableColumn.astro';

<Table class='text-center w-96'>
    <TableHeader slot="thead" class='bg-orange-700' head={headThree}/>
    <tbody>
        {
            elements.map( (element: any, index) => 
                <TableRow count={index} class=' hover:bg-orange-500'>
                    <TableColumn column={element}/>
                </TableRow>
            )
        }
    </tbody>
</Table>
```