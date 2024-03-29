## Приложение WeatherApp
Предназначено для получения информации о погоде со 110 тысяч метеостанций по всему миру

Для запуска приложения нужно нажать на кнопку "Поиск города" в левой части экрана, и ввести в поле ввода название города на русском языке.

Результаты на данный момент будут отражены в левой части экрана (в сайдбаре), в правой части экрана будет дан прогноз на 5 дней и почасовой с шагом в 3 часа.

Отображается основная информацию: температура, скорость ветра, влажность, видимость.

На стороне клиента сохраняется история последних 5 запросов (отображается в сайдбаре).

## Структура файлов (папка src):
# components (папка с компонентами):
-- apiBlock - модули для выполнения запросов к API для получения географических координат города (apiGetCity) и данных о погоде (apiGetData);
-- MainBlock (основной блок с файлами jsx):
--- SidebarBlock - модуль сайдбара для ввода запросов и получения данных о погоде на текущий момент;
---- Switch - модуль переключения темы (светлая / темная);
--- TopMainPanel - панель для вывода прогноза погоды (с переключением на 5 дней / почасовой (с шагом в 3 часа));
---- CarouselPanel - слайдер;
--- LowMainPanel - панель для вывода прогноза погоды на предстоящий день;
# styles (папка с глобальными стилями)
# utils (папка со вспомогательными функциями)
## tests (папка с файлом для организации работы с unit-тестами):

## Основные зависимости
- [@testing-library/jest-dom](https://www.npmjs.com/package/@testing-library/jest-dom) - версия 5.17.0
- [@testing-library/react](https://www.npmjs.com/package/@testing-library/react) - версия 13.4.0
- [@testing-library/user-event](https://www.npmjs.com/package/@testing-library/user-event) - версия 13.5.0
- [react](https://reactjs.org/) - версия 18.2.0
- [react-dom](https://reactjs.org/docs/react-dom.html) - версия 18.2.0
- [react-scripts](https://www.npmjs.com/package/react-scripts) - версия 5.0.1
- [styled-components](https://styled-components.com/) - версия 6.1.8
