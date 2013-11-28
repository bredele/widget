# View

  > Data binding wrapper

## Installation

    $ component install leafs/view

## API

### .html(tmpl, model)
  
  render template into dom and create binding with model (object or store)

### .insert(node, location)

  place the view dom into the document
  location can be beforebegin, afterbegin, beforeend (default), afterend

### .alive([node])

  apply binding on node (node can be the view dom or a document node)


## Usage

```js
var View = require('view');
var view = new View();
view.html('<span>{name}</span>', {
  name:'bredele'
});
view.insert(document.body);
```

## TODO

  - [ ] test and code destroy (destory plugin and dom)
  - [ ] add cross browser insert adjacent


## License

  MIT
