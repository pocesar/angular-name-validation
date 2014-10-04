angular-name-validation
=======================

Angular directive for validating UTF-8 full names on text inputs

## Usage

```js
angular.module('yourapp', ['nameValidation']);
```

```html
<input type="text" name-validation ng-model="ctrl.name" name="name">
<div ng-show="ctrl.form.name.$error.fullname">
  Please fill in a valid full name
</div>
```

if invalid, the `fullname` key will be added to the `$error` object on the `ngModel`
