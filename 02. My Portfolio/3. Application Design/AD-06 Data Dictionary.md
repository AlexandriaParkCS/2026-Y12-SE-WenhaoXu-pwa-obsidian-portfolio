***User***

| Attribute | Data Type | Bytes | Description                                                             | Example             |
| --------- | --------- | ----- | ----------------------------------------------------------------------- | ------------------- |
| name      | String    | 256   | A free text name (actual name, initials, user selected username, etc.). | johnd, John Doe     |
| email     | String    | 64    | A valid email address.                                                  | john@abc.com        |
| pwd_hash  | String    | 128   | bycrypt hash of a password                                              | 5d41402abc4b2a76... |

***Chores***

| Attribute   | Data Type | Bytes | Description                                                             | Example                   |
| ----------- | --------- | ----- | ----------------------------------------------------------------------- | ------------------------- |
| name        | String    | 256   | A free text name (actual name, initials, user selected username, etc.). | my chore, wash the dishes |
| description | String    | 1024  | A free text description (comments, description of whiteboard, etc.).    | This is my 13th chore     |
| time        | Timestamp | 8     | The time the chore will be due by                                       | 1:50pm                    |
| weekday     | Timestamp | 8<br> | The day that the chore is to be done                                    | Monday                    |

