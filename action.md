# \<action>

---

The [\<action>](./action.md) element enables you to provide links and buttons on a screen.

### Attributes:

* `URL`&mdash; specifies the landing URL after a submit.

  - [\<eval>](./eval.md) &mdash; this element is a child of the URL attribute. The text of this element is treated as an expression and evaluated.

* `id`(optional) &mdash; specifies the ID field.

* `output‑destination`(optional) &mdash; specifies the output format, either window or inline. The default is window. A value of window specifies showing the result page in a pop-up window. A value of inline specifies no change in the structure of the current page, and no pop-up window. The output‑destination could be a field replacement javascript call. The value ignore specifies a server side trigger, with no UI change.

* `sas‑sso`(optional) &mdash; this is a Boolean field that decides whether to do a SAS single sign-on automatically. The default is false.

* `trigger`(optional) &mdash; specifies when the action should execute. If omitted, the action is rendered as a button and is executed whenever the button is clicked. If specified, the only valid value for this attribute is save. When save is specified, this action is not manifested as a button in the UI, but rather it is automatically executed whenever an entity is successfully saved.

* `fail‑on‑error failed`(optional) &mdash; specifies the Boolean field that enables you to decide whether to continue running other trigger actions if there is an error in the action execution.

* `visible`(optional) &mdash; specifies whether the action is visible.

* `enabled`(optional) &mdash; specifies whether the action is enabled.

* `content‑type`(optional) &mdash; specifies the response content type for a backend action. This attribute currently supports text and HTML.

### Child elements:
* An optional [\<label>](./label.md) element. This element provides the window label or title.
* An optional [\<param>](./param.md) element. This element provides parameters for the URL.
* An optional [\<url>](./url.md) element. This element is used if an attribute URL is not specified. It provides a more convenient way to specify a URL.