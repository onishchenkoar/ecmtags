# \<grid-action>

---

Defines a URL or javascript that will be executed.

### Attributes:
* `id`(required) &mdash; specifies the ID field. Each ID must be unique for the screen.
* `url`(optional) &mdash; if output-destination is not set to `javascript`, this specifies the URL that is called to execute the action. If output-destination is set to `javascript`, this is the JavaScript snippet to execute.
* `output-destination`(optional) &mdash; specifies the output format. The possible values are inline, window, new-window, javascript, or ignore. The default is window. A value of window specifies replacing the existing window's contents with the result page. A value of new-window specifies showing the result page in a pop-up window. A value of inline causes a refresh of the parent DataGrid when the action completes, but no other change in the structure of the current page. A value of `javascript` means that the `url` parameter should be treated as JavaScript to execute, instead of a URL to submit. A value of ignore specifies to submit the URL, but does not refresh the grid or any other part of the page.
* `render-type`(optional) &mdash; specifies how the action is rendered. The possible values are `always`, `select`, and `row`. A value of `always` renders the action as a button at the top of the table that is always enabled. A value of `select` renders the action as a button at the top of that table that is enabled only when at least one row is selected. A value of `row` renders the action as an icon in each row and is an action that is performed just for that row. The default is `always`.
* `request-type`(optional) &mdash; specifies whether the URL should be made using http post or http get. The values are `post` or `get`. The default is `post`.
* `visible`(optional) &mdash; specifies whether the action is visible. The default is `true`.
* `enabled`(optional) &mdash; specifies whether the action is enabled. The default is `true`.

### Child elements:
* A required [\<label>](./label.md) element that specifies the label on the button. 
* An optional [\<tool-tip>](./tool-tip.md) element that provides a tool tip for actions that are rendered as buttons. For [\<grid-action>](./grid-action.md) elements with render-type set to row, this parameter is ignored. 
* A required [\<url>](./url.md) element that specifies the action being called. 
* [\<eval>](./eval.md) &mdash; this element is a child of the [\<url>](./url.md) element. The text of this element is treated as an expression and evaluated. 
* An optional [\<image>](./image.md) element that defines the URL used to retrieve the image. This is needed when the value for render-type is `row`. 
* Zero or more [\<param>](./param.md) elements, which are used for [\<datagrid>](./datagrid.md) components. 
* An optional [\<validations>](./validations.md) element that contains any validations that must evaluate to true for the GridAction to execute. 
* An optional [\<callback>](./callback.md) element that defines an action that will be executed on completion of the original action call.

### Parent elements:
* [\<datagrid>](./datagrid.md)

[Back to index](./README.md)
