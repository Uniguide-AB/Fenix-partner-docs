# User resource


| Field                                    | Remarks                                          |
| ---------------------------------------- | ------------------------------------------------ |
| `id`                                     | Unique DB id                                     |
| `display_id`                             | Display ID (Can be different from `id`)          |
| `type`                                   | `private` `organisation` _Yes, with s and not z_ |
| `active_category_junctions_fqdn_as_text` | Plain text summarizing  what categories are used |
| `ssn`                                    | Personal or organization number                  |
| `first_name`                             | Full name if organization                        |
| `last_name`                              | plain text or `null`                             |
| `email`                                  | plain text or `null`                             |
| `billing_email`                          | plain text or `null`                             |
| `phone1`                                 | plain text or `null`                             |
| `phone2`                                 | plain text or `null`                             |
| `delivery_address`                       | plain text or `null`                             |
| `delivery_co`                            | plain text or `null`                             |
| `delivery_postal_code`                   | plain text or `null`                             |
| `delivery_postal_city`                   | plain text or `null`                             |
| `billing_address`                        | plain text or `null`                             |
| `billing_co`                             | plain text or `null`                             |
| `billing_postal_code`                    | plain text or `null`                             |
| `billing_postal_city`                    | plain text or `null`                             |
| `is_active`                              | Boolean `true` or `false`                        |
| `activated_at`                           | date-string or `null`                            |
| `inactivated_at`                         | date-string or `null`                            |
| `inactivated_reason`                     | plain text or `null`                             |

*Example response*

```
{
    "id": 1,
    "display_id": "1",
    "type": "private",
    "active_category_junctions_fqdn_as_text": "Aktiv medlem (Nyhetsbrev, Försäkringstillägg 2)",
    "ssn": "19910510xxxx",
    "first_name": "tarre",
    "last_name": "islam",
    "email": null,
    "billing_email": null,
    "phone1": null,
    "phone2": null,
    "delivery_address": "Jungmansgatan 179",
    "delivery_co": null,
    "delivery_postal_code": "62151",
    "delivery_postal_city": "Visby",
    "billing_address": null,
    "billing_co": null,
    "billing_postal_code": null,
    "billing_postal_city": null,
    "is_active": true,
    "activated_at": "2021-11-06T23:00:00.000000Z",
    "inactivated_at": null,
    "inactivated_reason": null
}
```

