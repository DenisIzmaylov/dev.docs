#JavaScript. Стиль кодирования.

##Переменные
1. Название с маленькой буквы (lowerCamelCase), аббревиатуры не сокращаются:
  - *Плохо:*
  ```javascript
  var MyVariable;
  var UseCss = true;
  ```
  - **Хорошо:**
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
  - **Хорошо:**
  ```javascript
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

##Черновые заметки
- Если много мелких самодостаточных модулей (до 2 файлов), то можно сгруппировать директории по типам файлов (js, css, images).
- Если модули имеют разветвлённую структуру (больше 2 файлов каждого типа на модуль), то имеет смысл разделить по директориям модулей (module1, module2, module3).
- Избегать сайд-эффектов (функция взаимодействует только с теми объектами, которые ей переданы и своим владельцем - this).

##Ссылки
- http://programer.tips/2014/09/best-jquery-practices.html
- http://blog.risingstack.com/node-js-best-practices/
