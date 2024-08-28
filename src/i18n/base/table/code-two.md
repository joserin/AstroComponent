```astro

import Table from './Table.astro';
import TableHeader from './TableHeader.astro';
import TableRow from './TableRow.astro';
import TableColumn from './TableColumn.astro';

<Table class='text-center w-96'>
    <TableHeader slot="thead" class='bg-gray-700' head={headTwo}/>
    <tbody>
        {
            elements.map( (element: any, index) => 
                <TableRow count={index}>
                    <TableColumn column={element}/>
                </TableRow>
            )
        }
    </tbody>
</Table>
```