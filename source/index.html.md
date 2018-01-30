---
title: OR Infra API

language_tabs:
  - shell
  - python
  - golang

toc_footers:
  - <a href='#'>Get Access</a>

includes:
  - account
  - cluster
  - node-flavor
  - node-group
  - product
  - provider
  - rbac-binding
  - region
  - role
  - api-errors

search: true
---

# Introduction

Welcome to the Infra API! You can use this api to access and manage infrastructure, purpose built for the ObjectRocket Platform. 

# Authentication

> To authorize, use this code:

```python
import orinfra

infra = orinfra.authorize('dba')
```

```shell
# With shell, you can just pass the correct header with each request
curl "example.com"
  -H "Authorization: dba"
```

> Make sure to replace `dba` with your API key.

Infra API uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).

Infra API expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: dba`

<aside class="notice">
You must replace <code>dba</code> with your personal API key.
</aside>
