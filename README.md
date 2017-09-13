# result-list

A Polymer Element showing a paginated-list of single-result elements.

### Example
```js
headerExtractions = [{
  name: 'Built By',
  data: [{
    confidence: 'high',
    highlight: true,
    icon: 'star',
    link: 'https://nextcentury.com',
    text: 'Next Century'
  }]
}];

details = [{
  name: 'Description',
  text: 'DigElements is a library of common Polymer Elements built by Next Century Corporation.'
}];

detailExtractions = [{
  name: 'My Favorite DigElements',
  data: [{
    confidence: 'high',
    highlight: true,
    icon: 'link',
    link: 'https://github.com/DigElements/single-result',
    text: 'Single Result'
  }]
}];

images = [{
  link: 'https://github.com/DigElements',
  source: 'dig.png'
}];

results = [{
  flag: 'Important',
  highlightedText: 'The <em>DigElements</em> library.',
  icon: 'favorite',
  link: 'https://github.com/DigElements',
  rank: '0.99',
  type: 'Webpage',
  headerExtractions: headerExtractions,
  details: details,
  detailExtractions: detailExtractions,
  images: images
}];
```

```html
<result-list
  query-results="[[results]]"
  total-results="1"
  loading="[[loading]]"
  header="{{header}}">
</result-list>
```

### Styling

`<result-list>` provides the following custom properties and mixins for styling:

Custom property                  | Description                                | Default
---------------------------------|--------------------------------------------|--------
`--result-list-loading-spinner`  | Mixin applied to the loading-spinner       | none
`--result-list-max-height`       | Maximum height of the list                 | 1500px
`--result-list-scroll-threshold` | Mixin applied to the iron-scroll-threshold | none
`--result-list-show-more-button` | Mixin applied to the show more button      | none

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

