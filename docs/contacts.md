## Contacts

#### `GET /contacts/{ssn}/by-ssn`

`https://base-url.com/partners/v1/contacts/19910510xxxx/by-ssn`

Returns: [User resource](resources/user.md)

#### `GET /contacts/{display_id}`

`https://base-url.com/partners/v1/contacts/1`

Returns: [User resource](resources/user.md)

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
| `status`         | `active` `completed` `pending`                              |

