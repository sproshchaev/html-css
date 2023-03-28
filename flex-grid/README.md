[![HTML](https://img.shields.io/badge/HTML-E46035??style=for-the-badge&logo=HTML5&logoColor=FFFFFF)](https://html.spec.whatwg.org/multipage/)
[![CSS](https://img.shields.io/badge/CSS-274DE4??style=for-the-badge&logo=CSS3&logoColor=FFFFFF)](https://www.w3.org/Style/CSS/)

### CSS: flex и grid
```
1. Flex - более современный инструмент, чем Grid и рекомкндуется его использовать вместо Grid. Flex проще настраивается чем Grid (с Grid надо еще повозиться)  

Файл index.css
    Свойства .container
        height: 800px; - высота
        background-color: gray; - цвет фона

    Свойства Flex:

        display: flex; - позволяет адаптировать грид под размер экрана и сжимать при необходимости

        flex-direction: row; - слева на право (1..10). Он является базовым, если явно не задается, то используется row.
        flex-direction: row-reverse; - справа на лево (10..1)
        flex-direction: column; - по вертикали сверху вниз (1..10)
        flex-direction: column-reverse; - по вертикали сверху вниз (10..1)

        flex-wrap: wrap; - позволяет переностить на следующую строку при сжатии  (базовая опция)
        flex-wrap: wrap-reverse; - переносит на следующую строку при сужении экрана в обратном порядке, т.е. закидывает не вниз, а наверх

        Как закидывать наши элементы внутрь контейнеров div?
        justify-content: center; - все блоки помещены по центру экрана
        justify-content: flex-start; - все блоки с левого края
        justify-content: flex-end; - все блоки с правого края 
        justify-content: space-between; - поставить с зазорами (в равных долях между элементами)
        justify-content: space-around; - тоже что и space-between но добавляются зазоры слева и справа
        justify-content: space-evenly; - все зазоры максимально равны между собой 
        
        align-items: center; - центрирует по вертикали
        align-items: flex-start; - располагает все сверху
        align-items: flex-end; - закинет все вниз
        align-items: stretch; - растягиваются (используется редко)
        align-items: baseline; - держится где был 

        align-content: flex-start; - накидывает сверху элементы (используется редко)
        align-content: flex-end; - накидывает снизу элементы (используется редко)

        align-self: flex-start; - точечно для дочернего элемента задает его место расположения 

    Вывод: всегда будет: display: flex; flex-wrap: wrap; justify-content: center; align-items: center;

        order: 6; - изменяет порядок элемента, если был 3-ий, то станет 6-ым       
        flex-grow: 4; - можно расти до 4-х элементов (рост)
        flex-shrink 2; - может сжиматься (сужение)
        flex-basic: auto; - определяет размер элементов по умолчанию, когда распределяется пространство (auto - по умолчанию, может быть 150px, 200px)

        сокращенная запись flex: <grow> <shrink>, пример flex: 1 1 200px

    Рекомендация: не пытайтесь использовать все перечисленные свойства, в 90% случаев достаточно в проекте всего двух свойств: justify-content: space-between; и align-items: center;       

2. Grid - (тайминг у п.1. 59:08)
    Свойства Grid:

        display: grid; - главное свойство, которое определяет, что будет использоваться Grid
        grid-template-columns: 100px 100px ..100px; - создание колонок с заданным размером каждой колонки в 100 px
        grid-template-columns: 10% 10% - создаст две колонки с шириной в 10% от ширины контейнера, также можно по всей ширине grid-template-columns:  15% 50% 35%
        grid-template-columns: 1fr 1fr - создаст две колонки - разделит всю ширину на два, значит 1 fr = 50% ширины
        grid-template-rows: 15% 15% 15% - создаст три строки с размером 15%

        gap: 20px 50px; - добавляет разделение между элементами в ряду (первое значение) и колонками (второе значение) 

        grid-area - позволяет использовать "конструктор" для грида (тайминг у п.1.  1:23:00)
        grid-template-areas - для grid-area

        функция repeat() позволяет сокращать описание: grid-template-columns: repeat(1fr, 2) аналогично grid-template-columns: 1fr 1fr 

```
### References
1. JS/FE 2021Q3 Stage#1 CSS/Grid https://www.youtube.com/watch?v=0wnTkMeOTv0
2. Расположение элементов во flex (видео по слайдам) https://youtu.be/iSQcOjxttNg?list=PLe--kalBDwji8WXKVjhON39X4v_Uj6T_R&t=2053
3. Основные понятия Grid Layout https://developer.mozilla.org/ru/docs/Web/CSS/CSS_Grid_Layout/Basic_Concepts_of_Grid_Layout
4. Полное руководство по CSS Grid https://tuhub.ru/posts/css-grid-complete-guide
5. Вёрстка на Grid в CSS. Полное руководство и справочник http://bit.ly/40kbfGm 
6. CSS Grid #0 Введение в курс (Introduction) http://bit.ly/3JQRorg 
7. Изучение гридов посредством игры https://cssgridgarden.com/#ru

