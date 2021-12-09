# Invoice Resource

| Field                  | `Type`   | Remarks                                                      |
| ---------------------- | -------- | ------------------------------------------------------------ |
| ocr                    | `string` | OCR of the invoice                                           |
| public_url             | `string` | Url to the PDF                                               |
| paid_amount            | `string` | The amount in SEK paid                                       |
| amount                 | `string` | The total amount to pay                                      |
| balance                | `string` | How much is left to pay                                      |
| due_date               | `string` | zulu                                                         |
| billing_method         | `string` | one of `postal` `kivra` `e_invoice` `ag` `pdf_e_mail` `pdf_manual` |
| billing_method_as_text | `string` | Human readable version of `billing_method`, example "E-faktura" |
| type                   | `string` | `credit` `debit`                                             |
| type_as_text           | `string` | Human readable version of `type`, example "Kredit"           |
| status                 | `string` | `pending` `active` `completed`                               |
| status_as_text         | `string` | Human readable version of `status`, example "Pågående"       |

*Example response*

```
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
```

