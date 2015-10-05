# HTML, II часть

- [Интерактивные элементы](part-2.md#%D0%98%D0%BD%D1%82%D0%B5%D1%80%D0%B0%D0%BA%D1%82%D0%B8%D0%B2%D0%BD%D1%8B%D0%B5-%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-)
    - [Ссылочные элементы – a](part-2.md#%D0%A1%D1%81%D1%8B%D0%BB%D0%BE%D1%87%D0%BD%D1%8B%D0%B5-%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B--a-)
        - [Атрибут href, URL](part-2.md#Атрибут-href-url-)
        - [DNS](part-2.md#dns-)
        - [Абсолютные ссылки, относительные, ссылки на скачивание и якоря](part-2.md#Абсолютные-ссылки-относительные-ссылки-на-скачивание-и-якоря-)
        - [MIME](part-2.md#mime-)
    - [Элементы форм – form, input, select, ... ](part-2.md#Элементы-форм--form-input-select--)
    - [Элементы встраиваемого содержимого – audio, iframe, img, svg, video, ...] (part-2.md#%D0%AD%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-%D0%B2%D1%81%D1%82%D1%80%D0%B0%D0%B8%D0%B2%D0%B0%D0%B5%D0%BC%D0%BE%D0%B3%D0%BE-%D1%81%D0%BE%D0%B4%D0%B5%D1%80%D0%B6%D0%B8%D0%BC%D0%BE%D0%B3%D0%BE--audio-iframe-img-svg-video--)    
- [Глобальные атрибуты](part-2.md#%D0%93%D0%BB%D0%BE%D0%B1%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5-%D0%B0%D1%82%D1%80%D0%B8%D0%B1%D1%83%D1%82%D1%8B-)
- [Семантическая разметка](part-2.md#%D0%A1%D0%B5%D0%BC%D0%B0%D0%BD%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B0%D1%8F-%D1%80%D0%B0%D0%B7%D0%BC%D0%B5%D1%82%D0%BA%D0%B0-)
    - [HTML5](part-2.md#html5)
    - [Scheme.org](part-2.md#schemaorg)
    - [Микроформаты](part-2.md#Микроформаты)
-  [Интернационализация](part-2.md#%D0%98%D0%BD%D1%82%D0%B5%D1%80%D0%BD%D0%B0%D1%86%D0%B8%D0%BE%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F-)
    - [Кодировка](part-2.md#%D0%9A%D0%BE%D0%B4%D0%B8%D1%80%D0%BE%D0%B2%D0%BA%D0%B0-)
    - [Язык](part-2.md#%D0%AF%D0%B7%D1%8B%D0%BA-)
    - [Направление текста](part-2.md#%D0%9D%D0%B0%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D1%82%D0%B5%D0%BA%D1%81%D1%82%D0%B0-)
    - [Переводимость текста](part-2.md#%D0%9F%D0%B5%D1%80%D0%B5%D0%B2%D0%BE%D0%B4%D0%B8%D0%BC%D0%BE%D1%81%D1%82%D1%8C-%D1%82%D0%B5%D0%BA%D1%81%D1%82%D0%B0-)
    - [Слияемость текста](part-2.md#%D0%A1%D0%BB%D0%B8%D1%8F%D0%B5%D0%BC%D0%BE%D1%81%D1%82%D1%8C-%D1%82%D0%B5%D0%BA%D1%81%D1%82%D0%B0-)
- [Тип HTML документа](part-2.md#%D0%A2%D0%B8%D0%BF-html-%D0%B4%D0%BE%D0%BA%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%B0-)
    - [Doctype](part-2.md#doctype-)
    - [Document Type Definition](part-2.md#document-type-definition-)    
    - [Doctype для HTML 5](part-2.md#doctype-%D0%B4%D0%BB%D1%8F-html-5-)
- [Ссылки](part-2.md#%D0%A1%D1%81%D1%8B%D0%BB%D0%BA%D0%B8-)

## Интерактивные элементы [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

### Ссылочные элементы – a [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [a](https://webref.ru/html/a) (anchor) является основой любого HTML
документа. Он позволяет связать HTML документы и другие ресурсы сети друг с
другом, образуя сеть всемирной паутины. Ссылки очень гибкий элемент и имеет
много разновидностей.

Например, ссылки могут вести на другой HTML документ в сети:

```html
<a
    href="http://home.web.cern.ch/"
    hreflang="en"
    target="_blank"
    title="Официальный сайт CERN">
    CERN
</a>
```
[demo](http://codepen.io/anon/pen/BodoeL?editors=100)

Или на файл для скачивания:

```html
<a
    href="https://whatwg.org/pdf"
    download
    type="application/pdf">
    Спецификация HTML5
</a>  
```
[demo](http://codepen.io/anon/pen/BodoeL?editors=100)

Или на электронную почту:

```html
<a href="mailto:press.office@cern.ch">Написать нам письмо</a>
```
[demo](http://codepen.io/anon/pen/BodoeL?editors=100)

И даже на номер телефона:

```html
<a href="tel:+41 (0)22 767 2757">Или позвонить</a>  
```
[demo](http://codepen.io/anon/pen/BodoeL?editors=100)

#### Атрибут href, URL [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Самый важный атрибут ссылки – `href` (hyperlink reference). Он задаёт собственно
ссылку на другой документ или ресурс. В качестве значения атрибута используется
*URL (Uniform Resource Locator)* – единообразный указатель (адрес) ресурса в
сети Интернет.

```
https://yandex.ru/support/search
```

Любой URL состоит из двух частей: метод доступа к ресурсу `https` и
адрес ресурса `//yandex.ru/support/search`, разделённые двоеточием `:`.

**Метод доступа** обычно представляет собой идентификатор протокола, который
определяет какая программа будет обрабатывать событие нажатия на ссылку.

Протокол | Пример | Приложение | Действие
---- | ---- | ---- | ----
http | http://yandex.ru/support/search | Браузер | Загрузит новый HTML документ по протоколу HTTP (HyperText Transfer Protocol)
https | https://yandex.ru/support/search |Браузер | Загрузит новый HTML документ по защищённому протоколу HTTPS (HyperText Transfer Protocol Secure)
mailto | mailto:press.office@cern.ch | Почтовый клиент | Откроет форму создания письма
skype | skype:i-dont-like-skype | Skype | Откроет чат с пользователем
tel | tel:+43-000-00-000-00 | Skype | Попробует позвонить абоненту по номеру
file | file://home/Users/gogoleff/.zshrc | Браузер | Попробует открыть файл на вашем компьютере локально

Протокол *http* является протоколом по умолчанию и его можно не указывать.

Метод доступа определяет формат **адреса ресурса**:

Протокол |  Пример | Формат
---- | ---- | ----
mailto | mailto:press.office@cern.ch | Aдрес электронной почты
skype | skype:i-dont-like-skype | Логин пользователя
tel | tel:+43-000-00-000-00 | Номер телефона
file | file://home/Users/gogoleff/.zshrc | Абсолютный путь до файла (начиная с корня)
http, https | https://yandex.ru/support/search | Адрес HTML документа в сети интернет

Разберём адрес HTML документа в сети интернет чуть подробнее. Полный формат
выглядит так:

```
https://<логин>:<пароль>@<хост>:<порт>/<путь>?<параметры>#<якорь>
```

Например:

```
https://gogolef:123456@yandex.ru:443/search?text=метрика#results
```
Параметр | Пример | Назначение
---- | ---- | ----
<логин> | gogolef | Имя пользователя для доступа к ресурсу (если необходимо)
<пароль> | 123456 | Пароль для доступа к ресурсу (если необходим)
<хост> | yandex.ru | Доменное имя сервера (Domain Name), где расположен ресурс
<порт> | 443 | Номер порта по которому доступен ресурс. По умолчанию, 80 для HTTP и 443 для HTTPS – если так, его можно не указывать. На одном и том же сервере по разным портам можно получать разные ресурсы.
<путь> | /search | Путь до ресурса. В примере, форма поиска по Интернету. Это может быть HTML страницы или файл
<параметры> | text=метрика | Параметры доступа к ресурсу. В примере, запрос «метрика» в форму поиска.
<якорь> | results | Прокрутить страницу до элемента с id="results"

Мы немного коснулись темы доменных имён, рассмотрим их чуть подробнее.

#### DNS [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

*Доменное имя или домен (Domain Name)*– это уникальное виртуальное имя сервера в
сети Интернет в рамках *DNS (Domain Name System)*. *DNS* –  компьютерная
распределённая система для получения физического адреса сервера (IP-адреса) в
сети Интернет по виртуальному и **человеко-понятному** адресу (доменному имени).

Таблицы соответствий IP-адреса домену хранятся на специальных DNS-серверах по
всему миру. Условно они выглядят так:

```
yandex.ru       77.88.55.66
wikipedia.org   91.198.174.192
```

Когда вы в браузере набираете `yandex.ru`, то он в **первую очередь** cпрашивает
DNS-сервера и получает от них в ответ IP-адрес `77.88.55.66`. Затем у сервера
с этим IP-адресом браузер уже запрашивает HTML документ.

Доменные имена позволяют запрашивать ресурсы сети интернет в человеко-понятном
виде, а также размещать сразу несколько ресурсов на одном сервере (с одним IP).
Сервер по доменному имени сам поймёт какой ресурс отдать пользователю:

```
yandex.ru               77.88.55.66
my-awesome-site.ru      77.88.55.66
```

#### Абсолютные ссылки, относительные, ссылки на скачивание и якоря [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Все ссылки с протоколом http можно разделить на четыре вида.

- Абсолютные ссылки `href="http://yandex.ru/support/search"` или
  `href="//yandex.ru/support/search"` – обязательно содержат <хост>. Если
  протокол не указан, будет использован протокол текущего документа.

- Относительные ссылки `href="/support/search"` – в качестве <хост> использует
  доменное имя текущего документа.

- Якоря `href="#result"` – при клике прокручивают до элемента (переходят к
  элементу) с id равным идентификатору, указанном после `#`.

- Ссылки на скачивание `<a href="https://whatwg.org/pdf" download>` – задаются
  при помощи атрибута `download`. Он указывает браузеру, что документ необходимо
  именно скачать, а не показать (а современные браузеры умеют показывать даже PDF).
  С помощью атрибута `type` можно подсказать браузеру и пользователю MIME-тип
  скачиваемого файла `type="application/pdf"`.

  Например, можно добавить к нему иконоку в CSS стилях:

  ```css
  a[type=application/pdf]
  {
      background: url(pdf-icon.png);
  }
  ```
  [demo](http://codepen.io/anon/pen/pjrbvy)

  <img width="184" alt="2015-10-12_0130" src="https://cloud.githubusercontent.com/assets/4534405/10418897/e2d85d8c-7080-11e5-9827-a251a0baef0f.png">


#### MIME [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

*MIME-тип* – идентификатор типа файла согласно спецификации *MIME (Multipurpose
Internet Mail Extensions)* – стандарт,
[описывающий](https://tools.ietf.org/html/rfc2046) передачу различных типов
данных (изначально для передачи в тексте почтовых сообщений).

Идентификатор MIME имеет следующий формат:

```
<базовый тип>/<тип>
```

Например,

```sh
application/zip     # Архив zip
application/pdf     # PDF файл
audio/mpeg          # mp3 аудио файл
image/jpeg          # Картинка в jpeg формате
text/css            # Файл с CSS стилями
video/mp4           # mp4 видео файл
```

Различают следующие базовые типы:

Тип | Описание
---- | ----
application | Прикладные программы
audio | Аудио файлы
image | Изображения
message | Текстовый сообщения
model | 3D модели
multipart | Несколько типов файлов в одном
text | Текстовый файлы
video | Видео файлы

[Посмотреть список MIME-типов](https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_MIME-%D1%82%D0%B8%D0%BF%D0%BE%D0%B2).

### Элементы форм – form, input, select, ... [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Если нам необходимо не только давать пользователь информацию, но и принимать
информацию от него, то есть взаимодействовать с ним, то понадобится группа
элементов для описания форм.

#### form [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Форма [form](http://webref.ru/html/form) представляет собой набор элементов для
ввода информации и кнопок для различных действий с этой иноформацией, чаще всего
для отправки её на сервер.

Например, форма редактирования данных о книге «Война и мир»:

```html
<form action="/book/war-and-peace" method="POST">
    <!-- Поле для ввода заголовка книги -->
    <!-- Так как мы редактируем, то заголовок уже предустановлен в поле -->
    <input name="title" value="Война и мир">

    <!-- Поле для ввода автора книги -->
    <input name="author" value="Толстой Л.Н.">

    <!-- Кнопка сохранения -->
    <!-- При нажатии на неё, браузер соберёт все данные и отправит по адресу /book/war-and-peace -->
    <button type="submit">Сохранить</button>
<form>
```
[demo](http://codepen.io/anon/pen/LpjbeL)

В данной форме мы видим два поля и одну кнопку. Данные формы отправляются по
нажатию кнопки с атрибутом и значением `type="submit"`, либо по нажатии клавиши
ENTER. Что при этом произойдёт?

1. Браузер соберёт все введённые в поля данные в объект. Для этого из атрибута
   `name` он возьмёт название поля, а из `value` – значения:

   ```js
   {
       title: 'Война и мир',
       author: 'Толстой Л.Н.'
   }
   ```    

2. Затем он запакует в виде строки текста в формате
   `<поле1>=<значение1>&<поле2>=<значение2>` и специальным образом закодирует
   значения:

   ```text
   title=%D0%92%D0%BE%D0%B9%D0%BD%D0%B0%20%D0%B8%20%D0%BC%D0%B8%D1%80&author=%D0%A2%D0%BE%D0%BB%D1%81%D1%82%D0%BE%D0%B9%20%D0%9B.%D0%9D.
   ```

   Часть символов `a-Z  0-9 - _	. ~` не кодируются. А остальные кодируются при
   помощи *Percent-encoding* – специально механизма кодирования символов в
   в формат `%<номер>`, согласно их номеру в utf-8 (о нём подробнее чуть ниже).

   Например, смотрим в таблице [UTF-8 encoding table](http://www.utf8-chartable.de/unicode-utf8-table.pl?start=1024)
   в колонке `utf-8` номер у буквы `В` – `d0 92` и получам `%D0%92`.

   Подробнее о [Percent-encoding](https://en.wikipedia.org/wiki/Percent-encoding).

3. И на конец, отправит HTTP запрос c закодированными данными по адресу
   `/book/war-and-peace`, указанному в атрибуте 'action'.

У формы есть ещё один важный атрибут – `method`. В нём указан, простыми словами,
**тип действия**, а сложными – метод HTTP протокола.

Так как у ресурса в сети обычно один адрес `/book/war-and-peace` разработчикам
как-то необходимо различать, что мы с ним вообще делаем: просто смотрим, или
редактируем, или удаляем. Для этого и были придуманы методы HTTP протокола.
Вот 4 основных:

Метод | Назначение
---- | ----
GET | Прочитать ресурс
PUT | Создать ресурсу
POST | Отредактировать данные ресурса
DELETE | Удалить ресурс

Например, HTTP запрос вида `DELETE /book/war-and-peace` удаляет книгу.

К сожалению, HTML поддерживает только два метода GET и POST. Остальные эмулируются
при помощи скрытых полей `<input name="http-method" type="hidden" value="DELETE">`.

В нашем пример мы сохраняли (редактировал) данные в существующей книге,   
поэтому использовали значение `method="POST"`.

Вторым важным атрибутом формы является атрибут `enctype`. Он говорит
как кодировать данные:

Значение | Описание
---- | ----
application/x-www-form-urlencoded | Вместо пробелов ставится +, символы кодируются при помощи Percent-encoding.
multipart/form-data | Данные не кодируются. Это значение применяется при отправке файлов.
text/plain | Пробелы заменяются знаком +, буквы и другие символы не кодируются.

Мы уже познакомились с видом кодирования `application/x-www-form-urlencoded`.
Оно используется по умолчанию, поэтому мы его не указали в примере.

```
title=%D0%92%D0%BE%D0%B9%D0%BD%D0%B0%20%D0%B8%20%D0%BC%D0%B8%D1%80&author=%D0%A2%D0%BE%D0%BB%D1%81%D1%82%D0%BE%D0%B9%20%D0%9B.%D0%9D.
```

Кодирование `multipart/form-data` необходимо, когда мы хотим передать
**в одном запросе несколько типов данных**. Например, текстовые данные и файлы.

```html
<form action="/book/war-and-peace" method="POST" enctype="multipart/form-data">
    <input name="title" value="Война и мир">
    <input name="author" value="Толстой Л.Н.">

    <!-- Добавили ещё одно поле – обложка для книги -->
    <!-- Поле типа `file` позволяет выбрать локальный файл -->
    <input name="picture" type="file" value="">

    <button type="submit">Сохранить</button>
<form>
```
[demo](http://codepen.io/anon/pen/ojeYQp?editors=100)

Данные в этом случае будут передаваться как есть, но будут разделены специальными,
случайным образом сгенерированными, разделителями.

```
------WebKitFormBoundarybWhIqSXngmrzkD3q
Content-Disposition: form-data; name="title"

Война и мир
------WebKitFormBoundarybWhIqSXngmrzkD3q
Content-Disposition: form-data; name="author"

Толстой Л.Н.
------WebKitFormBoundarybWhIqSXngmrzkD3q
Content-Disposition: form-data; name="picture"; filename="2015-10-12_0033.png"
Content-Type: image/png

------WebKitFormBoundarybWhIqSXngmrzkD3q
```

Каждый блок соответствует своему полю и содержит:

- Имя поля `Content-Disposition: form-data; name="picture"`
- MIME-тип поля `Content-Type: image/png` (если отличается от text/plain – простой текст)
- И сами данные

#### input и label [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Основным кирпичиком форм является элемент [input](https://webref.ru/html/input).
Он позволяет добавить в форму поля различных типов. Мы уже видели два вида полей
– текст и файл.

```html
<input name="author" value="Толстой Л.Н.">
<input name="picture" type="file" value="">
```

Атрибут `name` задаёт название поля, `value` его текущее значение, а `type` – тип.
Тип `text` (простое текстовое поле) является типом по умолчанию, и его можно
не указывать.

Для каждого поля можно вывести подпись при помощи элемента [label](https://webref.ru/html/label).
Чтобы связать их у элемента label в атрибуте `for` должно быть то же значение,
что у элемента input в атрибуте `id`. При клике на label браузер переводит фокус
(выделяет и устанавливает курсор) на связанное поле.

```html
<label for="author">Автор</label>
<input id="author" name="author" value="Толстой Л.Н.">
```
[demo](http://codepen.io/anon/pen/bVrgeN?editors=100)

Если подпись необходима, но места для неё нет. Можно использовать атрибут
`placeholder` у самого элемента `input`. Тогда подпись будет прямо в поле ввода.
Атрибут может быть использован, конечно, только в подходящих для этого типах полей.

```html
<input placeholder="Автор" name="author" value="">
```
[demo](http://codepen.io/anon/pen/MavJeJ?editors=100)

Рассмотрим ещё примеры типов полей:

```html
<!-- Поле для ввода текста -->
<!-- Вводимое значение можно ограничить по числу символов атрибутом `maxlength` -->
<label for="author">Автор</label>
<input name="author" value="Толстой Л.Н." maxlength="16">
<br>

<!-- Поле для выбора файла -->
<!-- Выбор файла можно ограничить MIME-типами в атрибуте `accept` -->
<label for="audio">Аудио версия книги</label>
<input id="audio" name="audio" type="file" value="" accept="image/jpeg,image/png,image/gif">
<br>

<!-- Поле для ответа на вопрос в формате «да/нет» -->
<!-- Можно поставить галочку (означает «да») нажатием на label или input -->
<label for="isClassicBook">Это классическое произведение?</label>
<input id="isClassicBook" name="isClassicBook" type="checkbox" value="">
<br>

<!-- Это поле можно использовать для выбора нескольких значений -->
<!-- Атрибут checked обозначает уже выбранное поле -->
<h1>Список дел</h1>
<label for="to">То</label>
<input id="to" name="todo" type="checkbox" value="to" checked>
<br>
<label for="se">Сё</label>
<input id="se" name="todo" type="checkbox" value="se">
<br>
<label for="paytoe">Пятое</label>
<input id="paytoe" name="todo" type="checkbox" value="5" checked>
<br>
<label for="desyatoe">Десятое</label>
<input id="desyatoe" name="todo" type="checkbox" value="10">
<br>

<!-- Скрытое поле -->
<!-- Не видны пользователю, и в основном используются для отправки технических данных -->
<!-- Например, время загрузки формы -->
<input name="form-load-time" type="hidden" value="2.387s">
<br>

<!-- Поле для выбора изображения -->
<label for="picture">Обложка для книги</label>
<input id="picture" name="picture" type="image" value="">
<br>

<!-- Поле для ввода пароля -->
<!-- При вводе пароль не виден, посторонние не смогут его подсмотреть -->
<label for="password">Пароль</label>
<input id="password" name="password" type="password">
<br>

<!-- Поле для выбора одного значения из предложенных -->
<label for="cover">Обложка для книги</label>
<input id="cover" name="cover" type="radio" value="Мягкая">
<input name="cover" type="radio" value="Твёрдая">
<br>
```
[demo](http://codepen.io/anon/pen/pjreLO?editors=100)

В html5 добавили ещё много новых типов:

```html
<!-- Поле для ввода цвета -->
<label for="color">Цвет страниц</label>
<input id="color" name="color" type="color" value="#f0f0f0">
<br>

<!-- Поле для ввода даты при помощи календаря-->
<!-- С помощью атрибутов `min`и `max` можно ограничить вводимую дату -->
<label for="date">Дата публикации</label>
<input id="date" name="date" type="date" value="2015-10-12" max="2015-10-17">
<br>

<!-- Поле для ввода даты при помощи календаря-->
<label for="email">Электронная почта автора</label>
<input id="email" name="email" type="email" value="lev.tolstoy@yandex.ru">
<br>

<!-- Поле для ввода числа -->
<!-- С помощью атрибутов `min`и `max` можно ограничить вводимое число -->
<!-- С помощью атрибута `step` можно задать шаг приращения числа -->
<label for="number">Количество экземпляров</label>
<input id="number" name="number" type="number" value="5" max="10" step="2">
<br>

<!-- Поле для ввода телефона -->
<label for="phone">Телефон автора</label>
<input id="phone" name="phone" type="tel" value="+700000000000">
<br>

<!-- Поле для ввода URL -->
<label for="url">Домашняя страница автора</label>
<input id="url" name="url" type="url" value="http://www.lev-tosltoy.ru/">
<br>

<!-- Поле для ввода времени -->
<label for="time">Время публикации</label>
<input id="time" name="time" type="time" value="13:47">
<br>
```
[demo](http://codepen.io/anon/pen/yYogMg?editors=100)

[Подробнее о типах](https://webref.ru/html/input/type)

Практически вегда мы должны не только давать пользователю вводить данные HTML5,
но и проверять их (валидировать). Для этого есть ряд специальных атрибутов:

- `required` – обнозначает поле как обязательное. Если значение не будет введено,
  то форма не отправится, а напротив этого поля возникнет подсказка с ошибкой.

    ```html
    <form>
        <input name="author" value="" required>
        <button type="submit">Отправить</button>
    </form>
    ```  
    [demo](http://codepen.io/anon/pen/MavpKG?editors=100)

- `pattern="[0-9]{6}"` – ограничивает ввод регулярным выражением.
  Если введённое значение не будет ему удовлетворять, то форма не отправится,
  а напротив этого поля возникнет подсказка с ошибкой.

  ```html
  <form>
    <label for="index">Почтовый индекс</label>
    <input id="index" name="index" pattern="[0-9]{6}" placeholder="XXXXXX" maxlength="6">
    <button type="submit">Отправить</button>
  </form>
  ```  
  [demo](http://codepen.io/anon/pen/epEvzL?editors=100)

- `readonly` – обозначает поле как «только для чтения»

    ```html
    <form>
        <input name="author" value="Толстой Л.Н." readonly>
        <button type="submit">Отправить</button>
    </form>
    ```  
    [demo](http://codepen.io/anon/pen/zvdZNe?editors=100)

- `disabled` – обозначает поле как «отключенное».
  В отличии от `readonly` значение этого поля не будет отправлено совсем.

    ```html
    <form>
      <input name="author" value="Толстой Л.Н." disabled>
      <button type="submit">Отправить</button>
    </form>
    ```  
    [demo](http://codepen.io/anon/pen/wKqJJe?editors=100)

#### button

Для отправки данных нам безусловно нужна кнопка [button](https://webref.ru/html/button)

```html
<form>
  <input name="author" value="">

  <!-- Кнопка типа reset очищает все поля формы -->
  <button type="reset">Очистить поля</button>

  <!-- Кнопка типа submit отправляет поля формы на сервер -->
  <button type="submit">Отправить</button>
</form>
```  
[demo](http://codepen.io/anon/pen/Vvzpzv?editors=100)

Кнопку можно заблокировать атрибутом `disabled`:

```html
<form>
  <input name="author" value="">
  <button type="submit" disabled>Отправить</button>
</form>
```
[demo](http://codepen.io/anon/pen/jbLBLz?editors=100)

Если мы хотим, чтобы после загрузки формы фокус был сразу на кнопке можно
указать атрибут `autofocus`:

```html
<form>
  <input name="author" value="">
  <button type="submit" autofocus>Отправить</button>
</form>
```

#### textarea

Существует ряд полей, которые исторически определяются другими элементами.
Например, [textarea](https://webref.ru/html/input/textarea)

```html
<label for="description">Описание</label>
<textarea id="description" name="description"></textarea>
```

Как и элемента `<input>` у него есть все необходимы атрибуты:
`disabled`, `readonly`, `maxlength`, `required`.

#### select и option

Как элемент `<input type="radio">`, элемент `<select>` предлагает пользователю
выбрать один вариант из предложенных в удобном и компактном виде:

```html
<label for="cover">Обложка для книги</label>
<select id="cover" name="cover">
    <option>Мягкая</option>
    <option selected>Твёрдая</option>
</select>
```
[demo](http://codepen.io/anon/pen/QjMpxr?editors=100)

По умолчанию, выбран всегда первый вариант, но можно пометить необходимый
атрибутом `selected` (будет выбран последний с таким атрибутом).

### Элементы встраиваемого содержимого – audio, iframe, img, svg, video, ... [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Если мы в наш HTML документ хотим вставить содержимое других типов, кроме текста
мы можем воспользоваться группой элементов встраиваемого содержимого. С помощью
них вы может вставлять аудио, видео, изображения и другие.

Вы уже знакомы с двумя такими `<svg>` (для вставки векторной графики) и
`<math>` (для размещения математических формул). Рассмотрим ряд других.

#### img и picture

При помощи элемента [img](https://webref.ru/html/img) мы можем встроить в страницу
изображение:

```html
<img
    src="//yastatic.net/morda-logo/i/bender/logo.svg"
    alt="Yandex"
    width="140"
    height="100"
>
```
[demo](http://codepen.io/anon/pen/pjreQQ?editors=100)

Мы указываем URL до изображения в атрибуте `src`, альтернативный текст в атрибуте
`alt` для пользователей с ограничением зрения или тех, у кого картинки отключены
(он экономит трафик).

Дополнительно мы можем указать `width` (ширину) и `height` (высоту) изображения,
чтобы подсказать браузеру заранее какое место это изображение займёт.

Так как мы живём в мире с миллионами различных устройств, мы хотим, чтобы
изображения выглядели хорошо везде. Устройства различаются разрешением экрана и
плотность точек (retina, 4k).

Для этого мы можем использовать атрибут `srcset`

```html
<img
    src="//yastatic.net/logo.png"
    alt="Yandex"
    srcset="//yastatic.net/logo-2x.png 2x, //yastatic.net/logo-400.png 400w"
>
```
[demo](http://codepen.io/anon/pen/pjreQQ?editors=100)

Атрибут повозволяет задать изображения для разных разрешения и плотности пикселей
через запятую `,`. Мы указываем URL изображения и затем через пробел условия.
Например:

- `2x` – показывать изображение `//yastatic.net/logo-2x.png` на экранах с удвоенной
  плотностю пикселей. По умолчанию, `1x` (его можно не указывать)

- `400w` – показывать изображение `//yastatic.net/logo-400.png` на экранах менее
  400 пикселей по ширине.

Условия можно комбинировать.

Более гибкий элемент для этого – `<picture>` (но он ещё не поддерживается в IE и
Safari). В нём мы тоже можем разместить несколько вариантов изображений для самых
разных случаев:

```html
<picture>
    <!-- Если браузер поддерживает изображение формата webp,
         будет использовано это изображение -->
    <source srcset="/uploads/100-marie-lloyd.webp" type="image/webp">

    <!-- Если ширина окна менее 600px,
         будет использовано это изображение -->
    <source srcset="a-square.png" media="(max-width: 600px)">

    <!-- Если ширина окна менее 600px,
         будет использовано одно из двух изображении
         в зависимости от плотности пикселей: 2x или 4x -->
    <source srcset="a-2x.png 2x, a-4x.png 4x," media="(max-width: 600px)">

    <!-- Если ширина окна менее 600px,
         будет использовано одно из двух изображении
         в зависимости от плотности пикселей: 2x или 4x -->
    <source srcset="a-2x.png 2x, a-4x.png 4x," media="(max-width: 600px)">

    <!-- Если ширина окна менее 600px,
         будет использовано изображение a-small.png на всю ширину окна `100vw` (100% viewport width)
         иначе – a-large.png на половину ширины окна `50vw` (50% viewport width)  -->
    <source srcset="a-small.png, a-large.png" sizes="(max-width: 600px) 100vw, 50vw">

    <!-- Изображение будет использовано, если не нашлось подходящих
         или элемент `picture` не поддерживается -->
    <img src="/uploads/100-marie-lloyd.jpg" alt="">
</picture>
```

[Подробнее об этом элементе](https://dev.opera.com/articles/responsive-images/)

#### iframe

Элемент [iframe](https://webref.ru/html/iframe) позволяет встроит один HTML
документ в другой. Например, чтобы встроить систему покупки билетов на сайт
кинотеатр.

```html
<iframe src="//booking.yandex.ru/organizations?permalink=1225142754" width="800" height="800">
```
[demo](http://codepen.io/anon/pen/pjrPyB?editors=100)

#### audio и video

Элемент [audio](https://webref.ru/html/audio) позволяет вставлять на страницу
аудио-проигрыватель, а [video](https://webref.ru/html/video) соответственно
видео-проигрыватель.

Эти элементы пришли на смену Flash в спецификиации HTML5.

```html
<!-- Задаём размеры видео с помощью `width` и `height`.
     Говорим показывать элементы управления при помощи атрибута `controls`.
     Говорим сразу проигрывать ролик при помощи атрибута `autoplay`.
     Задаём постер к видео в атрибуте `poster` -->
<video width="400" height="300" controls autoplay poster="https://webref.ru/example/video/duel.jpg">
    <!-- Задаём пути до видео файлов с помощью элемента <source>.
         Разные браузеры поодерживаю разные форматы -->
   <source src="https://webref.ru/example/video/duel.ogv" type='video/ogg; codecs="theora, vorbis"'>
   <source src="https://webref.ru/example/video/duel.mp4" type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'>
   <source src="https://webref.ru/example/video/duel.webm" type='video/webm; codecs="vp8, vorbis"'>

   <!-- Если элемент не поддерживается браузером
        выводим пояснение и ссылку на скачивание видео -->

   Элемент video не поддерживается вашим браузером.
   <a href="video/duel.mp4">Скачайте видео</a>.
</video>
```
[demo](http://codepen.io/anon/pen/NGvjje?editors=100)

Аналогичным образом работает элемент `<audio>`

## Глобальные атрибуты [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Как мы помним, у каждого элемента есть набор атрибутов, которые задают его
свойства и поведение. Например, у элемента `<button>` есть атрибут `disabled`,
который делает кнопку не активной.

```html
<button disabled>Сохранить</button>
```
[demo](http://codepen.io/anon/pen/xwdKPY?editors=100)

Но есть небольшой набор атрибутов, которые есть у всех элементов:

- Если нам необходимо задать пояснение к элементу – используем атрибут `title`.  
  Браузеры выводят его при наведении на элемент.

  ```html
  <!-- Расшифруем аббревиатуру -->
  <abbr title="Conseil Européen pour la Recherche Nucléaire">CERN</abbr>

  <!-- Расскажем пользователю немного о странице, куда мы его отправляем -->
  <a href="/html-part-2" title="Продолжение лекции HTML: интерактивные элементы.">HTML, часть II</a>
  ```
  [demo](http://codepen.io/anon/pen/VvbZrE?editors=100)

- Если мы хотим обратиться к элементу в CSS, чтобы задать стили; или в JS,
  чтобы задать поведение – используем атрибут `id` (identificator).  

  Он задаёт идентификатор элемента, **уникальный** для всего документа.

  ```html
  <!-- Поле ввода электронной почты -->
  <input type="email" id="email">
  ```  

  Теперь мы можем задать для него ширину в стилях:

  ```css
    #email
    {
        width: 100px;
    }
  ```
  [demo](http://codepen.io/anon/pen/vNmBWv?editors=110)

  Или с помощью JS вывести, введённое в него, значение:

  ```js
    //  Получаем доступ к элементу как к JS объекту по id
    var emailInput = document.getElementById('email');

    // В поле value этого объекта хранится введённое значение
    var email = emailInput.value

    // Выводим его
    console.log(email);
  ```
  [demo](http://codepen.io/anon/pen/ZbKzvK?editors=101)

  Не рекомендуется использовать `id` для добавления стилей к элементу,  
  лучше всего для этого подходит другой атрибут – `class`.

- Атрибут `class` позволяет задать класс набору элементов, сгруппировать их и
  задать общее оформление в CSS и поведение в JS.

  ```html
  <ul class="list">
    <li class="list-item">Молоко</li>
    <li class="list-item">Хлеб</li>
    <li class="list-item">Яблоки</li>
    <li class="list-item">Audi TT</li>
  </ul>
  ```  

  В примере, мы задали класс `.list-item` для всех элементов списка. И теперь мы
  можем для всех элементов класса `list-item` задать зелёный цвет текста:

  ```css
    .list-item
    {
        color: green;
    }
  ```
  [demo](http://codepen.io/anon/pen/bVWbLd)

  Или вывести, через запятую все элементы списка в JS

  ```js
    // Получаем все элементы списка по классу
    var items = document.getElementsByClassName('list-item');

    // Складываем в массив текст каждого элемента
    for (var i = 0, values = []; i < items.length; i++) {
        values.push(items[i].innerText);
    }

    // Выводим через запятую
    console.log(values.join(','));
  ```
  [demo](http://codepen.io/anon/pen/bVWbLd)

- А если мы хотим задать оформление прямо в html – используем атрибут `style`.

  ```html
  <!-- Текст заголовка окрасится в зелёный, и будет написан шрифтом Arial -->
  <h1 style="color: green; font-family: 'Times New Roman';">The Martian.</h1>
  ```
  [demo](http://codepen.io/anon/pen/epWOMR?editors=100)

  Рекомендуется не использовать этот атрибут в пользу отдельных CSS файлов
  со стилями и атрибута `class`, если это возможно.

## Семантическая разметка [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Хорошая разметка должна не только определять структуру, но и делать это
осмысленно – закрепляя за элементами определённый смысл: вот здесь у нас
навигация, а здесь адрес. Такая разметка называется *семанитической (Semantic
Markup)*.

Такая разметка помогает браузерам и поисковым системам лучше ориентироваться
в вашем документе. Например, чтобы автоматически сформировать версию для чтения,
или помочь выделить из документа адрес и телефон, или информацию по фильму,
товару, книге.

Это очень важно, если вы хотите, чтобы ваш документ было легко найти среди
миллионов других.

#### HTML5

Как вы уже знаете HTML 5 предоставляет уже очень много средств для семантической
(осмысленной) разметки. Так есть элементы:

- `<abbr>` – для аббревиатур и определений
- `<address` - для обозначения адреса
- `<dfn>` – для терминов и определений
- `<code>` – для кода программ
- `<nav>` – для навигации

Например, в такую разметку:

```html
<div>
    <p>CERN is a European research organization that operates
    the largest particle physics laboratory in the world.</p>

    <p>CERN's main function is to provide the particle accelerators
    and other infrastructure needed for high-energy physics research</p>

    <p>Last modified: 2015-09-22</p>
    <p>Author: ivan@example.com</p>
</div>
```

Мы можем легко добавить семантику так:

```html
<!-- Обозначаем статью -->
<article>
    <!-- Аббревиатуру -->
    <p><abbr title="Conseil Européen pour la Recherche Nucléaire">CERN</abbr> is
    a European research organization that operates the largest particle physics
    laboratory in the world.</p>

    <p>CERN's main function is to provide the particle accelerators
    and other infrastructure needed for high-energy physics research</p>
</article>

<!-- Информацию в подвале -->
<footer>
    <!-- Время -->
    <p>Last modified: <time>2001-04-23</time></p>

    <!-- И контактную информацию -->
    <address>Author: fred@example.com</address>
</footer>
```

#### Schema.org

Семантичных элементов в HTML5 много, но недостаточно для того большого
разнообразия информации, которое мы сейчас наблюдаем. Нет элементов, которые бы
нам сказали, что здесь описание фильма `<movie>`, а здесь анкета человека
`<person>`.

В 2011 году по инициативе компаний Bing, Google and Yahoo! был создан проект
[Schema.org](http://schema.org/docs/schemas.html), в рамках которой поисковые
системы поддержали ряд дополнительных возможностей для семантической разметки.

Схемы Schema.org позволяют такой код:

```html
<section>Привет всем, я Артём Кувалдин! Работаю разработчиком интерфейсов в Яндексе,
офис которого расположен в Екатеринбурге по адресу Хохрякова, 10.</section>
```

Сделать более осмысленным для поисковых систем, обозначив с помощью
специальных атрибутов – *микроданными (Microdata)*, что здесь расположена
информация о человеке:

```html
<section itemscope itemtype="http://schema.org/Person">
	Привет всем, я
	<span itemprop="givenName">Артём</span>
    <span itemprop="familyName">Кувалдин</span>,
	Работаю
	<span itemprop="jobTitle">разработчиком интерфейсов</span>
    в
    <span itemprop="affiliation">Яндексе</span>
    , офис которого расположен
	<section itemprop="address" itemscope itemtype="http://schema.org/PostalAddress">
		в
		<span itemprop="addressRegion">Екатеринбурге</span>
        по адресу
		<span itemprop="streetAddress">Хохрякова, 10</span>
        .
	</section>
</section>
```

Давайте разберём подробно, что мы добавили в код. Для начала с помощью атрибута
`itemscope` обозначаем, что в коде элемента `<section>` будет использована одна
из схем Schema.org.

Далее с помощью атрибута `itemtype` указываем путь до схемы
[Person](http://schema.org/Person). Схема описывает поля и их назначение:

Идентификатор поля | Назначение
---- | ----
givenName | Имя
familyName | Фамилия
jobTitle | Должность
affiliation | Организация, к которой относится человек

Чтобы связать текст с полем из схемы, необходимо обернуть его в элемент
и добавить атрибут `itemprop` со значением – идентификатором поля:

```html
<!-- Было -->
Артём

<!-- Стало -->
<span itemprop="givenName">Артём</span>
```

Внутри схемы можно использовать другие схемы. Так, в пример, мы внутри
[Person](http://schema.org/Person) использовали схему
[PostalAddress](http://schema.org/PostalAddress) (почтовый адрес).

```html
<section itemprop="address" itemscope itemtype="http://schema.org/PostalAddress">
    в
    <span itemprop="addressRegion">Екатеринбурге</span>
    по адресу
    <span itemprop="streetAddress">Хохрякова, 10</span>
    .
</section>
```

Схемой PostalAddress мы выделили в адресе отдельно город, отдельно улицу и дом.

Схем очень много, вот пример распространённых:

Схема | Назначение
---- | ----
[Book](http://schema.org/Book) | Книга
[Movie](http://schema.org/Movie) | Фильм
[Organization](http://schema.org/Organization) | Организация

[Полный список схем](http://schema.org/docs/full.html)

#### Микроформаты

Существует менее популярная альтернатива Scheme.org – *микроформаты
(Microformats)*. В отличии Scheme.org, она опирается не на атрибуты, а на классы.

Микроформаты также как и Scheme.org широко поддерживаются поисковыми системами,
но их меньше и полей в каждой схеме тоже немного.

Вот пример схемы [hcard](http://microformats.org/profile/hcard) для описания
пользователя:

```html
<head>
    <!-- Указываем используемую схему микроформатов в документе -->
    <link rel="profile" href="http://microformats.org/profile/hcard">
</head>
<ul class="vcard"> <!-- В этом элементе используем схему hcard -->
    <li class="fn">Артём</li> <!-- Имя -->
    <li class="org">Яндекс</li> <!-- Организация -->
    <li class="tel">777-7777</li> <!-- Телефон -->
    <!-- Адрес домашней странички -->
    <li><a class="url" href="http://example.com/">http://example.com/</a></li>
</ul>
```

Сейчас существует новая редакция микроформатов – *Microformats2*, со слегка
изменёнными классами:

```html
<ul class="h-card">
    <li class="p-name">Артём</li>
    <li class="p-org">Яндекс</li>
    <li class="p-tel">777-7777</li>
    <li><a class="u-url" href="http://example.com/">http://example.com/</a></li>
</ul>
```

[Полный список микроформатов](http://microformats.org/wiki/microformats2#v2_vocabularies).

Мы рекомендуем использовать Scheme.org, так как она использует только атрибуты,
которые логично задают дополнительные свойства элемента. Микроформаты, напротив,
исопльзуют классы, которые нужные ещё и для визуального оформления – что может
приводить к путанице.

## Интернационализация [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Так как интернет – всемирная паутина, важно задумываться о пользователях разных
стран, говорящих на разных языках. Ваша разметка должна поддерживать это.

#### Кодировка [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

В первую очередь необходимо указать кодировку документа.

*Кодировка (или что вернее, набор символов, character set, charset)* –
таблица, где каждому символу сопоставляется последовательность нулей и единиц
(битов).

Согласно кодировке устройство преобразует последовательность нулей и единиц в
символы, которые видит пользователь. Чтобы браузер правильно интепретировал HTML
документ, charset указывать обязательно.

Иначе вместо:

```
لغة C++&lm; هي لغة برمجة تستخدم.
```

Пользователь увидит нечто такое:

```
Ù„ØºØ© C++&lm; Ù‡ÙŠ Ù„ØºØ© Ø¨Ø±Ù…Ø¬Ø© ØªØ³ØªØ®Ø¯Ù….
```

Рекомендуется использовать кодировку
[utf-8 (Unicode Transformation Format, 8-bit)](https://ru.wikipedia.org/wiki/UTF-8)
– кодировку текста, которая позволяет хранить символы Юникода. [Юникод (Unicode)](https://ru.wikipedia.org/wiki/%D0%AE%D0%BD%D0%B8%D0%BA%D0%BE%D0%B4)
– стандарт кодирования, позволяющий представить знаки почти всех письменных языков.

Существует несколько способов указать charset:

- Используя технический метатег
  ```html
  <meta http-equiv="сontent-type" content="text/html; charset=utf-8">
  ```

- Используя специальный метатег (рекомендуемый)
  ```html
  <meta charset="utf-8">
  ```

- Если документ формата XHTML или XHTML5, в начале документа:
  ```xml
  <?xml version="1.0" encoding="utf-8"?>
  ```

Кодировка по умолчанию в HTML –
[ISO 8859-1](https://ru.wikipedia.org/wiki/ISO_8859-1), XHTML – utf8.

#### Язык [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Затем необходимо указать язык документа. Существует несколько способов сделать это:

- Используя технический метатег
  ```html
  <meta http-equiv="Content-Language" content="en-US, ru">
  ```

- Используя атрибут `lang` у элемента `<html>` (рекомендуемый)
  ```html
  <html lang="ru">
  ```

- Если документ формата XHTML или XHTML5,
  используя атрибут `xml:lang` у элемента `<html>`:
  ```xml
  <?xml version="1.0" encoding="utf-8"?>
  <html xml:lang="ru">
  ```

Если в документе используется несколько языков, можно указывать атрибут `lang`
для отдельных элементов:

```html
<html lang="ru">
    <p>Как говорил Джон Леннон</p>
    <blockquote lang="en">
        Life is what happens to you while you’re busy making other plans.
    </blockquote>
<html>
```

Для определённого языка позже можно задать своё оформление:

```css
p:lang(ar) { color: yellow; }
```

#### Направление текста [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Если язык подразумевает другое направление письма, стоит указать атрибут `dir`:
`ltr` – слева направо, `rtl` – справа налево, `auto` – автоматически.  

```html
<html dir="ltr">
```

Если в документе используется несколько языков, можно указывать атрибут `dir`
для отдельных элементов:

```html
<html dir="ltr">
    <p>Фраза на арабском языке:</p>
    <p dir="rtl">اللغة العربية‎‎</p><!-- В переводе: Aрабский язык -->
</html>
```

Текст на арабском языке выведется справа налево.  

Если нужен элемент, который только указывает другое направление
и не несёт других смыслов, лучше использовать элемент `<bdo>`
(bi-directional output):

```html
<bdo dir="rtl">اللغة العربية‎‎</bdo><!-- В переводе: Aрабский язык -->
```

Если содержимое одного элемента включает в себя, как текст слева-направо,
так и справа-налево, мы можем явно этим управлять, при помощи невидимых символов:

- `&lrm;` (left-to-right mark) – форсирует отображение текста слева-направа.

- `&rlm;` (right-to-left mark) – форсирует отображение текста справа-налево.

Например,

```html
<!-- В переводе: Язык C++ это язык программирования -->
<p dir="rtl">لغة C++&lrm; هي لغة برمجة تستخدم.</p>
```

Мы указываем, что `C++` нужно писать слева направо в любом языке.

Благодаря utf8 современные браузеры могут сами определять направление вывода
текста без указания атрибута `dir`. Но при этом не будут выраванивать текст
по правому краю, для этого атрибут всё же необходим.

#### Переводимость текста [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Если необходимо обозначит какой-либо текст непереводимым, можно использовать
атрибут `translate`. Он указывает автоматическим переводчикам
нужно ли переводить это текст: `yes` – по умолчанию, или `no`.

```html
<p>Press button <span translate="no">RESUME</span> to continue</p>
```

При переводе страницы, само название кнопки переведено не будет:

```html
<p>Нажмите кнопку <span translate="no">RESUME</span>, чтобы продолжить</p>
```

Атрибут поддерживается online переводчиками Microsoft, Google и Яндекс.
Он влияет не только на текст внутри элемента, но и на атрибуты `title` и `alt`:

```html
<p>Нажмите кнопку <img title="RESUME" translate="no" src="resume-button.jpg">,
чтобы продолжить</p>
```

Всплывающая подсказка при наведении на изображение не будет переведена.

#### Слияемость текста [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Если письмо подразумевает слитное начертание некоторых символов,
то мы можем явно этим управлять, при помощи невидимых символов:

- `&zwj;` (zero-width joiner) – форсирует слияние двух символов,
  между которыми он расположен.

- `&zwnj;` (zero-width non-joiner) – явно запрещает слияние двух символов,
  между которыми он расположен.

Если написать последовательно символы `क` и `ष` (инидийское письмо Девана́гари),
они автоматически сольются в `क्ष`, что не желательно в ряде слов.
Чтобы этого не происходило можно записать их так:

```html
<p>क्&zwnj;ष</p>
```

## Тип HTML документа [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

С момента появления Интернета прошло много времени, и за это время в разные годы
было создано огромное количество HTML документов по разным спецификациям:  
HTML 3.2, HTML 4.0, XHTML 1.0, XHTML 1.1, HTML 5, ...

Чтобы правильно интепретировать HTML документ, браузеру необходимо знать по
какой спецификации автор документа его создавал. Каким образом автор может
указать это?

#### Doctype [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

В начале HTML документа обязательно размещение специального элемента `<!DOCTYPE>`,
указывающего на тип документа, иными словами на спецификацию, по которой он был
создан.

```html
<!-- Документ создан по спецификации XHTML 1.0 -->
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html>
    <title>My awesome HTML page</title>
</html>
```

Синтаксис у этого элемента следующий:

```html
<!DOCTYPE [Корневой элемент] [Публичность] "[Регистрация]//[Организация]//[Тип] [Имя]//[Язык]" "[URL]">
```

- *Корневой элемент* – для HTML это всегда элемент **html**.

- *Публичность* – является ли документ публичным (значение  **PUBLIC**)
  или системным ресурсом (значение SYSTEM). Для HTML всегда указывается
  значение PUBLIC.

- *URL* — адрес документа с формальной описанием спецификации.
  Например, http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd

- *Тип* – тип документа с формальной описанием спецификации.
  Для HTML/XHTML значение указывается **DTD**.

- *Имя* – уникальное имя документа с формальной описанием спецификации.
  Например, **XHTML 1.0 Strict**

- *Язык* – язык, документа с формальной описанием спецификации.
  Например, **EN**.

- *Организация* – уникальное название организации, разработавшей DTD.
  Официально HTML/XHTML публикует **W3C**.

- *Тип организации* – «–» сообщает, что разработчик DTD НЕ зарегистрирован
  в международной организации по стандартизации (ISO). «+» – зарегистрирован.

Распространённые сейчас типы:

DOCTYPE	| Описание
------- | --------
**HTML 4.01** |
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd"> |	Строгий синтаксис HTML.
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd"> |	Переходный синтаксис HTML.
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd"> | В HTML-документе применяются фреймы.
**XHTML 1.0** |
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd"> |	Строгий синтаксис XHTML.
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"> |	Переходный синтаксис XHTML.
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd">	| Документ написан на XHTML и содержит фреймы.
**XHTML 1.1** |
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd"> | Строгий синтаксис XHTML 1.1.

#### Document Type Definition [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

**DTD (Document Type Definition)** – формальная схема спецификация языка,
предназначеная для автоматического разбора браузером или программой
(например, валидатором документов).

Схема DTD определяет структуру и синтаксис языка – описывает какие элементы есть,
какие у них доступны атрибуты и значения.

Пример описания элемента `<a>`:

```xml
<!--================== The Anchor Element ================================-->

<!ELEMENT A - - (%inline;)* -(A)       -- ссылка -->
<!ATTLIST A
  %attrs;                              -- %coreattrs, %i18n, %events --
  charset     %Charset;      #IMPLIED  -- Кодировка документа по ссылке --
  href        %URI;          #IMPLIED  -- URL ссылки --
  title       %Text;         #IMPLIED  -- Пояснение к ссылке --
  >
```

- `<!ELEMENT` описывает элемент и его свойства
- `<!ATTLIST` описывает атрибуты элемента и их тип например `%Text` – текст.

[Посмотреть полную схему DTD для HTML 4.0](http://www.w3.org/TR/html4/sgml/dtd.html)

Важно заметить, что DTD не описывает семантику, в ней нет никакой информации,
о том что означает элемент `<h1>`, как правильно его отображать, и чем он
отличается от `<h2>`.

#### Doctype для HTML 5 [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Большинство современных документов создаётя по спецификации HTML5. Для него
по историческим причинам, нет формального описания DTD, поэтому HTML5 документ
обозначается очень коротким `<!DOCTYPE`:

```html
<!-- Документ создан по спецификации HTML 5 -->
<!DOCTYPE html>
<html lang="en">
    <title>CERN</title>
</html>
```

## Ссылки [⇡](part-2.mdpart-2.md-ii-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

**Спецификации**

- **HTML5 от WHATWG**  
  https://html.spec.whatwg.org/multipage/

- HTML5 от W3C
  http://www.w3.org/TR/html5/

- HTML 5.1 Nightly  
  http://www.w3.org/html/wg/drafts/html/master/

- Differences between the W3C HTML 5.1 specification and the WHATWG LS  
  http://www.w3.org/wiki/HTML/W3C-WHATWG-Differences  

- XHTML 2.0  
  http://www.w3.org/TR/2010/NOTE-xhtml2-20101216/  

- XHTML 1.1  
  http://www.w3.org/TR/xhtml11/

- HTML 4.0  
  http://www.w3.org/TR/REC-html40-971218/  

- HTML 3.2  
  http://www.w3.org/TR/REC-html32

- HTML 2.0  
  https://tools.ietf.org/html/rfc1866  

- HTML+  
  http://www.w3.org/MarkUp/HTMLPlus/htmlplus_1.html

- HTML  
  http://www.w3.org/MarkUp/draft-ietf-iiir-html-01.txt

**Языки разметки и метаданные**  

- Markup language на wiki  
  https://en.wikipedia.org/wiki/Markup_language

- Understanding metadata  
  www.niso.org/publications/press/UnderstandingMetadata.pdf

- Schema.org schemes  
  http://schema.org/docs/full.html

- Microformats  
  http://microformats.org/wiki/microformats2

- Open Graph protocol  
  http://fbdevwiki.com/wiki/Open_Graph_protocol  

- Попробовать MathML  
  http://www.tutorialspoint.com/try_mathml_online.php

- Попробовать SVG  
  http://svg-edit.googlecode.com/svn-history/r1771/trunk/editor/svg-editor.html    

**HTML**

- **HTML на WebReference**  
  https://webref.ru/html/

- A history of HTML  
  http://www.w3.org/People/Raggett/book4/ch02.html

- HTML на wiki  
  https://en.wikipedia.org/wiki/HTML  

- XHTML на wiki  
  https://en.wikipedia.org/wiki/XHTML  

- HTML element на wiki   
  https://en.wikipedia.org/wiki/HTML_element  

- HTML attribute на wiki  
  https://en.wikipedia.org/wiki/HTML_attribute  

- List of XML and HTML character entity references на wiki  
  https://en.wikipedia.org/wiki/List_of_XML_and_HTML_character_entity_references  

- The Art of HTML Semantics: Part 1  
  http://kevinsuttle.com/posts/the-art-of-html-semantics-pt1/

- Метатеги  
  https://ru.wikipedia.org/wiki/%D0%9C%D0%B5%D1%82%D0%B0%D1%82%D0%B5%D0%B3%D0%B8  

- Валидация HTML документов на W3C
  https://validator.w3.org/

- Responsive Images: Use Cases and Documented Code Snippets to Get You Started  
  https://dev.opera.com/articles/responsive-images/  

- Srcset and sizes  
  https://ericportis.com/posts/2014/srcset-sizes/  

**URL, DNS, MIME**

- Percent Encoding   
  https://en.wikipedia.org/wiki/Percent-encoding   

- Список MIME-типов  
  https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_MIME-%D1%82%D0%B8%D0%BF%D0%BE%D0%B2

- Multipurpose Internet Mail Extensions (MIME)  
  https://tools.ietf.org/html/rfc2046

- DNS сервер BIND (теория)  
  http://habrahabr.ru/post/137587/

**Интернационализация**

- Юникод  
  https://ru.wikipedia.org/wiki/%D0%AE%D0%BD%D0%B8%D0%BA%D0%BE%D0%B4

- Таблица симоволов Юникод    
  http://unicode-table.com/ru/  

- UTF-8  
  https://ru.wikipedia.org/wiki/UTF-8

- UTF-8 encoding table  
  http://www.utf8-chartable.de/unicode-utf8-table.pl  

**Книги**

- **Using HTML and XHTML (Special Edition) (Molly E. Holzschlag)**  
  http://www.amazon.com/Using-HTML-XHTML-Special-Edition/dp/0789727315

- HTML & XHTML The Definitive Guide (Chuck Musciano and Bill Kennedy)
  http://shop.oreilly.com/product/9780596527327.do

- HTML & CSS: The Complete Reference (Thomas A. Powel)  
  http://www.amazon.com/HTML-CSS-Complete-Reference-Edition/dp/0071496297
