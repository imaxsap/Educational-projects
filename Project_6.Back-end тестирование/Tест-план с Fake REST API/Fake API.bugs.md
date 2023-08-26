Project 07, exercise 2<br>by postwoman  

# Баг-репорты набора тест-кейсов для проверки всех эндпоинтов в Fake REST API  

## $`\textcolor{blue}{\text{Баг №1. Удаление несуществующей активности {id 31}}}`$  

**Предшествующие условия:**  
- `Пользователь находится в разделе Activities сайта https://fakerestapi.azurewebsites.net/index.html`   
- `Выбран необходимый метод HTTP-запроса`     

**Серьезность:**   
- `Trivial`

**Шаги воспроизведения:**  

- `1. Отправить запрос Delete/api​/v1​/Activities​/{31}`  

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Found`  

**Фактический результат:**   
- `Код фактический: 200 ОК`  

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`  

## $`\textcolor{blue}{\text{Баг №2. Удаление несуществующей активности {id 0}}}`$

**Предшествующие условия:**  
- `Пользователь находится в разделе Activities сайта https://fakerestapi.azurewebsites.net/index.html`   
- `Выбран необходимый метод HTTP-запроса`     

**Серьезность:**   
- `Trivial`

**Шаги воспроизведения:**  

- `1. Отправить запрос Delete/api​/v1​/Activities​/{0}`  

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Found`  

**Фактический результат:**   
- `Код фактический: 200 ОК`  

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`    

## $`\textcolor{blue}{\text{Баг №3. Получение данных об авторе {id 012}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе Authors сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**     
- `Minor`  

**Шаги воспроизведения:**   
- `Отправить запрос GET​/api​/v1​/Authors​/{012}`    

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Foud`    
- `Тело JSON ожидаемый результат: в теле отображается код ошибки 404 Not Foud`    

**Фактический результат:**    
- `Код фактический: 200 ОК`   
- `Тело JSON фактический результат:`
```
{
  "id": 12,
  "idBook": 4,
  "firstName": "First Name 12",
  "lastName": "Last Name 12"
}
```   
**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`  

## $`\textcolor{blue}{\text{Баг №4. Получение данных о книге {id 0}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе Authors сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**     
- `Minor`  

**Шаги воспроизведения:**   
- `Отправить запрос GET​/api​/v1​/authors​/books​/{0}`    

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Foud`    
- `Тело JSON ожидаемый результат: в теле отображается код ошибки 404 Not Foud`    

**Фактический результат:**    
- `Код фактический: 200 ОК`   
- `Тело JSON фактический результат:`
```
[]
```   
**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`    

## $`\textcolor{blue}{\text{Баг №5. Получение данных о книге {id 1}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе Authors сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**     
- `Critical`  

**Шаги воспроизведения:**   
- `Отправить запрос GET​/api​/v1​/authors​/books​/{1}`    

**Ожидаемый результат:**   
- `Тело JSON ожидаемый результат:`    
```
Тело JSON ожидаемый результат:

{
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  },
  {
    "id": 2,
    "idBook": 1,
    "firstName": "First Name 2",
    "lastName": "Last Name 2"
  },
  {
    "id": 3,
    "idBook": 1,
    "firstName": "First Name 3",
    "lastName": "Last Name 3"
  },
  {
    "id": 4,
    "idBook": 1,
    "firstName": "First Name 4",
    "lastName": "Last Name 4"
  }
  ```

**Фактический результат:**    
- `Тело JSON фактический результат:`
```
{
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  },
  {
    "id": 2,
    "idBook": 1,
    "firstName": "First Name 2",
    "lastName": "Last Name 2"
  },
  {
    "id": 3,
    "idBook": 1,
    "firstName": "First Name 3",
    "lastName": "Last Name 3"
  }
```   
**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`   

## $`\textcolor{blue}{\text{Баг №6. Получение данных о книге {id 201}}}`$      

**Предшествующие условия:**    
- `Пользователь находится в разделе Authors сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Minor`   

**Шаги воспроизведения:**    
- `GET​/api​/v1​/authors​/books​/ {201}`     

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Foud`    
- `Тело JSON ожидаемый результат: в теле отображен код 404 Not Foud`   

**Фактический результат:**    
- `Код фактический: 200 OK`   
- `Тело JSON фактический результат: []`    

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`   

## $`\textcolor{blue}{\text{Баг №7. Получение данных о книге {id 012}}}`$     

**Предшествующие условия:**     
- `Пользователь находится в разделе Authors сайта https://fakerestapi.azurewebsites.net/index.html`       
- `Выбран необходимый метод HTTP-запроса`        

**Серьезность:**   
- `Minor`   

**Шаги воспроизведения:**    
- `GET​/api​/v1​/Authors​//books​/{012}`   

**Ожидаемый результат:**     
- `Код ожидаемый: 404 Not Foud`    
- `Тело ожидаемый результат: в теле отображается код ошибки 404 Not Foud`   

**Фактический результат:**    
- `Код фактический: 200 ОК`   
- `Тело JSON фактический результат:
```
  {
    "id": 35,
    "idBook": 12,
    "firstName": "First Name 35",
    "lastName": "Last Name 35"
  },
  {
    "id": 36,
    "idBook": 12,
    "firstName": "First Name 36",
    "lastName": "Last Name 36"
  }
```
**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`  

## $`\textcolor{blue}{\text{Баг №8.Удаление списка автора {id 0}}}`$ 
    
**Предшествующие условия:**    
- `Пользователь находится в разделе Authors сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Trivial`   

**Шаги воспроизведения:**    
- `Отправить запрос Delete/api​/v1​/Authors/{0}`     

**Ожидаемый результат:**  
- `Код ожидаемый: 404 Not Found` 

**Фактический результат:**    
- `Код фактический: 200 ОК`

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`    

## $`\textcolor{blue}{\text{Баг №9.Удаление списка автора {id 700}}}`$ 

**Предшествующие условия:**    
- `Пользователь находится в разделе Authors сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`  

**Серьезность:**  
- `Trivial`   

**Шаги воспроизведения:**    
- `Отправить запрос Delete/api​/v1​/Authors/{0}`     

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Found`

**Фактический результат:**    
- `Код фактический: 200 ОК`

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)` 

## $`\textcolor{blue}{\text{Баг №10. Получение данных о книге {id 1}}}`$       

**Предшествующие условия:**    
- `Пользователь находится в разделе Books​ сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Major`   

**Шаги воспроизведения:**    
- `Отправить запрос GET​/api​/v1​/Books​/{1}`  

**Ожидаемый результат:**   
- `Тело JSON:` 
```
{
    "id": 1,
    "title": "Book 1",
    "description": "At luptatum sed eu tempor dolore nulla clita voluptua eirmod accumsan. Vel takimata lobortis eos amet no adipiscing magna eos. Dolore dolor dignissim vero.\n",
    "pageCount": 100,
    "excerpt": "Diam rebum et est consetetur nonumy nihil consetetur. Voluptua magna soluta voluptua ut et sed labore dolores et elitr gubergren volutpat dolore sed. Eros eu erat. Voluptua no diam vero vel ut vel duo ex sadipscing ea. Gubergren vero vero iriure et sanctus magna tempor ipsum stet cum exerci dolores dolor.\nSadipscing tempor consequat takimata duo sed diam dolores ipsum euismod vulputate facilisi stet gubergren ex. Velit sed adipiscing nonumy in dolores invidunt odio sit. Amet rebum invidunt et sea eirmod et ea at volutpat takimata facilisi voluptua dolor justo accusam sea. Et exerci vero hendrerit consetetur clita vel justo dolor hendrerit nisl at. Ea at gubergren in diam exerci et volutpat blandit et feugiat ut tempor lorem. Facilisi et illum diam elitr dolore nonumy elitr invidunt facilisis et kasd et eirmod in tempor. Lorem et hendrerit et dolores dolore amet nostrud. Dolor veniam sadipscing. Et sea stet cum nulla rebum lorem ipsum soluta sit voluptua vel eos. Accusam dolores amet ipsum diam erat eos ut ipsum sea et in est esse. Dolores nulla quod erat ut blandit clita lorem. Sadipscing voluptua gubergren vero et magna et. Sadipscing sea erat clita gubergren ipsum amet.\nMolestie est sanctus dignissim diam gubergren tempor tincidunt ut accusam dolor stet kasd zzril. Tempor labore vulputate sit diam enim esse nisl sed et ipsum minim takimata eos sea ut sanctus est. Magna takimata sadipscing erat ipsum dolores erat nonummy magna at elit accusam kasd nonummy. Et et eos. Eu erat et dolores ea et voluptua wisi. Aliquyam sed vel. Sea sea dolore sit diam lorem lorem et dolores invidunt elitr diam facilisis. Velit dolore velit sanctus sit erat lorem takimata ut lorem nostrud sed. Sea accusam lorem dolores et sit stet. Dolor dolor justo. Ut dolor ex rebum consectetuer accumsan consequat takimata gubergren sea sed. At dolore dolor elitr magna vero amet tation duo ea sea.\nVolutpat justo justo est ea. Consequat enim euismod wisi illum erat elitr labore at velit. Erat dolor velit. No sadipscing amet aliquyam gubergren veniam et consetetur magna justo ut vero. Et et ut ipsum dolore vero kasd amet lorem aliquyam ea accumsan sed labore tation tempor consequat invidunt. Sanctus dolore eros aliquyam et voluptua nonumy justo at ut vel imperdiet dolore vel. Justo aliquam et amet duo sed diam te gubergren erat gubergren aliquyam eirmod voluptua. Diam soluta et amet dolores consequat justo facer kasd. Sed est suscipit accusam vero commodo magna ipsum dolores ipsum tempor sit kasd dolor aliquyam aliquyam justo.\nRebum et vulputate minim accusam et elitr at. Tempor feugait veniam. Sea quod diam eos accusam est dignissim imperdiet diam elitr wisi eos ad lorem sanctus dolore ipsum. Eu lobortis est magna takimata consequat kasd adipiscing eos illum nonumy consectetuer et no aliquam sanctus vero. At vero accumsan eu amet nonumy eos facilisis sadipscing hendrerit nonumy dolore invidunt diam diam sanctus. Takimata sea aliquyam. Amet eum velit et vero lobortis diam accusam takimata duo at dolores assum sed vero dolor. At luptatum vero at elitr accusam doming eu sit elitr iriure ea et ad augue sadipscing dolores. Sanctus et labore nisl ex zzril hendrerit invidunt et ipsum consetetur.\n",
    "publishDate": "2023-06-19T07:53:05.6320947+00:00"
  }
  ```

**Фактический результат:**  
- `Тело JSON:`  
```
{
  "id": 1,
  "title": "Book 1",
  "description": "Consequat dolor eros dolores ipsum ea labore iriure et rebum iusto sit sit sea dolor clita dolores. Ea amet diam sed justo aliquam et sea lorem invidunt ad. Nonumy ipsum accusam amet dolore at nonumy consequat. Kasd voluptua consectetuer. Ut dolor et dolor nulla. Gubergren sed et volutpat sadipscing lorem sed soluta lorem amet exerci no ipsum dolore vel at et. Est dolor diam. Nobis mazim est sed et nulla duo dignissim velit voluptua kasd lorem lobortis et vero invidunt sed molestie. Eos ut nonumy justo ipsum diam tempor vero at dolore tempor sit. Labore tempor diam molestie ad sit dolore volutpat dolor dolor nam dolor ipsum amet eum. Dolor et sit ipsum dolores stet tempor stet lorem volutpat rebum. Erat ipsum dolor accusam erat magna. Luptatum sanctus est sed exerci esse dolores vulputate commodo eleifend molestie lorem sed takimata tincidunt vel eu vel et. Nonumy amet consectetuer ut elitr accumsan sadipscing ipsum nihil autem ut takimata dolores. Magna gubergren sed voluptua sea et amet eos lobortis clita ut amet invidunt gubergren diam takimata sanctus vel invidunt. Dolor dolore in et option labore amet duo consetetur ipsum ea ipsum. Consetetur diam dolor sanctus odio sea no vel luptatum no ut ut veniam assum et sea velit.\n",
  "pageCount": 100,
  "excerpt": "Odio iriure takimata dolore qui molestie sit diam et dolore nulla aliquip. Justo clita elitr et tation dolor duo amet autem gubergren erat. Accusam invidunt eirmod rebum clita gubergren et eu magna vero. Liber quis eu ipsum consetetur magna eirmod minim dolor stet lorem dolores amet. Lorem ut in vero nonumy voluptua ut erat nonummy vel ut. Stet sadipscing et et eos illum at ipsum suscipit aliquyam vero ipsum vero rebum elitr. Diam esse dolores qui iusto dolores delenit voluptua labore est elitr vel. Voluptua dolore sit sit invidunt justo consetetur at id in. Gubergren imperdiet sed dolor gubergren hendrerit labore in duo tempor. Takimata aliquyam consequat ipsum amet facilisis dolor at sit sea diam aliquyam nonumy sanctus vero dolor.\nDolor voluptua consequat dolor ipsum consetetur gubergren at justo lorem enim. Et dolore accusam sea voluptua et clita praesent vero duo consetetur eirmod nonumy iriure magna et diam takimata consequat. Amet lorem possim sea ipsum no luptatum sed voluptua ipsum tation feugiat diam. Feugait takimata gubergren stet et ipsum kasd. Volutpat rebum ea sit no ut accumsan diam erat adipiscing duis et dolor labore sed.\nEt lorem erat elitr possim suscipit ad kasd sadipscing et stet takimata. Diam blandit feugiat sanctus consequat nibh amet diam sit et enim congue sed. Ipsum ipsum accusam nibh sed et magna magna ipsum dolore ea magna vero accusam ut duis eos. Hendrerit duo lorem consetetur nostrud hendrerit liber volutpat volutpat amet ea est magna exerci.\nGubergren odio nonumy nostrud sit elitr augue sit qui zzril. Et ipsum at est dolor amet et gubergren vero feugait no magna duis et sadipscing praesent ea. Consetetur ut accusam consequat consetetur kasd ipsum iriure ex dolor magna nonumy exerci sadipscing no dolor nonumy erat iriure. Stet est sea nobis elitr ut duo euismod tation nulla elitr ullamcorper rebum aliquyam nibh aliquyam lorem. Elitr rebum diam euismod magna at stet. Invidunt duis est diam eu nulla at diam lorem nonumy diam et no gubergren sadipscing et eirmod kasd et. At vero dolores nulla quod tation diam eu est suscipit. Lorem sit sea illum ipsum et accusam. Dolore dolor gubergren. In tempor et et. Accusam duo eirmod lorem sea et no eros dolore laoreet in sadipscing ut quis.\nLorem imperdiet duo sit sadipscing sea molestie et ut tempor accusam. Praesent dolor minim feugait dolore sed ut lorem duo eirmod sea sit dolore sea. Stet kasd praesent duo accusam at sed diam dolore et at. Eum option accusam duo. Voluptua facilisis at nisl rebum duo sed esse diam sed amet gubergren hendrerit lorem. Ut eirmod vero tincidunt ipsum qui lorem dignissim takimata ut eirmod feugait sea eirmod minim ut veniam et molestie. Molestie et duo amet sadipscing magna consequat ex duis sed erat ut kasd est laoreet sea at. Et vel eos no. Aliquyam gubergren eum et duis diam vero vel sed blandit. Amet ipsum accusam sea magna delenit diam enim tempor erat. Molestie amet ipsum molestie aliquip ipsum dolore lorem invidunt duo at delenit accusam nonumy amet justo dolor iusto. Sadipscing labore aliquip facilisis et lorem tempor et consequat magna erat vero et takimata. Iusto no praesent et elitr et dolor invidunt luptatum consectetuer et aliquam amet justo enim kasd sadipscing. Minim dolor takimata tempor lorem congue magna ad luptatum dolores ipsum in duis takimata takimata ut duo diam. Ad ea dolores elitr dolores ut dolor et luptatum tempor ipsum tempor et invidunt erat tincidunt sanctus sed. Sanctus lorem labore feugait te labore soluta diam et. Lorem stet sit magna feugait eros delenit duis gubergren in invidunt takimata vel. Iriure dolore aliquyam euismod lorem et facilisis dolor sanctus. Ut dolor diam est at at dolore amet diam sit.\n",
  "publishDate": "2023-06-19T07:45:16.8557293+00:00"
}
```    

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`   

## $`\textcolor{blue}{\text{Баг №11. Удаление данных о книге {id 201}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе Books сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Critical`   

**Шаги воспроизведения:**      
- `Отправить запрос Delete/api​/v1​/Books/{201}`      

**Ожидаемый результат:**    
- `Код ожидаемый: 404 Not Found`     

**Фактический результат:**      
- `Код фактический: 200 ОК`       

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`   

## $`\textcolor{blue}{\text{Баг №12. Удаление данных о книге {id 0}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе Books сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Critical`   

**Шаги воспроизведения:**     
- `Отправить запрос Delete/api​/v1​/Books/{0}`      

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Found`     

**Фактический результат:**     
- `Код фактический: 200 ОК`        

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`   

## $`\textcolor{blue}{\text{Баг №13. Получение данных о фото {id 012}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе CoverPhotos сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Minor`   

**Шаги воспроизведения:**    
- `Отправить запрос GET​/api​/v1​/CoverPhotos​/{012}`     

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Foud`    
- `Тело ожидаемый результат: в теле отображается код ошибки 404 Not Foud`   

**Фактический результат:**    
- `Код фактический: 200 ОК`    
- `Тело JSON фактический результат:`
```
{
  "id": 12,
  "idBook": 12,
  "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 12&w=250&h=350"
}
```    

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`   

## $`\textcolor{blue}{\text{Баг №14. Получение данных о фото {id 201}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе CoverPhotos сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Critical`   

**Шаги воспроизведения:**    
- `Отправить запрос GET​/api​/v1​/CoverPhotos/books/covers​/{201}`     

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Foud`    
- `Тело JSON ожидаемый результат: в теле отображен код 404 Not Foud`   

**Фактический результат:**     
- `Код фактический: 200 ОК`    
- `Тело JSON фактический результат: []`    

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`  

## $`\textcolor{blue}{\text{Баг №15. Получение данных о фото {id 0}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе CoverPhotos сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Critical`   

**Шаги воспроизведения:**    
- `Отправить запрос GET​/api​/v1​/CoverPhotos/books/covers​​/{0}`     

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Foud`    
- `Тело JSON ожидаемый результат: в теле отображен код 404 Not Foud`   

**Фактический результат:**    
- `Код фактический: 200 ОК`    
- `Тело JSON фактический результат: []`    

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`   

## $`\textcolor{blue}{\text{Баг № 16. Получение данных о фото книги {id 012}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе CoverPhotos сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Minor`   

**Шаги воспроизведения:**    
- `Отправить запрос GET​/api​/v1​/CoverPhotos/books/covers​​/​/{012}`     

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Foud`    
- `Тело ожидаемый результат: в теле отображается код ошибки 404 Not Foud`   

**Фактический результат:**    
- `Код фактический: 200 ОК`    
- `Тело JSON фактический результат:`
```
  {
    "id": 12,
    "idBook": 12,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 12&w=250&h=350"
  }
  ```    

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`   

## $`\textcolor{blue}{\text{Баг №17. Удаление списка фото {id 201}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе CoverPhotos сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Trivial`   

**Шаги воспроизведения:**    
- `Отправить запрос Delete/api​/v1​/CoverPhotos/{201}`     

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Found`       

**Фактический результат:**    
- `Код фактический: 200 ОК`       

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)`   

## $`\textcolor{blue}{\text{Баг №18. Удаление списка фото {id 0}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе CoverPhotos сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Trivial`   

**Шаги воспроизведения:**    
- `Отправить запрос Delete/api​/v1​/CoverPhotos/{0}`     

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Found`       

**Фактический результат:**    
- `Код фактический: 200 ОК`       

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)` 

## $`\textcolor{blue}{\text{Баг №19. Удаление списка пользователей {id 11}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе Users сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Trivial`   

**Шаги воспроизведения:**    
- `Отправить запрос Delete/api​/v1​/Users/{11}`     

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Found`       

**Фактический результат:**    
- `Код фактический: 200 ОК`       

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)` 

## $`\textcolor{blue}{\text{Баг №20. Удаление списка пользователей {id 0}}}`$    

**Предшествующие условия:**    
- `Пользователь находится в разделе Users сайта https://fakerestapi.azurewebsites.net/index.html`     
- `Выбран необходимый метод HTTP-запроса`       

**Серьезность:**  
- `Trivial`   

**Шаги воспроизведения:**    
- `Отправить запрос Delete/api​/v1​/Users/{0}`     

**Ожидаемый результат:**   
- `Код ожидаемый: 404 Not Found`       

**Фактический результат:**    
- `Код фактический: 200 ОК`       

**Окружение:**   
- `Браузер Google Chrome, Версия 114.0.5735.134 (Официальная сборка), (64 бит)` 


















