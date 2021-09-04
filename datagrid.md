# \<datagrid>

---

Describes a grid of tabular data.

### Attributes:
* `name`(required) &mdash; a unique name for the instance of [\<datagrid>](./datagrid.md).
* `selectedKeyField`(required for actions on row data) &mdash; name of the column or field in the grid’s data that represents the key field of the row. It is needed to pass a row’s unique identifier for actions that act upon selected rows.
* `columns`(optional) &mdash; used to provide a function that returns a list of DataGrid column entries to be shown in the [\<datagrid>](./datagrid.md) element instead of using [\<datagrid-column>](./datagrid-column.md) elements.
* `visible`(optional) &mdash; an expression that is evaluated by the expression handler to determine whether the field is visible. The default is true.
* `readonly`(optional) &mdash; an expression that is evaluated by the expression handler to determine whether the field is read-only. The default is false.
* `component-name`(optional) &mdash; the name of the component to use when adding a [\<datagrid>](./datagrid.md) element-based component.

### Child elements:
* An optional [\<label>](./label.md) element that specifies the label or description for this table. 
* An optional [\<help-text>](./help-text.md) section that is an alternative to specifying a Help URL attribute. 
* Zero or more [\<validation>](./validation.md) elements, which are evaluated when the Save button is clicked. 
* Either one of a [\<datastore>](./datastore.md) or [\<datastore-ref>](./datastore-ref.md) element. 
* An optional [\<layout-info>](./layout-info.md) element that specifies layout information for the grid. 
* Zero or more [\<datagrid-column>](./datagrid-column.md) elements that each define a single DataGrid column. 
* Zero or more [\<filter>](./filter.md) elements that define what subset of data the DataGrid should display. 
* Zero or more [\<grid-action>](./grid-action.md) elements that each define a single grid action. 
* Zero or more [\<param>](./param.md) elements, which are applicable only if type=“component”. 
* An optional [\<on-change>](./on-change.md) element, which describes any dynamic actions to be executed when table data changes. 
* An optional [\<on-select>](./on-select.md) element, which describes any dynamic actions to be executed when a row is selected in the data grid.

[Back to index](./README.md)