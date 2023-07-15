## 具体的な操作
### ユーザデータ
* users

| user_id | user_name | mail_address | profile_text | header_image | password | regstration_date |
|---|---|---|---|---|---|---|
| 1 | A | A_address | Hello | A_image | A_pass | 2023/7/15 |
| 2 | B | B_address | GoodMorning | B_image | B_pass | 2023/7/14 |
| 3 | C | C_address | GoodNight | C_image | C_pass | 2023/7/13 |
| 4 | D | D_address | SeeYou | D_image | D_pass | 2023/7/12 |

### フォロー関係の操作
* user_follows

 | user_follow_id | follower_id | followee_id |
|---|---|---|
| 1 | 1 | 2 |
| 2 | 2 | 3 |

### リスト関係の操作
* lists

| list_id | list_name | author_id | header_image |
|---|---|---|---|
| 1 | リストA | 1 | listA_image |

* list_members

| list_member_id | user_id | list_id | operator_id |
|---|---|---|---|
| 1 | 2 | 1 | 1 |

### ツイート関係の操作
* tweets

| tweet_id | user_id | tweet_content | quote_tweet_id | reply_tweet_id | tweet_date |
|---|---|---|---|---|---|
| 1 | 1 | hello | null | null | 2023/7/15 |
| 2 | 2 | hi | null | 1 | 2023/7/15 |
| 3 | 1 | how are you? | 2 | null | 2023/7/15 |

* retweets

| retweet_id | user_id | tweet_id | retweet_date |
|---|---|---|---|
| 1 | 3 | 2 | 2023/7/15 |