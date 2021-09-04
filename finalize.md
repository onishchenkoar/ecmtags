# \<finalize>

---

An optional section that contains code that is executed when the screen is considered complete (usually when the user clicks Save).

### Child elements:
* Zero or more [\<set>](./set.md) elements that compute derived fields. These fields are evaluated when the user clicks Save. 
* Zero or more [\<if>](./if.md) elements that contain conditional [\<set>](./set.md) or [\<validation>](./validation.md) elements. 
* Zero or more screen-level [\<validation>](./validation.md) elements that are checked when the user clicks Save.

[Back to index](./README.md)