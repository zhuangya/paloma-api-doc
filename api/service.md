## service(name[, fn])

Register a service constructor or get a service instance. If `fn` missing, return a service instance by `name`.

Param      | Type       | Description
:----------|:-----------|:-----------
**name**   | *String*   | The name of the service.  Must be unique to each service instance.
**fn**     | *Function* | A constructor function that will be instantiated as a singleton.
