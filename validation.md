# \<validation>

---

A test that is performed at the screen, section, or field level. The test is evaluated by the expression handler (usually, when the user clicks Save). If it is false, the error message is displayed and the user remains on the same screen.

### Attributes:
* `test`&mdash; an expression that is evaluated by the expression handler using the current contents of the memory hash table (which will include the values from the database and everything the user has entered up to this point). For example, if the input field was a month number in a field named MONTH, the expression might be `test="month ge 1 and month le 12"`.

### Child elements:
* An [\<errmsg>](./errmsg.md) element that describes the message to display if the test fails.

[Back to index](./README.md)