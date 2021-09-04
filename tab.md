# \<tab>

---

A tab is nested under a [\<tab-section>](./tab-section.md) and defines a tab page.

### Attributes:
* `id`&mdash; the section ID. This must be a valid XML name (also a valid SAS name).
* `required`(optional) &mdash; an expression that is evaluated by the expression handler to determine whether the tab should display the required indicator. Default is `false`.

### Child elements:
* An optional [\<label>](./label.md) element providing the tab label and title. 
* An optional [\<initialize>](./initialize.md) element containing one or more child [\<set>](./set.md) elements. 
* Zero or more [\<field>](./field.md) elements. 
* Zero or more [\<section>](./section.md) elements. 
* Zero or more [\<if>](./if.md) elements. 
* Zero or more [\<validation>](./validation.md) elements, which are evaluated when the user clicks Save. 
* Zero or more [\<action-group>](./action-group.md) elements.

[Back to index](./README.md)