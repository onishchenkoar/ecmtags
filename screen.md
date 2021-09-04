# \<screen>

---

Describes the appearance and behavior of a single screen.

### Attributes:
* `id`&mdash; the screen ID. This must be unique for each screen. For each entity, the following specific IDs are required in the UI definition:   
  - \<screen id="case">   
  - \<screen id="incident">   
  - \<screen id="party">   
  - \<screen id="report">   
  - \<screen id="efile">   
  - \<screen id="financialItems">
* `help`(optional) &mdash; a URL specifying the Help location for this screen.

### Child elements:
* An optional [\<app-title>](./app-title.md) element providing the application title for a screen. 
* An optional [\<title>](./title.md) element providing the screen title. 
* An optional [\<menu>](./menu.md) element. 
* An optional [\<help-text>](./help-text.md) element that provides an alternative means of specifying Help instead of using a URL in the help attribute. 
* An optional [\<initialize>](./initialize.md) section that describes any initialization that must be performed before the screen is rendered. 
* Any number of [\<action-group>](./action-group.md), [\<field>](./field.md), [\<datagrid>](./datagrid.md), [\<datastore>](./datastore.md), [\<section>](./section.md), [\<tab-section>](./tab-section.md), [\<column-layout>](./column-layout.md), or [\<if>](./if.md) elements. 
* An optional [\<finalize>](./finalize.md) section that describes any validations or computations that must be performed when the user clicks Save.

[Back to index](./README.md)