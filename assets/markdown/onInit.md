`$onInit`

for ***all*** Controller initialisation code
```javascript
var myComponent = {
  ...
  controller: function () {
    this.$onInit = function () {
      this.foo = 'bar';
      this.bar = 'foo';
    };
    this.fooBar = function () {
      console.log(this.foo); // 'bar'
    };
  }
};
```