`$onChanges`

called in the local component controller from changes that occurred 
in the parent controller. Changes that occur from the parent which are
inputted into a component using `bindings: {} `

```javascript
var childComponent = {
  bindings: {
    user: '<'
  },
  template: '<div><pre>{{ $ctrl.user | json }}</pre></div>',
  controller: function () {
    this.$onChanges = function (changes) {
      this.user = changes.user.currentValue;
    };
  }
};
```