`$postLink`

enables us to hook into the final phase of the compile process - where we know
for sure our child elements are compiled and linked

```javascript
var myComponent = {
  ...
  controller: function () {
    this.$postLink = function () {
      // execute sports
    };
  }
};
```