# BarChart
Выводит массив в виде барового графика.

## Детали

Рабочей областью для отрисовки графика служит `div#chart`.

Все общие стили объявленные в теге `style`. Для области отрисовки с помощью градиента наносятся вспомогательные элементы, а с помощью псевдоэлементов стрелочки графика.

Для самих баров применяется общий класс '.bar', с помощью которого бары прижимаются вниз и позиционируются в дальнейшем.

За размер графикаотвечает константа `BAR_SIZE`.

Перед отрисовкой идёт расчет нужной высоты и ширины "холста" в зависимости от размера массива (для ширины) и его значений (для высоты).

Для отрисовки одного бара используется функция `drawBar` которая имеет 2 параметра: `item, index` (значение и индекс). Функция создаёт элемент `div` задаёт общий класс `bar` устанавливаются соответствующие размеры и отступ. Затем идёт цветовая градация и добавления бара на страницу.

Для обработки всех элементов массива, функция передаётся как callback в метод `forEach`.

Онлайн версия на [codepen](https://codepen.io/artemveremienko/pen/zYqGdOX).
