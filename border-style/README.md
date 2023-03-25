[![HTML](https://img.shields.io/badge/HTML-E46035??style=for-the-badge&logo=HTML5&logoColor=FFFFFF)](https://html.spec.whatwg.org/multipage/)
[![CSS](https://img.shields.io/badge/CSS-274DE4??style=for-the-badge&logo=CSS3&logoColor=FFFFFF)](https://www.w3.org/Style/CSS/)

### CSS: Рамки
```
Любой блочный элемент в HTML можно выделять с помощью рамок. Такой стилистический приём позволяет удобно отделить однотонные компоненты друг от друга, или выделить ключевой элемент на странице

Этот текст находится в рамке, поэтому его легко найти с первого взгляда на странице

Для создания границы у элемента используется свойство border, которое является сокращением от нескольких свойств:

border-width — ширина границы
border-style — стиль границы
border-color — цвет границы
Можно указывать несколько свойств, а можно всё объединить в рамках свойства border. Такой вариант встречается чаще всего и выглядит он так:

.element {
  border: 1px solid #ccc;
}
где:

1px — ширина границы
solid — стиль границы
#ccc — цвет границы
Со значениями в пикселях и hex-цветом мы уже сталкивались в рамках курса, а вот стилей границ в CSS восемь:

dotted
dashed
solid
double
groove
ridge
inset
outset
и есть значение none, которое «удалит» границу, так как при значении border-style: none браузеры игнорируют другие свойства и удаляют границу
```
### References
1. CSS: Рамки https://code-basics.com/ru/languages/css/lessons/border-style