A Recipe for **Success**

```html
<div>
  <ul>
    <li ng-repeat="user in activeUsers track by user.name">
      <p ng-bind="::user.name"></p>
      <span ng-bind="user.lastLogin"></span>
      <span ng-show="user.unreadMsgs" 
            ng-bind="user.unreadMsgs"></span>
    </li>
  </ul>
</div>
```