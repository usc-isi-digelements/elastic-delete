# elastic-delete

Element providing a way to delete a single elasticsearch document based on an _id. 

Example:
```html
    <template is="dom-bind">
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
    </template>
```

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

To run the demo, you will need a local elasticsearch instance and the 
mockads data referenced in the elastic-client-search repo.
