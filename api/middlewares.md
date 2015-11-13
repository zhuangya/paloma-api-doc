## middlewares([name, ]fn)

Register a middleware function. This function will be executed every time the service is accessed. Distinguish with koa's `middleware`.

Param                      | Type       | Details
:--------------------------|:-----------|:--------
**name**<br />*(optional)* | *String*   | The name of the service for which this middleware will be called. Will run for all services if not passed.
**fn**                     | *Function* | A function that will accept the service as the first parameter, and a `next` function as the second parameter. Should execute `next()` to allow other middleware in the stack to execute. Bottle will throw anything passed to the `next` function, i.e. `next(new Error('error msg'))`.

