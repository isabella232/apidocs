---
title: 'Error codes'
---


### Error

Error responses are simply returning [standard HTTP error codes](http://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html) along with some additional information:

* The error code
* The error message

an example error response is:

```{
  "error": {
      "status": 409,
      "message": "This email is already in use, please try another one.",
      "code": "EmailAlreadyExists"
  }
}```


### List of errors

```{
  status                      : 500
  message                     : 'The server encountered an internal error.'
  code                        : 'InternalError'
}```

```{
  status                      : 400
  message                     : 'Request is invalid'
  code                        : 'InvalidRequestDomain'
}```

```{
  status                      : 403
  message                     : 'The group of the given api token
                                does not exist.'
  code                        : 'GroupNotFound'
}```

```{
  status                      : 403
  message                     : 'Api usage for this group is disabled.'
  code                        : 'ApiIsDisabled'
}```

```{
  status                      : 400
  message                     : 'Api token is invalid.'
  code                        : 'InvalidApiToken'
}```

```{
  status                      : 401
  message                     : 'The request is unauthorized,
                                an api token is required.'
  code                        : 'UnauthorizedRequest'
}```

```{
  status                      : 400
  message                     : 'One of the request inputs is invalid.'
  code                        : 'InvalidInput'
}```

```{
  status                      : 500
  message                     : 'An error occurred, failed to create user.'
  code                        : 'FailedToCreateUser'
}```

```{
  status                      : 500
  message                     : 'An error occurred, failed to create user
                                session. User may not be logged in.'
  code                        : 'failedToCreateSession
}```

```{
  status                      : 409
  message                     : 'This username is already in use,
                                please try another one.'
  code                        : 'UsernameAlreadyExists'
}```

```{
  status                      : 409
  message                     : 'This email is already in use,
                                please try another one.'
  code                        : 'EmailAlreadyExists'
}```

```{
  status                      : 400
  message                     : 'This email domain is not in
                                allowed domains for this group.'
  code                        : 'InvalidEmailDomain'
}```

```{
  status                      : 400
  message                     : 'Given username is invalid.'
  code                        : 'InvalidUsername'
}```

```{
  status                      : 400
  message                     : 'User is not a member of the api token group.'
  code                        : 'NotGroupMember'
}```

```{
  status                      : 400
  message                     : 'The sso token in request could not be parsed.'
  code                        : 'SSOTokenFailedToParse'
}```

```{
  status                      : 400
  message                     : 'One of the required fields in
                                payload is invalid'
  code                        : 'InvalidSSOTokenPayload'
}```

```{
  status                      : 400
  message                     : 'A required query parameter was
                                not specified for this request.'
  code                        : 'MissingRequiredQueryParameter'
}```

```{
  status                      : 400
  message                     : 'Given username is out of range.'
  code                        : 'OutOfRangeUsername'
}```

```{
  status                      : 400
  message                     : 'Given suggested username is out of range.'
  code                        : 'OutOfRangeSuggestedUsername'
}```