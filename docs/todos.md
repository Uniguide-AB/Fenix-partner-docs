## Contacts

#### `GET /contacts/{display_id}/todos`

`https://base-url.com/partners/v1/todos/12234567/todos`

```
[{
    "id": 1,
    "subject": "Jag har en fråga",
    "text": "Det är såhär att..",
    "due_at": "2021-11-06T23:00:00.000000Z",
    "completed_at": null,
    "is_due": true,
    "is_completed": false,
    "has_assigned_users": true,
}]
```

*Special fields*

| Field  | Possible values                                  |
| ------ | ------------------------------------------------ |
| `type` | `private` `organisation` _Yes, with s and not z_ |

#### `POST /contacts/{display_id}/todo`

`https://base-url.com/partners/v1/contacts/1`

