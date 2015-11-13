## route(route)

Register a route. `route` use `app.use` internally, so pay attention to the middleware load order.

Param                                 | Type                                 | Description
:-------------------------------------|:-------------------------------------|:-----------
**route**                             | *Object*                             | 
**route.method**                      | *String*                             | HTTP request method, eg: `GET`, `post`.
**route.path**                        | *String*                             | Request path, see [path-to-regexp](https://github.com/pillarjs/path-to-regexp), eg: `/:name`.
**route.controller**                  | *String\|Function\|[String\|Function]*  | Controller functions or names.
**route.validate**<br />*(optional)*  | *Object*                             | Validate Object schemas.
**route.template**<br />*(optional)*  | *String*                             | View name. If exist, return rendered html.

