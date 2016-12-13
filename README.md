# elastic-delete

A Polymer Element providing a way to delete a single elasticsearch document based on an _id.

### Example
```html
<elastic-client
  config='{"host": "http://localhost:9200"}'
  client="{{esclient}}"
  cluster-status="{{my-status}}">
</elastic-client>

<elastic-delete
  client="[[esclient]]"
  index="mockads"
  id="4"
  elastic-type="ad"
  results="{{data}}"
  last-error="{{error}}">
</elastic-delete>
```

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests require a local instance of elasticsearch with the `mockads` index created by running `data/import_test_data.sh`.

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

