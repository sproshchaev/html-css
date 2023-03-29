[![HTML](https://img.shields.io/badge/HTML-E46035??style=for-the-badge&logo=HTML5&logoColor=FFFFFF)](https://html.spec.whatwg.org/multipage/)
[![CSS](https://img.shields.io/badge/CSS-274DE4??style=for-the-badge&logo=CSS3&logoColor=FFFFFF)](https://www.w3.org/Style/CSS/)

### Figma
```
1. Файл css/reset.css необходим для обнуления всех стилей https://bit.ly/ResetCss
2. Добавление шрифтов: google-webfonts-helper — сервис для сохранения шрифтов из Google Fonts https://gwfh.mranftl.com/fonts
    1) Lato (sans-serif), Select styles: regular, 700, 900. 
    2) Copy CSS: Modern Browsers. Customize folder prefix (optional): ../fonts/
    3) создать style.css и скопировать в него все @font-face-ы для подключения шрифтов
    4) Download files: копируем все шрифты в ../fonts/
    5) В html подключить style.css <link rel="stylesheet" href="./css/style.css">
3. Настройка стилей в style.css
    1) параметры .item для блока <div>
    2) добавить box-sizing для html (это правильный способ подключения, который не сказывается на производительности): html {box-sizing: border-box;} *, *::before, *::after{box-sizing: inherit;}
    3) для сокращения времени зугрузки объединить файлы style.css и reset.css (перенести все в style.css)

```
### References
1. Figma https://www.youtube.com/watch?v=OkNfBnq_c7c&list=PL5_s7xdj2Vsw-bCx5nOZJMFIiHwRgok--
2. Файл reset.css https://gist.github.com/DavidWells/18e73022e723037a50d6
3. Вертикальное меню для сайта https://html5book.ru/vertikalnoe-menu/
