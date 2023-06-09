[![HTML](https://img.shields.io/badge/HTML-E46035??style=for-the-badge&logo=HTML5&logoColor=FFFFFF)](https://html.spec.whatwg.org/multipage/)
[![CSS](https://img.shields.io/badge/CSS-274DE4??style=for-the-badge&logo=CSS3&logoColor=FFFFFF)](https://www.w3.org/Style/CSS/)

### CSS: Цветовая модель RGB
```
Свойства, значениями которых является цвет:

color
background-color
border-color

Для обозначения цвета использовалась шестнадцатеричная модель RGB, которая переводится как Red Green Blue. В CSS для обозначения цвета в RGB используется две основные записи:

1. Шестнадцатеричная. Это запись из 6 символов, разбитые на три блока по два значения. Каждый блок отвечает за один из цветов: красный, зелёный или синий
С использованием функции rgb(red, green, blue). Функция принимает три числа от 0 до 255, каждое из которых определяет количество красного, зелёного и синего цвета
Шестнадцатеричная запись
При использовании такой записи используется шестнадцатеричная система счисления. Запись делится на три блока по два числа:

от 00 до ff — количество красного цвета
от 00 до ff — количество зелёного цвета
от 00 до ff — количество синего цвета
/* Белый цвет */
color: #ffffff;

/* Чёрный цвет */
color: #000000;
Предположим, что для текста нужен фиолетовый цвет. Как он получается? Для этого смешивается красный и синий цвет. В фиолетовом отсутствует зелёный цвет. Значит нужна максимальная запись в первом и третьем блоке. Итого получится цвет #ff00ff

Текст фиолетового цвета
Можно получать разные вариации этого цвета, добавляя или уменьшая количество составных цветов

2. Функция rgb
Второй способ указать цвет с помощью цветовой модели RGB — использование специальной функции rgb(). Она принимает три числа от 0 до 255, где первое число определяет количество красного цвета, второе число — количество зелёного цвета, а третье — количество синего. Ничего не напоминает?

Если вам показалось, что это похоже на шестнадцатеричную систему, то будете правы — суть точно такая же. Только записываем цвета в привычных нам цифрах. В остальном всё то же самое, а значит можно создать фиолетовый цвет, используя функцию rgb():

<p class="text">Текст фиолетового цвета</p>
.text {
  color: rgb(255, 0, 255);
}
Текст фиолетового цвета
А вот как будет выглядеть белый и чёрный цвет при использовании функции rgb():

/* Белый цвет */
color: rgb(255, 255, 255);

/* Чёрный цвет */
color: rgb(0, 0, 0);

3. Прозрачность и функция rgba()
При использовании фонового цвета часто используют не просто цвет, но и добавляют ему прозрачность. В цветовой модели RGB для этого используется понятие «альфа»-канал. Он определяет насколько прозрачный цвет должен выводиться и задаётся числом от 0 до 1, где 0 — полностью прозрачный цвет, а 1 — полностью непрозрачный.

Чтобы использовать альфа-канал создаётся функция rgba(), где a — alpha. В остальном всё точно так же, как и было изучено ранее. Сделаем полупрозрачный фиолетовый фон:

<div class="background">Блок с полупрозрачным фиолетовым фоном</div>
.background {
  background-color: rgba(255, 0, 255, 0.5);
}
```
### References
1. CSS: Цветовая модель RGB https://code-basics.com/ru/languages/css/lessons/colors