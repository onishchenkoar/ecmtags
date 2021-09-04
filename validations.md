# \<validations>

---

An optional section that contains code that is executed before a GridAction executes.

### Child elements:
* Zero or more [\<set>](./set.md) elements that set variables to some computed value. 
* Zero or more [\<validation>](./validation.md) elements that are checked when the user attempts to execute the GridAction. If any of these validations do not evaluate to true, the appropriate error message is displayed and the GridAction is not executed.

[Back to index](./README.md)