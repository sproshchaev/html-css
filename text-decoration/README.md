[![HTML](https://img.shields.io/badge/HTML-E46035??style=for-the-badge&logo=HTML5&logoColor=FFFFFF)](https://html.spec.whatwg.org/multipage/)
[![CSS](https://img.shields.io/badge/CSS-274DE4??style=for-the-badge&logo=CSS3&logoColor=FFFFFF)](https://www.w3.org/Style/CSS/)

### CSS: Горизонтальная черта
```
Для усиления текста часто используется подчёркивание. Оно показывает важность текущего слова или текста (часто его ещё используют для указания ссылок в документе). Другим средством стилизации текста является перечёркивание, показывающее неправильный участок текста, например «А вот так, дети, не делайте».

Для такого оформления используется свойство text-decoration с тремя основными свойствами:

underline — Подчёркивание текста
line-through — Перечёркивание текста
overline — Надчёркивание текста
Чтобы отменить подчёркивание у ссылок используется значение none. Его часто используют для удаления подчёркивания у ссылок, которое есть по умолчанию

<a href="#">Обычная ссылка с подчёркиванием по умолчанию</a>
<a href="#" class="text-decoration-none">Cсылка без подчёркивания</a>
.text-decoration-none {
  text-decoration: none;
}
```

### References
1. CSS: Горизонтальная черта https://code-basics.com/ru/languages/css/lessons/text-decoration