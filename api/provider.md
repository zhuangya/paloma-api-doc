## provider(name, fn)

Register a service provider.

Param        | Type       | Details
:------------|:-----------|:--------
**name**     | *String*   | The name of the service. Must be unique to each service instance.
**fn**       | *Function* | A constructor function that will be instantiated as a singleton. Should expose a function called `$get` that will be used as a factory to instantiate the service.

