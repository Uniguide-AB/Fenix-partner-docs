# Todo Request

| Field   | `Type`   | Remarks                                                      | Rules                      |
| ------- | -------- | ------------------------------------------------------------ | -------------------------- |
| subject | `string` | The subject for the todo                                     | required, string, max:191  |
| text    | `string` | The body of the todo                                         | required, string, max:1024 |
| due_at  | `string` | This date also determines when in the Fenix calendar it will show up | can be null, date          |

*Example request*

```
{
    "subject": "Byta telefonnummer",
    "text": "Jag önskar att byta mitt telefonnummer till 070147123213",
    "due_at": null
}
```

