<h3 id="xpath">XPath</h3>

**XPath (XML Path Language)** — это язык запросов к элементам XML-документа. Представьте, что в документе Word вы сочетанием клавиш `Ctrl + F` вызываете функцию поиска контента. Вписывая что-то в поле ввода, вы можете осуществить поиск элементов в вашем документе. То же самое можно делать и в коде HTML, только тут функционал поиска расширяется как раз за счёт XPath'ов, при помощи которых вы можете либо точно указать позицию элемента, либо найти элементы, относящиеся к конкретному классу и многое-многое другое. 

Самый простой способ получить XPath — это во вкладке `Elements` нажать правой кнопкой на элемент и нажать на "Copy full XPath", тем самым скопировав _абсолютный_ XPath. Выглядеть он будет примерно следующим образом: `/html/body/div[11]/div/div`. Означает это то, что наш элемент (конечный блок `div`) располагается в другом блоке, который располагается 11-ым по счёту блоком в третьем блоке `div`, который, в свою очередь, располагается в `body`, который находится в главном теге `html`. Но в подобных абсолютных указателях есть два огромных недостатка:

1. Это совершенно неудобно читать и не сразу понятно, о каком элементе идёт речь.
2. Если HTML-код данной страницы хотя бы немного поменяется, например, добавится новый блок и тем самым сдвинет наш элемент выше или ниже, то такой XPath будет указывать уже на совсем другой элемент.

Для _относительного_ XPath путь начинается с середины структуры HTML DOM. Он начинается с двойной косой черты (`//`), что означает, что он может искать элемент в любом месте на веб-странице. Далее используется имя тега нужного нам узла, указывается атрибут узла и значение этого атрибута: `//tagname[@Attribute='value']`. Например, представим, что мы пишем XPath до поля ввода Email адреса в простом веб-приложении, тогда он может быть написан двумя способами:

- `/html/body/div/div/form/table/tbody/tr/td/input`
- `//input[@id='email']`

Второй XPath выглядит гораздо лучше первого, не так ли?

---
---
# Задание №1.XPath на сайте [СберСтрахования](https://online.sber.insure/store/propertyins/)</h3>

Перейдите на сайт [СберСтрахования](https://online.sber.insure/store/propertyins/). Ознакомьтесь с основным функционалом приложения. Создайте файл `XPath1.md`, в котором опишите XPath'ы на первых двух страницах ("1. Выбор полиса" и "2. Оформление")  для:
- Каждой кнопки;
- Каждого поля для ввода текста;
- Каждого чекбокса;
- Каждого датапикера;
- Логотипа "СБЕР СТРАХОВАНИЕ";
- Слайдера в блоке выбора суммы;
- Хедера "Что будет застраховано?";
- Текстовых блоков: "Мебель, техника и ваши вещи", "Падение летательных аппаратов и их частей";
- Каждой колонки в списка, который находится под хедером "Страховая защита включенная в программу".

_P.S.: XPath'ы нужно писать для каждого элемента отдельно_