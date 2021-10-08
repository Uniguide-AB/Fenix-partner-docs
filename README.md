# About Fenix partner integration

#### Endpoints

`https://BASE_NAME/api/partners/v1`

#### Rate limitation

The limit is 600 requests per minute and  Service account

#### Status codes

Our API can return 8 different status codes

| Code | Meaning                         |       Returns       |
| :--: | ------------------------------- | :-----------------: |
| 200  | Successfully retrieved resource |      **JSON**       |
| 201  | Successfully created resource   | _void_ or **JSON**  |
| 400  | Bad request                     | _Exception message_ |
| 403  | Forbidden due to permissions    | _Exception message_ |
| 404  | Resource not found              | _Exception message_ |
| 422  | Bad request with specifics      |      **JSON**       |
| 429  | To many requests                | _Exception message_ |
| 500  | Server error                    | _Exception message_ |

#### Authentication
All requests _must_ have an header named `Authentication` containing an valid token provided by the system owner.

#### Locale

The API can accept a header called `Locale` which defaults to `en`

Available Locales

* Swedish `se`
* English `en`

#### Token abilities

Token abilities determines what you can read / write from the API

* `contacts:read`
  * Validate contact existence by social security number
  * Read basic contact information
    * Customer number
    * Social security number / Organization numbers
    * Names
    * Phone numbers
    * Email addresses
    * Delivery addresses
    * Billing addresses
* `invoices:read`
  * List the latest 12 invoices

#### Routes

Here are all the routes currently supported

| URI                                   | Required token abilities        | Docs                          |
| ------------------------------------- | ------------------------------- | ----------------------------- |
| **Contacts**                          |                                 |                               |
| `GET /contacts/{ssn}/by-ssn`          | `contacts:read`                 | [Read more](docs/contacts.md) |
| `GET /contacts/{display_id}`          | `contacts:read`                 | [Read more](docs/contacts.md) |
| `GET /contacts/{display_id}/invoices` | `contacts:read` `invoices:read` | [Read more](docs/contacts.md) |
| **TBA**                               |                                 |                               |



