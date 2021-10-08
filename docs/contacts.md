## Contacts

#### `GET /contacts/{ssn}/by-ssn`

`https://base-url.com/partners/v1/contacts/19910510xxxx/by-ssn`

```
{
    "id": 1,
    "display_id": "1",
    "type": "private",
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
    "billing_postal_city": null
}
```

*Special fields*

| Field  | Possible values                                  |
| ------ | ------------------------------------------------ |
| `type` | `private` `organisation` _Yes, with s and not z_ |

#### `GET /contacts/{display_id}`

`https://base-url.com/partners/v1/contacts/1`

```
{
    "id": 1,
    "display_id": "1",
    "type": "private",
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
    "billing_postal_city": null
}
```

*Special fields*

| Field  | Possible values                                  |
| ------ | ------------------------------------------------ |
| `type` | `private` `organisation` _Yes, with s and not z_ |

#### `GET /contacts/{display_id}/invoices`

`https://base-url.com/partners/v1/contacts/1/invoices`

```
[
    {
        "ocr": "366494438582150",
        "public_url": "http://localhost/public/invoices/94951f4a-c2d1-4626-9ced-a3c0fee539b1",
        "paid_amount": "0",
        "amount": "200",
        "balance": "200",
        "due_date": "2021-11-06T23:00:00.000000Z",
        "billing_method": "postal",
        "billing_method_as_text": "Postalt",
        "type": "debit",
        "type_as_text": "Debet",
        "status": "active",
        "status_as_text": "Pågående"
    }
]
```

*Special fields*

| Field            | Possible values                                             |
| ---------------- | ----------------------------------------------------------- |
| `billing_method` | `postal` `kivra` `e_invoice` `ag` `pdf_e_mail` `pdf_manual` |
| `type`           | `credit` `debit`                                            |
| `status`         | `active` `completed`                                        |

