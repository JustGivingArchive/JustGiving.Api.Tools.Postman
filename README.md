JustGiving.Api.Tools.Postman
============================

It's config file for Postman https://chrome.google.com/webstore/detail/postman-rest-client/fdmmgilgnpjigdojojpjoooidkmcomcm?hl=en.

This file will add JustGiving API methods to your postman collections, whole documentation you can find here https://api.justgiving.com/docs

Additionally we have provided two environment config files, which ideally fit into collection files. Basically you have to change those two values

```text
yourAppID -> Your generated appId https://apimanagement.justgiving.com/
```

and

```text
yourBasicAuthToken -> Your generated basic authentitacion key
```

You can easily import those environment config files by choosing : Manage environments -> Import
By having environment configuration, you can very easily change variables against our environments like sandbox and production.