#JavaScript. Стиль кодирования.

##Переменные
1. Название с маленькой буквы (lowerCamelCase), аббревиатуры не сокращаются:
  - *Плохо:*
  ```javascript
  var MyVariable;
  var UseCss = true;
  ```
  - *Хорошо:*
  ```javascript
  var myVariable;
  var useCSS = true;
  ```
2. Объявлять в логическом блоке их непосредственного использования:
  - *Плохо:*
  ```javascript
  var myVar1 = 1;
  var myVar2 = ‘abc’;
  // some code
  if (myVar1 === 1) {
    // some code
  }
  // some code
  if (myVar2 === ‘abc’) {
      // some code
  }
  ```
  - *Хорошо:*
  // some code
  var myVar1 = 1;
  if (myVar1 === 1) {
      // some code
  }
  // some code
  var myVar2 = ‘abc’;
  if (myVar2 === ‘abc’) {
      // some code
  }
  ```
