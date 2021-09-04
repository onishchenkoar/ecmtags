# \<field>

---

Describes a prompt for user input.

### Attributes:
* `name`&mdash; the name of the field. This should be one of the names associated with the type of user interface definition that you are editing.
* `type`&mdash; the GUI component that is used for the input control. The following are valid values:   
  - string   
  - number   
  - boolean   
  - dropdown   
  - checkbox   
  - radio   
  - date   
  - textarea   
  - readonly   
  - component
* `component-name`(optional) &mdash; the name of a fixed screen component. Applicable only if `type=“component”`. Ignored otherwise.
* `length`(optional) &mdash; the width of the input control on the screen (not necessarily the field length in the database).
* `rows`(optional) &mdash; applies to text area type only. Indicates the number of rows in the text area.
* `max-length`(optional) &mdash; the maximum length of the input content allowed in the text input.
* `decimal-digits`(optional) &mdash; limits the number of digits in number format.
* `min`(optional) &mdash; minimum value for dates and numbers.
* `max`(optional) &mdash; maximum value for dates and numbers.
* `minSelectableDate`(optional) &mdash; minimum selectable date.
* `maxSelectableDate`(optional) &mdash; maximum selectable date.
* `default`(optional) &mdash; an expression whose value is used as the default value for the field. This value is used only when creating a new object.
* `values`(optional) &mdash; an expression whose value is a list of items used to populate a drop-down list, check box, or radio button group. Each item in the list is a label and value pair, where label is the displayed value, and value is the internally used value. Using the values attribute with a check box displays a group of check boxes to be multi-selected.[\<br>](./br.md) __Note__: Although multiple values for a string, number, Boolean, or text area type field are permissible, a result will not be set if used, since these field types can handle only a single value.
* `align`(optional) &mdash; the alignment of the input field’s label. Valid values are `top`, `left`, and `inline`. The default is `left`.
* `required`(optional) &mdash; an expression that is evaluated by the expression handler to determine whether the user must complete the field before saving. Default is `false`.
* `visible`(optional) &mdash; an expression that is evaluated by the expression handler to determine whether the field is visible. Default is `true`.
* `readonly`(optional) &mdash; an expression that is evaluated by the expression handler to determine whether the field is Read-Only. Default is `false`.
* `escape-xml`(optional) &mdash; by default, any XML character in a Read-Only field is escaped. Specifying false keeps the characters from being escaped. Default is `true`. Valid only for Read-Only fields.
* `label-width`(optional) &mdash; applies a width to the HTML element that holds a field's label. It is useful to line up fields and their labels when they are inside a column. An example is label-width="’25%’".

### Child elements:
* A [\<label>](./label.md) element that specifies the label and prompt for this input field. 
* Zero or more [\<validation>](./validation.md) elements, which are evaluated when the user clicks Save. 
* Zero or more [\<param>](./param.md) elements, which are applicable only if `type=“component”`. 
* An optional [\<on-change>](./on-change.md) element, which describes any dynamic actions to be executed when the field value changes. 
* An optional [\<true-label>](./true-label.md) element, which is applicable only if `type=“boolean”`. 
* An optional [\<false-label>](./false-label.md) element, which is applicable only if `type=“boolean”`.

[Back to index](./README.md)