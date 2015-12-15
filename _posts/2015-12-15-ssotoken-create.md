---
category: SSO Token
path: '/-/api/ssotoken/create'
title: 'Create SSO token'
type: 'POST'

---

This method allows API consumers to create new users for their Koding teams.

### Authentication

* The headers must include a **valid authentication token**.
```Authentication: Bearer {TOKEN}```


### Parameters

* **username** (_required_)
  * should be an existing Koding username that belongs to API consumer's team.


### Response

**If succeeds**, returns a loginUrl. Redirecting the user to this url
should login the user immediately.

```{
  data : {
    loginUrl : 'someLoginUrl'
  }
}```

For error responses, see the [response status codes documentation](#/response-status-codes).
