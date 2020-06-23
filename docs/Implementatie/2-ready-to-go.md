---
tags: [Implementatie details]
---

# Ready-to-go

<!-- title: Course api-calls -->

| Method   | URL                        | Name              | Ready | Documented |
| -------- | -------------------------- | ----------------- | :---: | :-: |
| `GET`    | /course/all                | Get all courses   |   ✓   |  ✓  |
| `GET`    | /course/{code} | Get course details |   ✓   |   ✓  |
| `GET`    | /course/{code}/issues | Get course issues |   ✓   |  ✓  |
| `POST`   | /course/new                | Create course        |   ✓   |  ✓  |
| `POST`   | /course/{code}/remove | Remove course     |   ✓   |  ✓   |
| `POST`   | /course/{code}/modify | Modify course     |   ✓   |  ✓  |


<!-- title: Issue api-calls -->

| Method   | URL                       | Name              | Ready | Documented |
| -------- | ------------------------- | ----------------- | :---: | :-: |
| `GET`    | /issue/{issue_id}         | Get issue details |   ✓   |  ✓  |
| `GET`    | /issue/{issue_id}/comments  | Get issue comments |   ✓   |  ✓  |
| `POST`   | /issue/new                | Create issue      |   ✓   |  ✓  |
| `POST`   | /issue/duplicates         | Get issue duplicates      |   ✓   |  ✓  |
| `POST`   | /issue/{issue_id}/modify  | Modify issue      |   ✓   |  ✓  |
| `POST`   | /issue/{issue_id}/vote{vote_type}    | Up/downvote  |   ✓   |  ✓  |
| `POST`   | /issue/{issue_id}/resolve | Resolve issue     |   ✓   |  ✓  |
| `POST`   | /issue/{issue_id}/remove  | Remove issue      |   ✓   |  ✓  |

<!-- title: User api-calls -->

| Method   | URL                    | Name             | Ready | Documented |
| -------- | ---------------------- | ---------------- | :---: | :-: |
| `GET`    | /user/all              | Get users      |   ✓   |   ✓  |
| `GET`    | /user/{user_id}        | Get user details |   ✓   |  ✓  |
| `GET`    | /user/{user_id}/issues | Get user issues  |   ✓   |  ✓  |
| `GET`    | /user/{user_id}/courses | Get user courses  |  ✓   |  ✓ |
| `GET`    | /user/{user_id}/comments | Get user comments  |   ✓   |  ✓   |
| `POST`   | /user/new              | Create user      |   ✓   |  ✓  |
| `POST`   | /user/login            | Login            |   ✓   |  ✓  |
| `POST`   | /user/forgot_password  | Forgot password  |       |     |
| `POST`   | /user/{user_id}/modify | Modify user      |   ✓   |  ✓  |
| `POST`   | /user/{user_id}/verify | Verify user      |       |     |
| `POST`   | /user/{user_id}/promote | Promote user    |   ✓   |  ✓  |
| `POST`   | /user/{user_id}/remove | Remove user      |   ✓   |  ✓  |


<!-- title: Comment api-calls -->

| Method   | URL                    | Name             | Ready | Documented |
| -------- | ---------------------- | ---------------- | :---: | :-: |
| `GET`    | /comment/{comment_id}        | Get comment      |   ✓   |  ✓  |
| `POST`   | /comment/new              | Create comment   |   ✓   |  ✓  |
| `POST`   | /comment/{comment_id}/vote/{vote_type}   | Upvote comment  |  ✓  |  ✓  |
| `POST`   | /comment/{comment_id}/modify | Modify comment   |   ✓   |  ✓  |
| `POST`   | /comment/{comment_id}/remove | Remove comment   |   ✓   |  ✓  |