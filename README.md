A short reference for XML tags used in SAS Enterprise Case Management for interface design.

This is a reproduction of section *Valid XML Elements and Descriptions for User Interface Definitions* in chapter 6 of the [official administrator's guide PDF](https://support.sas.com/documentation/onlinedoc/ecm/6.3/casemgmtag.pdf).

---

# Index (alphabetically)

||||
|:---|:---|:---|
|[\<action>](./action.md)|[\<false-label>](./false-label.md)|[\<refresh>](./refresh.md)|
|[\<action-group>](./action-group.md)|[\<field>](./field.md)|[\<screen>](./screen.md)|
|[\<app-title>](./app-title.md)|[\<filter>](./filter.md)|[\<section>](./section.md)|
|[\<call>](./call.md)|[\<finalize>](./finalize.md)|[\<set>](./set.md)|
|[\<callback>](./callback.md)|[\<function>](./function.md)|[\<set-required>](./set-required.md)|
|[\<column>](./column.md)|[\<grid-action>](./grid-action.md)|[\<set-value>](./set-value.md)|
|[\<column-layout>](./column-layout.md)|[\<help-text>](./help-text.md)|[\<set-values>](./set-values.md)|
|[\<component>](./component.md)|[\<if>](./if.md)|[\<set-visible>](./set-visible.md)|
|[\<datagrid>](./datagrid.md)|[\<image>](./image.md)|[\<tab>](./tab.md)|
|[\<datagrid-column>](./datagrid-column.md)|[\<initialize>](./initialize.md)|[\<tab-section>](./tab-section.md)|
|[\<datagrid-column-sorter>](./datagrid-column-sorter.md)|[\<label>](./label.md)|[\<title>](./title.md)|
|[\<datagrid-renderer>](./datagrid-renderer.md)|[\<layout-info>](./layout-info.md)|[\<tool-tip>](./tool-tip.md)|
|[\<datagrid-renderer-ref>](./datagrid-renderer-ref.md)|[\<menu>](./menu.md)|[\<true-label>](./true-label.md)|
|[\<datastore>](./datastore.md)|[\<message>](./message.md)|[\<ui-definition>](./ui-definition.md)|
|[\<datastore-ref>](./datastore-ref.md)|[\<on-change>](./on-change.md)|[\<url>](./url.md)|
|[\<errmsg>](./errmsg.md)|[\<on-select>](./on-select.md)|[\<validation>](./validation.md)|
|[\<eval>](./eval.md)|[\<param>](./param.md)|[\<validations>](./validations.md)|


| Attribute Name                 | Attribute Definition                                                                                                                                                                                               | Column Name                    | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------------------|:-------------------|:---------------------|:---------------|:---------------|
| account_number                 | "Natural Key" from source system.  This may be concatenated e.g. division, branch, acct number..                                                                                                                   | account_number                 | VARCHAR2(50)       | Not Null             | Yes            | No             |
| segment_id                     | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                                             | segment_id                     | VARCHAR2(128)      | Not Null             | Yes            | No             |
| expected_incoming_amount       | Currency amount of credits expected to the account during the period (e.g. monthly).                                                                                                                               | expected_incoming_amount       | NUMBER(18,5)       | Null                 | No             | No             |
| expected_outgoing_amount       | Currency amount of debits expected to the account during the period (e.g. monthly).                                                                                                                                | expected_outgoing_amount       | NUMBER(18,5)       | Null                 | No             | No             |
| expected_incoming_count        | Number of credits expected to the account during the period (e.g. monthly).                                                                                                                                        | expected_incoming_count        | NUMBER(10)         | Null                 | No             | No             |
| expected_outgoing_count        | Number of debits expected to the account during the period (e.g. monthly).                                                                                                                                         | expected_outgoing_count        | NUMBER(10)         | Null                 | No             | No             |
| increased_behavior_credit_amt  | A threshold amount above which the behavior of the account is determined to have increased. See scenario SAS10088.                                                                                                 | increased_behavior_credit_amt  | NUMBER(18,5)       | Null                 | No             | No             |
| increased_behavior_debit_amt   | A threshold amount above which the behavior of the account is determined to have increased. See scenario SAS10088.                                                                                                 | increased_behavior_debit_amt   | NUMBER(18,5)       | Null                 | No             | No             |
| increased_behavior_credit_cnt  | A threshold transaction count above which the behavior of the account is determined to have increased. See scenario SAS10088.                                                                                      | increased_behavior_credit_cnt  | NUMBER(15,5)       | Null                 | No             | No             |
| increased_behavior_debit_cnt   | A threshold transaction count above which the behavior of the account is determined to have increased. See scenario SAS10088.                                                                                      | increased_behavior_debit_cnt   | NUMBER(15,5)       | Null                 | No             | No             |
| expected_credit_ceiling_amount | An expected total amount of credits to an account in a given period.  This is determined using the Largest Credit Amount field in the Account Profile.  Used in scenario SAS10091.                                 | expected_credit_ceiling_amount | NUMBER(18,5)       | Null                 | No             | No             |
| expected_debit_ceiling_amount  | An expected total amount of debits to an account in a given period.  This is determined using the Largest Debit Amount field in the Account Profile.  Used in scenario SAS10091.                                   | expected_debit_ceiling_amount  | NUMBER(18,5)       | Null                 | No             | No             |
| last_activity_date             | Date the account last had activity.  Client determines if non-financial transactions should be included (e.g. inquiries), or whether bank-initiated transactions are included, and how often to update this field. | last_activity_date             | DATE               | Null                 | No             | No             |
