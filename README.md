## create auth login flow


```mermaid

erDiagram
direction LR
user ||--o{ session :has

user{
    int id_user PK
    string firs_name
    string last_name
    string email
    string password
}

session{
    int id_login PK
    string email
    string password
    int id_user FK
}


```
