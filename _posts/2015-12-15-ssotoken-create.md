---
category: SSO Token
path: '/-/api/ssotoken/create'
title: 'Create SSO token'
type: 'POST'

---

This method allows API consumers to create SSO tokens for the users in their teams.
With a SSO token, users can login to their Koding team domains without entering
username and password.

### Authorization

* The request headers must include a **valid API token** which can be obtained from team settings page.
```Authorization: Bearer {TOKEN}```


### Parameters

* **username** (_required_)
  * should be an existing Koding username that is registered to API consumer's team domain.


### Response

**If succeeds**, returns a loginUrl which contains the SSO token.
Redirecting the user to this url should login the user immediately.

```{
  data : {
    loginUrl : 'someLoginUrl'
  }
}```

For error responses, see the [error responses documentation](#/error-responses).
