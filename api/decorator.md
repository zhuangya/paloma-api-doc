## decorator([name, ]fn)

Register a decorator function that the provider will use to modify your services at creation time.

Param                      | Type       | Details
:--------------------------|:-----------|:--------
**name**<br />*(optional)* | *String*   | The name of the service this decorator will affect. Will run for all services if not passed.
**fn**                     | *Function* | A function that will accept the service as the first parameter. Should return the service, or a new object to be used as the service.
