# Todo Resource

| Field              | `Type`   | Remarks                                                      |
| ------------------ | -------- | ------------------------------------------------------------ |
| id                 | `int`    | Id of todo item                                              |
| subject            | `string` | Subject of the todo                                          |
| text               | `string` | The body of the todo                                         |
| due_at             | `string` | When the todo is expected to be expired                      |
| is_due             | `bool`   | `true` if the todo is expired, otherwise `false`             |
| is_completed       | `bool`   | if the given todo has been marked as completed by a fenix user |
| has_assigned_users | `bool`   | If the todo has any user assigned to it                      |

*Example response*

```
{
    "id": 1,
    "subject": "Byta telefonnummer",
    "text": "Jag önskar att byta mitt telefonnummer till 070147123213",
    "due_at": "2022-03-11T14:42:21.000000Z",
    "is_due": true,
    "is_completed": false,
    "has_assigned_users": true
}
```

