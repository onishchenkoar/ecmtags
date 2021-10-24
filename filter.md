# \<filter>

---

Adds a filter expression that is run for each possible record in a DataGrid. Each [\<filter>](./filter.md) expression must evaluate to true for that record to be displayed in the grid. This filter typically checks the value of one or more fields in the row of the grid against an expected value.

### Attributes:
* `name`(optional) &mdash; the name of this filter.
* `value`&mdash; the expression that must evaluate to true for a row to be displayed.

### Parent elements:
* [\<datagrid>](./datagrid.md)

[Back to index](./README.md)