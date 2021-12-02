# Authentication

- The _auth_ endpoint is used for user authentication, user registration and user authorization
- The table is named **_users_** and it contains the following fields

## Database table

```mysql
mysql> SHOW COLUMNS FROM `users`
```

| **Field**         | **Type**     | **Null** | **Key** | **Default**       | **Extra**         |
| ----------------- | ------------ | -------- | ------- | ----------------- | ----------------- |
| user_id           | varchar(300) | NO       | PRI     | NULL              |                   |
| user_first_name   | varchar(100) | NO       |         | NULL              |                   |
| user_last_name    | varchar(100) | NO       |         | NULL              |                   |
| user_email        | varchar(100) | NO       | UNI     | NULL              |                   |
| registration_date | datetime     | YES      |         | CURRENT_TIMESTAMP | DEFAULT_GENERATED |

## Database table fields and description

| **Field**         | **Description**                                                            | **Example**                           |
| ----------------- | -------------------------------------------------------------------------- | ------------------------------------- |
| user_id           | user identity stored using [UUID](https://google.com?q=uuid) specification | 2d633e2e-9432-4982-8a18-ebbf7971f0e4  |
| user_first_name   | user's firstname                                                           | Jane                                  |
| user_last_name    | user's lastname                                                            | Doe                                   |
| user_email        | user's email                                                               | templatico@mailer.com                 |
| registration_date | the time stamp the user is registered                                      | 2021-11-30T04:40:42.000Z              |
