Table profile_check
===========

DFRN remote auth use

Fields
------

| Field   | Description   | Type               | Null | Key | Default | Extra          |
| ------- | ------------- | ------------------ | ---- | --- | ------- | -------------- |
| id      | sequential ID | int unsigned       | NO   | PRI | NULL    | auto_increment |
| uid     | User id       | mediumint unsigned | NO   |     | 0       |                |
| cid     | contact.id    | int unsigned       | NO   |     | 0       |                |
| dfrn_id |               | varchar(255)       | NO   |     |         |                |
| sec     |               | varchar(255)       | NO   |     |         |                |
| expire  |               | int unsigned       | NO   |     | 0       |                |

Indexes
------------

| Name    | Fields |
| ------- | ------ |
| PRIMARY | id     |
| uid     | uid    |
| cid     | cid    |

Foreign Keys
------------

| Field | Target Table | Target Field |
|-------|--------------|--------------|
| uid | [user](help/database/db_user) | uid |
| cid | [contact](help/database/db_contact) | id |

Return to [database documentation](help/database)
