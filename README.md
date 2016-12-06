# lrStickyHeader

make table headers sticky, example for [React CRM](http://reactcrm.com/)

![stStickeyHeader](http://i.imgur.com/ocN250H.gif)

[live demo](http://lorenzofox3.github.io/lrStickyHeader/example.html)

* (almost)no css to add 
* no dependency
* does not add any other element to the markup
* ~ 100 loc

## install 

``bower install lr-sticky-header``

``npm install lr-sticky-header``

## dependencies 

None

## usage

```Javascript
var tableElement = document.getElementById('table');

var stickyTable = lrStickyHeader(tableElement);

var parentElement = document.getElementById('scrollPanel');
var stickyTable2 = lrStickyHeader(tableElement, {parent: parentElement});
```

### style

You'll need your table element and its children to have the property ``box-sizing`` set to ``border-box`` (it is the default of many css framework such bootstrap

when the header is sticked the class name ``lr-sticky-header`` is added to the thead element if you want to add some more style

### api

*  **setWidth()** : if you want to call manually the resize of the column (within a resize event handler for example)
*  **clean()** ~: to detach the scroll event handler from the window

### [example of a directive](https://github.com/lorenzofox3/stStickyHeader) with [smart-table](http://lorenzofox3.github.io/smart-table-website/)
