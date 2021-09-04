# \<datagrid-column>

---

Provides a single column entry to a DataGrid.

### Attributes:
* `name`(required) &mdash; the name of the field to be used for the column in each row.
* `id`(optional) &mdash; if the ID is specified, then the ID is used for the [\<datagrid-column>](./datagrid-column.md) element. Otherwise, the name attribute is used. If a DataGrid has two columns displaying the same field, but using different renderers, unique values for the `id` attribute should be given to each [\<datagrid-column>](./datagrid-column.md) element. This allows the columns to be distinguishable from one another and rendered properly.
* `default-width`(optional) &mdash; the amount of space to give to this column in the DataGrid, if you have not yet customized the grid columns. This attribute should be a percentage between 1 and 100, in the format "57%". You must specify this attribute for either all [\<datagrid-column>](./datagrid-column.md) elements in a DataGrid, or none. When this attribute is specified, all columns must have their values for this attribute sum to 100%. If this attribute is omitted for the columns in a DataGrid, its columns will be given equal widths.

### Child elements:
* A required [\<label>](./label.md) element that specifies the header for this column. 
* An optional [\<datagrid-renderer-ref>](./datagrid-renderer-ref.md) element that defines how to format the column data. 
* An optional [\<datagrid-column-sorter>](./datagrid-column-sorter.md) element that defines how the column should be sorted.

[Back to index](./README.md)