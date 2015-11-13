### Example

```javascript
'use strict';

const Paloma = require('paloma');
const app = new Paloma();

app.controller('indexCtrl', function (ctx, next, indexService) {
  ctx.body = `Hello, ${indexService.getName()}`;
});

app.service('indexService', function () {
  this.getName = function () {
    return 'paloma';
  };
});

app.route({
  method: 'GET',
  path: '/',
  controller: 'indexCtrl'
});

app.listen(3000);
```
More examples see [test](https://github.com/palomajs/paloma/tree/master/test) and [paloma-examples](https://github.com/palomajs/paloma-examples).
