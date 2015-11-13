## factory(name, fn)

Register a service factory.

Param       | Type       | Description
:-----------|:-----------|:--------
**name**    | *String*   | The name of the service.  Must be unique to each service instance.
**fn**      | *Function* | A function that should return the service object. Will only be called once; the Service will be a singleton. Gets passed an instance of the container to allow dependency injection when creating the service.

