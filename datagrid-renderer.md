# \<datagrid-renderer>

---

Defines a custom renderer for the [\<datagrid-column>](./datagrid-column.md) element.

### Attributes:
* `id`(required) &mdash; a logical identifier that [\<datagrid-column>](./datagrid-column.md) elements can reference this renderer with. This must begin with "C_" (or "c_").

### Child elements:
* A JavaScript function to use for rendering DataGrid cells. This should be wrapped in a CDATA block. The [\<message>](./message.md) and [\<eval>](./eval.md) elements are permitted.

### Parent elements:
* [\<ui-definition>](./ui-definition.md)

[Back to index](./README.md)