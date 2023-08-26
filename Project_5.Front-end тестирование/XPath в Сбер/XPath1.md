# 1. Выбор полиса <br>
## Кнопки <br>
**_Квартира_** <br>`//button[@id="mat-button-toggle-1"]` <br> **_Дом_** <br>`//button[@id="mat-button-toggle-2"]`<br>**_Сдается в аренду - Да_** <br>`//button[@id="mat-button-toggle-22"]`<br>**_Сдается в аренду - Нет_** <br>`//button[@id="mat-button-toggle-23"]`<br>**_Расположена на первом или последнем этаже - Да_** <br>`//button[@id="mat-button-toggle-25"]`<br>**_Расположена на первом или последнем этаже - Нет_** <br>`//button[@id="mat-button-toggle-26"]` <br>**_Установлена охранная сигнализация - Да_** <br>`//button[@id="mat-button-toggle-28"]`<br>**_Установлена охранная сигнализация - Нет_** <br>`//button[@id="mat-button-toggle-29"]`<br>**_Материал несущих стен -  Кирпич или монолит_** <br>`//button[@id="mat-button-toggle-37"]`<br>**_Материал несущих стен -  Дерево_** <br>`//button[@id="mat-button-toggle-38"]`<br>**_Применить_** <br> `//button[@id="mat-focus-indicator action-back mat-stroked-button mat-button-base"]`<br>
## **Поля для ввода текста** <br> 
**_Регион проживания(селект)_** <br> `//input[@id="mat-input-0"]`<br> **_Срок действия страхования(датапикер)_** <br> `//input[@id="mat-input-1"]`<br> **_Сумма(слайдер)_** <br> `//input[@id="mat-input-3"]`<br> **_Промокод_** <br> `//input[@id="mat-input-2"]`<br> 
## **Датапикеры** <br>
**_Дата начала действия страхования_** <br> `//mat-datepicker[@class="mat-datepicker-toggle ng-tns-c61-22"]`<br> **_Срок действия страхования_** <br> `//input[@id="mat-input-1"]` <br>
## **Логотип СберСтрахование** <br>
`//div[@class="sber-logo"]`<br>
## **Слайдер в блоке выбора суммы** <br>
`//div[@class="mat-slider-wrapper"]`<br> OR <br> `//mat-slider`
## **Хедер "Что будет застраховано?"** <br>
`//div[class="sbi-form__rov ng-star-inserted"]/div[2]`<br>
## **Тестовые блоки** <br>
**_Мебель, техника и ваши вещи_** <br> `//div[text()[contains(.,'Мебель, техника и ваши вещи')]]`<br> **_Падение летательных аппаратов и их частей_** <br> `//div[text()[contains(.,'Падение летательных аппаратов и их частей')]]`<br>
## **Колонки списка под хейдером "Страховая защита включенная в программу"** <br>
**_Колонка 1_** <br> `//div[text()='Чрезвычайная ситуация']/ancestor::ul`<br> **_Колонка 2_** <br> `//div[text()='Стихийные бедствия']/ancestor::ul`<br>

---
---


# 2. Оформление <br> 
## Кнопки <br> 
Заполнить по Сбер ID <br> `//*[@class="mat-focus-indicator sber-id-button mat-flat-button mat-button-base mat-primary"]` <br> 
Мужской <br> `//*[@id="mat-button-toggle-76-button"]` <br> Женский <br> `//*[@id="mat-button-toggle-77-button"]` <br> 
Вернуться <br> `//*[@class='mat-focus-indicator action-back mat-stroked-button mat-button-base']` <br> 
Оформить <br> `//*[@class='mat-focus-indicator mat-flat-button mat-button-base mat-accent']` <br>  
## Поля для ввода текста <br> 
Фамилия <br> `//*[@id="mat-input-25"]` <br> Имя <br> `//*[@id="mat-input-26"]` <br> Отчество <br> `//*[@id="mat-input-27"]` <br> Дата рождения <br> `//*[@id="mat-input-28"]` <br> Серия <br> `//*[@id="mat-input-29"]` <br> Номер <br> `//*[@id="mat-input-30"]` <br> Дата выдачи <br> `//*[@id="mat-input-31"]` <br> Кем выдан <br> `//*[@id="mat-input-32"]` <br> Код подразделения <br> `//*[@id="mat-input-33"]` <br> Регион <br> `//*[@id="mat-input-34"]` <br> Город или населенный пункт <br> `//*[@id="mat-input-35"]` <br> Улица <br> `//*[@id="mat-input-36"]` <br> Дом, литера, корпус, строение <br> `//*[@id="mat-input-37"]` <br> Квартира <br> `//*[@id="mat-input-38"]` <br> Телефон <br> `//input[@type="phone"]` <br> Электронная почта <br> `//*[@id="mat-input-19"]` <br> Повтор электронной почты <br> `//*[@id="mat-input-20"]` <br> 
## Чекбоксы <br> 
Отчество отсутствует <br> `//*[@id="mat-checkbox-1"]/label/div` <br>
Улица отсутствует <br> `//*[@id="mat-checkbox-2"]/label/div` <br>
## Датапикеры <br> 
Дата рождения <br> `//mat-datepicker[@class="ng-tns-c61-6"]` <br>  
Дата выдачи <br> `//mat-datepicker[@class='ng-tns-c61-9']` <br>
## Логотип <br>
"СБЕР СТРАХОВАНИЕ" <br> `//div[@class="sber-logo"]` <br>  
## Текстовые блоки <br>                       
Страхователь <br> `//*[@class="contact-form__insurant-title block-header"]` <br> Паспортные данные Страхователя <br> `//*[@class="contact-form__passport-title block-header"]` <br> Адрес имущества <br> `//*[@class="contact-form__address-title block-header"]` <br> Контактные данные Страхователя <br> `//*[@class="contact-form__contact-title block-header"]` <br> Обратите особое внимание: на указанную электронную почту будет выслан ваш договор! Указывайте только тот адрес, которым Вы пользуетесь. <br> `//*[@class="contact-form__contact-item info"]` <br> Футер: ООО СК «Сбербанк страхование». Лицензии Банка России: СИ № 4331 выдана 12.10.2020 бессрочно, СЛ № 4331 выдана 12.10.2020 бессрочно, ПС № 4331 выдана 12.10.2020 бессрочно, ОС № 4331 – 05 выдана 12.10.2020 бессрочно, ОС № 4331 – 04 выдана 12.10.2020 бессрочно, ОС № 4331-03 выдана 10.06.2021 бессрочно. <br> `//*[@id="footer"]/div` или `//*[@class="footer__content"]`
