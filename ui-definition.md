# \<ui-definition>

---

The top-level element that describes the screens in the UI definition.

### Attributes:
* `id`&mdash; a unique identifier for this user interface definition (userdefined). This must be a valid XML name.
* `type`&mdash; indicates the type of object that this UI definition is used for. Valid values include `case`, `incident`, `party`, `report`, `efile`, `financialItem`, and `viewer`.

### Child elements:
* An optional [\<title>](./title.md) element. The title appears on the administration page, but it is not visible to the end user (for example, the user who is editing an issue). 
* Zero or more [\<function>](./function.md), [\<datagrid-renderer>](./datagrid-renderer.md), or [\<component>](./component.md) elements. 
* Zero or more [\<screen>](./screen.md) elements.

[Back to index](./README.md)