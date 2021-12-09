# Contact resource


| Field                                    | Type              | Remarks                                             |
| ---------------------------------------- | ----------------- | --------------------------------------------------- |
| `id`                                     | `number`          | Unique DB id                                        |
| `display_id`                             | `string`          | Can differ from `id`                                |
| `type`                                   | `string`          | `private` `organisation` _Yes, with s and not z_    |
| `active_category_junctions_fqdn_as_text` | `string`          | Summary of what categories are used                 |
| `ssn`                                    | `string` / `null` | Personal or organization number                     |
| `first_name`                             | `string` / `null` | Full name if organization                           |
| `last_name`                              | `string` / `null` |                                                     |
| `email`                                  | `string` / `null` |                                                     |
| `billing_email`                          | `string` / `null` |                                                     |
| `phone1`                                 | `string` / `null` |                                                     |
| `phone2`                                 | `string` / `null` |                                                     |
| `delivery_address`                       | `string` / `null` |                                                     |
| `delivery_co`                            | `string` / `null` |                                                     |
| `delivery_postal_code`                   | `string` / `null` |                                                     |
| `delivery_postal_city`                   | `string` / `null` |                                                     |
| `billing_address`                        | `string` / `null` |                                                     |
| `billing_co`                             | `string` / `null` |                                                     |
| `billing_postal_code`                    | `string` / `null` |                                                     |
| `billing_postal_city`                    | `string` / `null` |                                                     |
| `is_active`                              | `boolean`         | If the contact is considered active                 |
| `activated_at`                           | `string` / `null` | zulu-date, when the contact was first activated at  |
| `inactivated_at`                         | `string` / `null` | zulu-date, when the contact was last inactivated at |
| `inactivated_reason`                     | `string` / `null` | The human written reason for the inactivation       |

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

