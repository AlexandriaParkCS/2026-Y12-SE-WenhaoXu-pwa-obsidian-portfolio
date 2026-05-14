***User***

| Attribute    | Data Type | Bytes | Description                                                             | Example             |
| ------------ | --------- | ----- | ----------------------------------------------------------------------- | ------------------- |
| name         | String    | 256   | A free text name (actual name, initials, user selected username, etc.). | johnd, John Doe     |
| email        | String    | 64    | A valid email address.                                                  | john@abc.com        |
| pwd_hash     | String    | 128   | bycrypt hash of a password                                              | 5d41402abc4b2a76... |
| member since | Timestamp | 8     | The date and time when the user created their account.                  | 27/02/2026 16:38.42 |
***Whiteboard***

| Attribute    | Data Type | Bytes | Description                                                             | Example                             |
| ------------ | --------- | ----- | ----------------------------------------------------------------------- | ----------------------------------- |
| name         | String    | 256   | A free text name (actual name, initials, user selected username, etc.). | my_whiteboard, The Binomial Theorem |
| description  | String    | 1024  | A free text description (comments, description of whiteboard, etc.).    | This is my 13th Whiteboard!         |
| date_created | Timestamp | 8     | The date and time when the whiteboard was made.                         | 27/02/2026 1:39:20pm                |
| last_used    | Timestamp | 8     | The date and time when the whiteboard was last accessed.                | 27/02/2026 1:40:28pm                |
|              |           |       |                                                                         |                                     |
