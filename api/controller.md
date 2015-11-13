## controller(name[, fn])

Register or get a controller. If `fn` missing, return a controller by `name`.

Param                       | Type        | Description
:---------------------------|:------------|:-----------
**name**                    | *String*    | Controller name.
**fn**<br />*(optional)*    | *Function*  | Controller handler.
**fn->arguments[0]->ctx**   | *Object*    | Koa's `ctx`.
**fn->arguments[1]->next**  | *Function*  | Koa's `next`.
**fn->arguments[2...]**     | *Object*    | Instances of services.
