`$onDestroy`

for cleaning up things that can cause memory leaks

```javascript
var childComponent = {
  bindings: {
    user: '<'
  },
  controller: function () {
    this.$onDestroy = function () {
      // clean-up
    };
  }
};
```