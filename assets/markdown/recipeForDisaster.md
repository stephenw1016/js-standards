A Recipe for **Disaster**

```html
<div>
  <ul>
    <li ng-repeat="user in getUsers() | filter:activeUsers">
      <p>{{user.name}}</p>
      <span>{{user.lastLogin}}</span>
      <span ng-show="hasUnreadMsgs(user)">{{user.messages}}</span>
    </li>
  </ul>
</div>
```