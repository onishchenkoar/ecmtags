# \<layout-info>

---

Specifies layout information for a DataGrid.

### Attributes:
* `page-size`(optional) &mdash; determines how many rows of data should be visible on one page. If omitted, the value of the metadata property `Table.Records.Per.Page` is used.
* `page-size-choices`(optional) &mdash; a list of page sizes that are listed in the footer of the DataGrid. When a value in this list is clicked, the page size of the DataGrid is changed to that value. This should be a list of whole numbers separated by commas (for example, “10, 25, 50, 100”). A value of all can be used for the last value instead of a number. This adds an item that displays all available data on one page. If this attribute is omitted, no page size choices are displayed.

[Back to index](./README.md)