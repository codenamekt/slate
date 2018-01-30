# Account

## Get All Accounts

```python
import orinfra

infra = orinfra.authorize('dba')
orinfra.accounts.get()
```

```shell
curl "http://example.com/account"
  -H "Authorization: dba"
```

```golang
type Account struct {
  gorm.Model
  Name string `json:"name" db:"name"`
  Provider string `json:"provider" db:"provider"`
  Credential string `json:"credential" db:"credential"`
}
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Batman",
    "credential": "iamahero",
    "provider_id": 4324543
  },
  {
    "id": 2,
    "name": "Robin",
    "credential": "iamasidekick",
    "provider_id": 4324545
  }
]
```

This endpoint retrieves all accounts.

### HTTP Request

`GET http://example.com/account`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
name | false | Name of the account or subscription.
credential | false | If set to false, the result will include kittens that have already been adopted.
provider_id | false | Id of a provider.

<aside class="success">
Remember — a happy account is an authenticated one!
</aside>

## Get a Specific Account

```python
import orinfra

infra = orinfra.authorize('dba')
orinfra.accounts.get(2)
```

```shell
curl "http://example.com/account/2"
  -H "Authorization: dba"
```

> The above command returns JSON structured like this:

```json
{
    "id": 2,
    "name": "Robin",
    "credential": "iamasidekick",
    "provider_id": 4324545
}
```

This endpoint retrieves a specific account.

<aside class="warning">Credentials should be encrypted. &mdash; <code>&lt;Thomas&gt;</code></aside>

### HTTP Request

`GET http://example.com/account/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the account to retrieve