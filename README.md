
# users_テーブル
| Column     | Type   | Options     |
| ---------- | ------ | ------------|
| email      | string | null: false |
| password   | string | null: false |
| name       | string | null: false |
| profile    | test   | null: false |
| occupation | test   | null: false |
| position   | test   | null: false |

# Association
- has_many :prototypes
- has_many :comments

# prototypes
| Column     | Type       | Options     |
| ---------- | ---------- | ------------|
| title      | string     | null: false |
| catch_copy | string     | null: false |
| concept    | string     | null: false |
| image      |            |             |
| user       | references | null: false |

# Association
- belongs_to :users
- has_many   :comments

# comments
| Column     | Type       | Options     |
| ---------- | ---------- | ------------|
| test       | test       | null: false |
| user       | references | null: false |
| prototype  | references | null: false |

# Association
- belongs_to :users
- belongs_to :comments




