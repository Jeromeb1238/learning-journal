## Tables

- Table elements
```html
<table> table headers and table rows go inbetween here </table?
<tr> equals for table row
<td> equals table data

structure looks like this:
<table>
  <tr>
    <td> 'data' </td>
    <td> 'data' </td>
  </tr>
</table>
  
  Table headers look like this
  
  <table>
    <tr>
      <th></th>   Leave text empty between tags to leave an empty cell
      <th scope="col">column name</th>
      <th scope="col">column name</th>
    </tr>
    <tr>
      <th scope="row">row name</th>
      <th scope="row">row name</th>
    </tr>
  </table>
  
  <td colspan="# columns to span">row information</td> to have a single row span multiple columns
  <td rowspan="# rows to span">column information</td> to have a single column span multiple rows
  
  <thead>  </thead>  for table headers
  <tbody>   </tbody>  for table body data
  <tfoot>   </tfoot>  for table footer/total rows
  ```
