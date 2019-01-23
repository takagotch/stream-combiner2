### stream-combiner2
---
https://github.com/substack/stream-combiner2

```js
var combine = require('stream-combiner2')

var Combine = require('stream-combiner')
var es = require('event-stream')

Combine(
  process.openStdin(),
  es.split(),
  es.map(function(data, callback){
    var repr = inspect(JSON.parse(data))
    callback(null, repr)
  }),
  process.stdout
)

```

```
```

```
```


