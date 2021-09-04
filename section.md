# \<section>

---

Describes the appearance and behavior of a section of other elements.

### Attributes:
* `id`&mdash; the section ID. This must be a valid XML name (also a valid SAS name).
* `required`(optional) &mdash; an expression that is evaluated by the expression handler to determine whether the section should display the required indicator. Default is `false`.
* `visible`(optional) &mdash; an expression that is evaluated by the expression handler to determine whether the section is visible. Default is `true`.
* `expanded`(optional) &mdash; an expression that is evaluated by the expression handler to determine whether the section is expanded by default. Default is `true`.

### Child elements:
* An optional [\<label>](./label.md) element providing the section label and title. 
* Zero or more [\<field>](./field.md) elements. 
* Zero or more [\<section>](./section.md) elements. 
* Zero or more [\<if>](./if.md) elements. 
* Zero or more [\<validation>](./validation.md) elements, which are evaluated when the user clicks Save. 
* Zero or more [\<action-group>](./action-group.md) elements.

[Back to index](./README.md)