# HTML, I часть

- [Введение](part-1.md#%D0%92%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-)
- [История](part-1.md#%D0%98%D1%81%D1%82%D0%BE%D1%80%D0%B8%D1%8F-)
- [Анатомия](part-1.md#%D0%90%D0%BD%D0%B0%D1%82%D0%BE%D0%BC%D0%B8%D1%8F-)
    - [Элементы](part-1.md#%D0%AD%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-)
    - [Атрибуты](part-1.md#%D0%90%D1%82%D1%80%D0%B8%D0%B1%D1%83%D1%82%D1%8B-)
    - [Комментарии](part-1.md#%D0%9A%D0%BE%D0%BC%D0%BC%D0%B5%D0%BD%D1%82%D0%B0%D1%80%D0%B8%D0%B8-)
    - [Текст](part-1.md#%D0%A2%D0%B5%D0%BA%D1%81%D1%82-)
    - [Типы разметки](part-1.md#%D0%A2%D0%B8%D0%BF%D1%8B-%D1%80%D0%B0%D0%B7%D0%BC%D0%B5%D1%82%D0%BA%D0%B8-)
- [Элементы](part-1.md#%D0%AD%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B--1)
    - [Метаэлементы – title, meta, link, ...](part-1.md#%D0%9C%D0%B5%D1%82%D0%B0%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B--title-meta-link--)
    - [Секционные элементы – article, header, footer, section, nav, ...] (part-1.md#%D0%A1%D0%B5%D0%BA%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D1%8B%D0%B5-%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B--article-header-footer-aside-section--)
    - [Заголовочные элементы – h1 - h6,  hgroup](part-1.md#%D0%97%D0%B0%D0%B3%D0%BE%D0%BB%D0%BE%D0%B2%D0%BE%D1%87%D0%BD%D1%8B%D0%B5-%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B--h1---h6-hgroup-)
    - [Группирующие элементы – main, p, blockquote, ol, ul, dl, figure, div, ...](part-1.md#%D0%93%D1%80%D1%83%D0%BF%D0%BF%D0%B8%D1%80%D1%83%D1%8E%D1%89%D0%B8%D0%B5-%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B--main-p-blockquote-ol-ul-dl-figure-div--)
    - [Табличные элементы – table, tr, td, ... ](part-1.md#%D0%A2%D0%B0%D0%B1%D0%BB%D0%B8%D1%87%D0%BD%D1%8B%D0%B5-%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B--table-tr-td--)
    - [Текстовые элементы – em, br, mark, abbr, code, span, ...](part-1.md#%D0%A2%D0%B5%D0%BA%D1%81%D1%82%D0%BE%D0%B2%D1%8B%D0%B5-%D1%8D%D0%BB%D0%B5%D0%BC%D0%B5%D0%BD%D1%82%D1%8B--em-br-mark-abbr-code-span--)
- [Ссылки](part-1.md#%D0%A1%D1%81%D1%8B%D0%BB%D0%BA%D0%B8-)

## Введение [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

В основе обмена информацией в сети Интернет лежал *простой текст (Plain Text)*:

```text
Log entry: sol 7 Ok, I’ve had a good night’s sleep, and things don’t seem as
hopeless as they did yesterday. Today I took stock of supplies, and did a quick
EVA to check up on the external equipment. Here’s my situation: The surface
mission was supposed to be 31 days. For redundancy, the supply probes had enough
food to last the whole crew 56 days. That way if one or two probes had problems,
we'd still have enough food to complete the mission. We were six days in when
all hell broke loose, so that leaves enough food to feed six people for 50 days.
I’m just one guy, so it’ll last me 300 days. And that’s if I don’t ration it.
So I’ve got a fair bit of time.
```

Простого текста достаточно для обмена короткими сообщениями, например, в чате.
Но для обмена новостями, дневниками, научными работами, любой другой насыщенной
информацией возможностей простого текста стало недостаточно.

Текст не может нам рассказать ни о своей структуре, ни как правильно её
отображать, ни как его найти среди миллионов других. Всё что мы можем – разбить
текст на абзацы, используя символ переноса строки и обозначить заголовки
заглавными буквами.

```text
LOG ENTRY: SOL 7

Ok, I’ve had a good night’s sleep, and things don’t seem as hopeless as they
did yesterday.

Today I took stock of supplies, and did a quick EVA to check up on the external
equipment. Here’s my situation:

The surface mission was supposed to be 31 days. For redundancy, the supply
probes had enough food to last the whole crew 56 days. That way if one or two
probes had problems, we'd still have enough food to complete the mission.

We were six days in when all hell broke loose, so that leaves enough food
to feed six people for 50 days. I’m just one guy, so it’ll last me 300 days.
And that’s if I don’t ration it. So I’ve got a fair bit of time.
```

Ещё можем как-то разбавить стену текста ASCII графикой – и только.

```text
,--.   ,--.  ,---.  ,------.  ,---.
|   `.'   | /  O  \ |  .--. ''   .-'
|  |'.'|  ||  .-.  ||  '--'.'`.  `-.
|  |   |  ||  | |  ||  |\  \ .-'    |
`--'   `--'`--' `--'`--' '--'`-----'
```

Но в информационный век хочется большего:

- Хочется дополнить текст ссылками и цветными изображениями (с котиками).

- Хочеться удобного визуальное представления с выделенными заголовками
  списками и таблицами.

- Хочеться подсказать поисковыми система о чём наш текст,  
  чтобы больше людей смогли найти его среди бездны других.

Для полноценного решения этих задач были придуманы
*Языки разметки (Markup Language)*. Они позволяют нам дополнять простой текст
метаданными – «данными о данных», или «данными о тексте» в нашем случае.

Разметка (метаданные) не видна пользователю, но видна браузерами, поисковым
системам и другим программам для чтения размеченных текстов. Браузеры, читая
разметку, создают удобное визуальное представление текста.

Рассмотрим несколько примеров популярных языков разметки. Например, *MathML* –
для описания математических формул. Взяв простой текст формулы вычисления
корней квадратного уровнения:

```text
x = (-b ± √(b^2 - 4ac)) / 2a
```

Мы можем разметить его метаданными, обозначить дробь `<mfrac>`
и квадратный корень `<msqrt>`:

```xml
<math xmlns="http://www.w3.org/1998/Math/MathML">
    <mi>x</mi> <mo>=</mo>
    <mfrac>
      <mrow>
        <mo>−</mo> <mi>b</mi> <mo>±</mo>
        <msqrt>
          <msup> <mi>b</mi> <mn>2</mn> </msup>
          <mo>−</mo>
          <mn>4</mn> <mi>a</mi> <mi>c</mi>
        </msqrt>
      </mrow>
      <mrow> <mn>2</mn> <mi>a</mi> </mrow>
    </mfrac>
</math>
```

И современные браузеры отобразят скучный текст в виде красивой формулы:  

![](https://upload.wikimedia.org/math/8/c/5/8c58ae2d322a33f3036800d96db0e91a.png)

Или *SVG (Scalable Vector Graphics)* – язык разметки масштабируемой векторной
графики. Мы разметкой обозначаем круг `<circle>` и прямоугольник `<rect>`:

```xml
<svg width="100" height="100" xmlns="http://www.w3.org/2000/svg">
    <rect x="0" y="0" width="50" height="50" />
    <circle cx="50" cy="50" r="25" fill="red" />
</svg>
```
[demo](http://codepen.io/anon/pen/QjKLgm?editors=100)

А браузер рисует нам фигуры:  

![](https://img-fotki.yandex.ru/get/3709/32167648.0/0_133480_b838ff92_S)

Но мы поговорим о *HTML (HyperText Markup Language)*  
– языке разметки документов, предназначенных для обмена ими в Интернете.

```html
<meta name="keywords" content="Молоко, Хлеб, Яблоки">

<h1>Список покупок</h1>

<ul>
    <li>Молоко</li>
    <li>Хлеб</li>
    <li>Яблоки</li>
    <li>Audi TT</li>
</ul>
```
[demo](http://codepen.io/anon/pen/MajgoP?editors=100)

С помощью метаданных мы в тексте обозначили заголовок `<h1>` и список `<ul>`.
А так же добавили ключевых слов `<meta name="keywords"` – пользователи их не
увидят, а поисковые системы прочитают и помогут быстрее найти этот список.

В примере мы видим два типа метаданных:

- *Структурные метаданные (Structural Metadata)* – для описания структуры текста
  и компонентов из которых он состоит.

- *Описательные метаданные (Descriptive Metadata)* – для поиска и идентификации
  текстов.

Подробнее о метаданных можно прочитать в документе [Understanding metadata](http://www.niso.org/publications/press/UnderstandingMetadata.pdf)
от организации [NISO (National Information Standards
Organization)](http://www.niso.org/home/)

Но а мы проследим за становлением HTML с самих истоков.

## История [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

А истоки приводят нас в CERN (Conseil Européen pour la Recherche Nucléaire).
CERN – это научная площадка для учёных-физиков из университетов по всему миру
для совместной работы над ядерными исследованиям.

Для плодотворной работы любого сообщества необходима система обмена
документацией. Такая система существовала и в CERN в виде файлов, которые надо
было постоянно скачивать. И чтобы посмотреть связанный документ, необходимо было
искать его в куче файлов и снова скачивать. В какой-то момент такой обмен стал
катастрофически не удобным.

Так в 1989 году, британский учёный Tim Berners-Lee, работая в CERN над
улучшением системы обмена научной документацией, предложил новый формат
документов, который позволял бы быстро переходить из одного документа
в другой по ссылкам, не скачивая их.

![](http://static.trustedreviews.com/94/00002fb36/2f31/Tim-Berners-Lee.jpeg)

Уже в 1991 году он опубликовал первое описание формата для разметки таких
документов под названием «HTML Tags» и включил в неё описание 18 элементов,
11 из которых используются и по ныне, включая самый важный:
`<A HREF="http://info.cern.ch/">CERN</A>` – элемент ссылки.

В 1993 году был публично опубликован первый черновик спецификации
[HTML Internet-Draft](http://www.w3.org/MarkUp/draft-ietf-iiir-html-01.txt).

А чуть позже, в 1994 году, другой учёный Dave Raggett, просматривая новости
в газете, подумал, что неплохо было бы приспособить этот формат не только для
научной документации. Так появился другой черновик
[HTML+ (Hypertext Markup Format)](http://www.w3.org/MarkUp/HTMLPlus/htmlplus_1.html).
Dave добавил в него таблицы `<table>` для табличных данных и формы `<form>`.

В 1995 оба черновика были объединены в первую официальную рабочую спецификацию –
[HTML 2.0](https://tools.ietf.org/html/rfc1866). Она была немного дополнена
новыми возможностями: картами `<map>` - для отображения интерактивных карт,
и загрузкой файлов в формах `<input type="file" />`.

Интернет рос и потребности пользователей росли вместе с ним. В связи с бурным
ростом, развитием формата заинтересовались крупные компании – разработчики
браузеров Netscape и Microsoft. И чтобы как-то ускорить и упорядочить процесс,
работа была поручена организации
*[W3C (World Wide Web Consortium)](http://w3.org/)*

![](https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQ4k-OfCn24kJo0-2jlSJggdiXFYiGCw2coyGWdl1X6PVzWl759nQ)

Организация разрабатывала технологические стандарты для Интернета с 1994 года,
и на тот момент её воглавлял Tim Berners-Lee. Разработка спецификации HTML 3.0
стала первым серьёзным успехом. В этой версии они решили назревшую проблему –
поддержку оформления документов, добавить возможность описывать стили `<style>`.

Спецификация вышла очень громоздкой и весьма абстрактной, и каждая крупная
компания понимала её по своему, дополняя и разрабатывая свою собственную
интепретацию, положив начало, так называемым,
*[браузерным войнам](https://en.wikipedia.org/wiki/Browser_wars)*.
Результатом работы над ошибками стала спецификация
[HTML 3.2](http://www.w3.org/TR/REC-html32)

К тому моменту, в Интернете уже существовало множество документов, созданных
согласно разным версиям HTML. И браузерам стало необходимо как-то различать
документы, созданные по старым лекалам от новых.

Эту проблему решили в версии [HTML 4.0](http://www.w3.org/TR/REC-html40-971218/)
(1998 год) – она была разделена две интепретации:

- Strict (строгая) – устаревшие элементы не были разрешены
- Transitional (традиционная, консервативная) – устаревшие элементы были разрешены

В зависимости от того, какую версию автор HTML документа выбирал,
браузеры по разному её интепретировали, включая или нет новые возможности.

К тому моменту, стали больше задумываться о людях с ограниченными возможностями.
Для этого в HTML4 добавили атрибут `title` для всех элементов разметки.
Синтезатор речи для невидящих людей, использовал этот атрибут, чтобы подсказывать
пользователю, где он сейчас находится.

Следующую проблему, которую пытались решить разработчики HTML, – сделать его
более дружелюбным для программ (парсеров) и устройств. К тому моменту
существовало миллион программ, которые хорошо умели работать с форматом XML,
обладающим более строгим синтаксисом.

И самым простым решением было добавить в HTML строгий синтаксис XML:

HTML                            | XHTML                             | Пояснение
----                            | -----                             | ----
`<img src="image.png">`         | `<img src="image.png" />`         | Обязательное закрытие всех тегов ' />'
`<input checked>`               | `<input checked="checked" />`     | Атрибуты всегда в развёрнутой форме
`<TITLE>Список покупок</TITLE>` | `<title>Список покупок</title>`   | Теги и аттрибуты только строчными буквами

Бонусом к этому шла возможность легко включать внутрь HTML разметку
на других языках: SVG и MathML.

С тех пор вышло несколько версий
[XHTML 1.0](http://www.w3.org/TR/xhtml1/) (2000 год),
[XHTML 1.1](http://www.w3.org/TR/xhtml11/) (2001 год),
[XHTML 2.0](http://www.w3.org/TR/2010/NOTE-xhtml2-20101216/) (черновик, 2009 год).

Язык XHTML 2.0 препологал полный отказ от HTML – революционное развитие. Его
разработка продвигалась крайне медленно. Многие возможности XHTML 2.0 требовали
кардинально новых движков в браузерах.

В ответ на это в 2004 году появилась организация *[WHATWG (Web Hypertext
Application Technology Working Group)](https://whatwg.org/)*, организованная
сотрудниками компаний Apple, Mozilla Foundation и Opera Software.

![](https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcQy6TI865DkSA94_3z8dFD-0okRbiXg_Vi7qX9y09c1Wtxzo7Ui-AkaIIsT)

WHATWG предложила эволюционный путь развития, и вместо того, чтобы всё выкинуть
– продолжить развивать HTML 4, двигаясь постепенно к версии HTML5. Они показали,
что многи возможности XHTML 2.0 можно реализовать без существенных изменений в
браузерах. Такой путь оказался элементарно дешевле и в итоге победил.

В 2007 году W3C положил на полку XHTML 2.0 и взяла за основу версию спецификации
от WHATWG, но до настоящего времени по прежнему существую две версии.
Они практически идентичны, но отличаются в [незначительных деталях](http://www.w3.org/wiki/HTML/W3C-WHATWG-Differences).

Например, по версии W3C элемент `<main>` (главное содержимое документа)
может быть только один в документе, а по версии WHATWG их может быть несколько.

Плавная разработка формата позволила быстрее реагировать на меняющийся рынок:

- расцвет мобильных устройств;
- увеличение ширины сетвых каналов, появилась возможность смотреть видео
  и слушать музыку online;
- простые сайты превратились в целые приложение: почта, google docs.

В ответ на эти вызовы в [HTML5](http://www.w3.org/TR/html5/)
было добавлено много новых возможностей:

- Новые API, важные для мобильных устройств: Geolocation API (определение местоположения),
  Notification API (быстрые уведомления), ...;
- Теги `<audio>` и `<video>` на замену громоздкому и не безопасному решению - Flash;
- Новые виды полей ввода в формах: date/time, email, url, tel – для удобства
  ввода данных в больших web-приложениях.

![](http://photos3.meetupstatic.com/photos/event/6/4/b/2/global_20965778.jpeg)

Кое-что HTML5 унаследовал и от XHTML 2.0: возможность встраивать другие языки
разметки: SVG или MathML. А кое-что так и не было воплощено в жизнь:

- Для всех элементов можно было бы задать альтернативное изображение.
  ```html
  <h1 src="london-bridge.png">London Bridge</h1>
  ```
  – при наведении на заголовок всплывает изображение.

- Любой элемент мог стать ссылкой (а не только '<a>')
 ```html
 <img src="london-bridge.png" href="https://en.wikipedia.org/wiki/London_Bridge" />
 ```

HTML5 стандарт де-факто сейчас, его и будем препарировать.

## Анатомия [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

#### Элементы [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Кирпичиком разметки HTML документа является *элемент (HTML element)*. Каждый
элемент несёт своё предназначение. Например, ссылка:

```html
<a href="http://home.web.cern.ch/">CERN</a>
```

Каждый элемент состоит из:

- Открывающего тега (или дескриптора) – `<a>`;
- Закрывающего тега – `</a>`;
- Атрибутов – `href="http://home.web.cern.ch/"`;
- И содержимого – `CERN`.

*Тег (HTML tag)* состоит из имени элемента `a`, окруженного угловыми
скобками `<>`.

*Атрибут (HTML attribute)* состоит из имени атрибута `href`
и значения `http://home.web.cern.ch/`,   
окруженного кавычками `""`. Атрибуты задают свойства элемента.

По синтакисису все элементы можно разделить на четыре группы:

- *Void elements* – не имеют содержимого и закрывающего тега, только атрибуты.  
  Например элемент `<img>` (image), описывающий изображение:

  ```html
  <img src="https://images.whatwg.org/logo.svg">
  <!--  атрибут src хранит путь до картинки -->
  ```
  [demo](http://codepen.io/anon/pen/yYaBox?editors=100)

  Таких элементов всего 15:
  `<area>`, `<base>`, `<br>`, `<col>`, `<embed>`, `<hr>`, `<img>`, `<input>`,
  `<keygen>`, `<link>`, `<meta>`, `<param>`, `<source>`, `<track>` и `<wbr>`

- *Raw text elements* – в качестве содержимого могут иметь только текст.  
  Например элемент `<title>`, описывающий заголовок документа:

  ```html
  <title>CERN</title>
  ```

  Таких элементов всего четыре: `<script>`, `<style>`, `<title>` и `<textarea>`.

  Внутри таких элементов не может быть других элементов – текст.

- *Normal elements* – в качестве содержимого могут иметь как текст,
  так и другие вложенные элементы. Например элемент `<p>`,
  описывающий параграф текста:

  ```html
  <p>
    <a href="http://home.web.cern.ch/">CERN</a>
    is a European research organization
    that operates the largest particle physics laboratory in the world.
  </p>
  ```
  [demo](http://codepen.io/anon/pen/vNXBZK?editors=100)

  Внутри элеменета `<p>` (paragraph) лежит элемент `<a>` (anchor) и текст.

- *Foreign elements* – элементы из сторонних спецификаций **со своим синтаксисом**,
  например SVG:

  ```xml
  <svg width="100" height="100" xmlns="http://www.w3.org/2000/svg">
    <rect x="0" y="0" width="50" height="50" />
    <circle cx="50" cy="50" r="25" fill="red" />
  </svg>
  ```
  [demo](http://codepen.io/anon/pen/zvKOwX?editors=100)

Весь документ состоит из вложенных друг в друга элементов:

```html
<html>
    <meta name="keywords" content="CERN, European, physics">
    <title>CERN</title>
    <p>
        <a href="http://home.web.cern.ch/">CERN</a>
        is a European research organization
        that operates the largest particle physics laboratory in the world.
    </p>
</html>
```
[demo](http://codepen.io/anon/pen/zvKOZb?editors=100)

У ряда элементов мы можем не указывать закрывающий тег,  
например у элемента `<li>`, описывающего список:

```html
<ul>
    <li>Молоко
    <li>Хлеб
    <li>Яблоки
    <li>Audi TT
</ul>
```
[demo](http://codepen.io/anon/pen/JYRPOj?editors=100)

[Полный список элементов](http://www.w3.org/TR/html5/syntax.html#optional-tags),
у которых мы можем не указывать закрывающий тег.

Чтобы не запоминать все тонкости, **рекомендуется всегда закрывать теги**.

Чтобы один элемент мог вести себя по разному, существуют атрибуты.

#### Атрибуты [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Атрибуты задают свойства и поведение элемента и состоят из имени атрибута и значения,
окруженного кавычками `""` или `''` (не рекомендуется). Их может быть несколько:

```html
<input type="button" value="Click me!"> <!-- Кнопка с названием Click me! -->
```
[demo](http://codepen.io/anon/pen/GpjKOW?editors=100)

Кавычки не обязательны (если в тексте нет пробелов):

```html
<input type=button value=Click>
```

Бывают атрибуты без значений:

```html
<input type=button value=Click disabled> <!-- Кнопка заблокирована -->
```
[demo](http://codepen.io/anon/pen/jbMxrb?editors=100)

#### Комментарии [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

В коде HTML документа (как и в языках программирования)
можно оставлять комментарии:

```html
<!-- One line comment -->
```

Он может быть многострочным:

```html
<!--
    Multi line
    comment
-->
```

Обычно комментарии оставлят для пояснения кода,  
но они могут использоваться для специальных указаний браузеру:

```html
<!--[if IE 8]><link rel="stylesheet" href="ie8.css"/><![endif]-->
```

Благодаря такому комментарию, браузер Internet Explorer понимает,
что файл со стилями оформления `ie8.css` нужно загрузить только,
если версия браузера равна `8`.

#### Текст [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Текст в HTML разрешён только внутри элементов, значений аттрибутов и комментариях.  
Между атрибутами его размещать нельзя.

```html
<abbr здесь нельзя title="а здесь можно">и здесь можно</abbr> и тут.
```
[demo](http://codepen.io/anon/pen/jbMNaK?editors=100)

Новая строка может быть обозначена как символом `CR` (carriage return)
– возврат каретки, так и `LF` (line feed) – подача на строку, так и
двумя сразу `CR LF`.

Чтобы вставить особые символы, например ©, для удобства можно использовать  
*символы-мнемоники (Entity Characters)*:

```html
<p>&copy;</p> <!-- © -->
```
[demo](http://codepen.io/anon/pen/XmjrzQ?editors=100)

Указание `&` и `;` – обязательно.

Мы можем использовать *именованную ссылку на символ (Named Сharacter References)*.

```html
<p>&copy;</p>   <!-- © -->
<p>&amp;</p>    <!-- & -->
<p>&pound;</p>  <!-- £ -->
```
[demo](http://codepen.io/anon/pen/merbpR?editors=100)

Или *числовую ссылку (Numeric Character Reference)*.
Например для символа Σ (код которого в таблице символов 03A3):

```html
<p>&#x03A3;</p> <!-- Шестнадцатеричный код -->
<p>&#x3A3;</p>  <!-- Ноль можно опустить -->
<p>&#0931;</p>  <!-- Или десятичный код -->
<p>&#931;</p>   <!-- Ноль можно опустить -->
```
[demo](http://codepen.io/anon/pen/WQGedz?editors=100)

Символ может быть и невидим. Например:

```html
<p>Hello,&nbsp;World!</p>
<!--
     Неразрывный пробел (no-break space)
     – запрещает перенос World! отдельно от Hello
-->
```
[demo](http://codepen.io/anon/pen/yYaBpR?editors=100)

[Полный список именованых ссылок](http://www.w3.org/TR/html5/syntax.html#named-character-references)

#### Типы разметки [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

По назначению разметку делят на четыере группы:

- *Описательная (Descriptive Markup)* – определяет метаинформацию документа.
  Например, ключевые слова, автора документа, заголовок и кодировку.

  ```html
  <!-- заголовок документа -->
  <title>CERN</title>
  <!-- ключевые слова документа -->
  <meta name="keywords" content="CERN, European, physics">
  <!-- автор документа -->
  <meta name="author" content="Tim Berners-Lee">
  ```

- *Структурная (Structural Markup)* – определяет структуру и назначение текста

  ```html
  <h1>About CERN</h1> <!-- Заголовок первого уровня-->
  <p> <!-- Параграф -->
      <abbr title="Conseil Européen pour la Recherche Nucléaire">CERN</abbr> <!-- Аббревиатура -->
      is a European research organization
      that operates the largest particle physics laboratory in the world.
  </p>
  ```
  [demo](http://codepen.io/anon/pen/dYpbdG?editors=100)

- *Визуальная (Presentational Markup)* – определяет то, как элемент будет выглядеть

    ```html
    <b>bold text</b>                 <!-- Выделить жирным шрифтом -->
    <i>italic text</i>               <!-- Выделить курсивом -->
    <u>underlined text</u>           <!-- Подчеркнуть -->
    <center>centered text</center>   <!-- Вывести текст по центру -->
    ```
    [demo](http://codepen.io/anon/pen/merbXR?editors=100)

- *Ссылочная (Hypertext Markup)* - обозначает части документа, как ссылки

    ```html
    <a href="http://home.web.cern.ch/">CERN</a>
    ```
  В спецификации HTML5 такой элемент только один – `<a>`.

Визуальная разметка появилась до широкого распространения стилей CSS,
но в на сегодняшний день её уже рекомендуется не использовать. Вместо элементов:

```html
<p><center>centered text</center></p>
```
[demo](http://codepen.io/anon/pen/zvKORV?editors=100)

Рекомендуется использовать стили:  

```html
<p style="text-align: center">centered text</p>
```
[demo](http://codepen.io/anon/pen/VvKZXj?editors=100)

#### html [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Во основе документа лежит корневой элемент [html](https://webref.ru/html/html).
Он определяет границы документа:

```html
<html lang="ru">
</html>
```
[demo](http://codepen.io/anon/pen/qOaWYd?editors=100)

Рекомендуется указывать у него атрибут языка `lang="ru"`.
Атрибут языка помогает инструментам синтеза речи для не видящих людей
правильно выбирать произношение.

Этот тег не обязателен.

Для того, чтобы отделить описательную разметку от структурной, метаинформацию
для роботов, браузеров и поисковых систем, от содержимого для пользователей
есть два элемента '<head>' и '<body>'.

#### head [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [head](https://webref.ru/html/head) хранит в себе набор элементов,
определяющих метаинформацию документа для роботов, браузеров и поисковых систем.
Например, ключевые слова, автора документа, заголовок.  

```html
<html lang="en">
    <head>
        <meta charset="utf-8">
        <!-- ключевые слова документа -->
        <meta name="keyword" content="CERN, European, physics">
    </head>
</html>
```
[demo](http://codepen.io/anon/pen/gawYzR?editors=100)

Этот тег не обязателен.

#### body [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [body](https://webref.ru/html/body) хранит в себе набор элементов,
определяющих содержимое документа для пользователей.

```html
<html lang="en">
    <body>
        <p>CERN is a European research organization that operates
        the largest particle physics laboratory in the world.</p>
    </body>
</html>
```
[demo](http://codepen.io/anon/pen/bVwbML?editors=100)

Этот тег не обязателен.

## Элементы [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элементов в HTML очень много,
для удобства их можно разделить на несколько больших групп:

- Метаэлементы – title, meta, link, ...
- Секционные элементы – article, header, footer, nav, ...
- Заголовочные элементы – h1 - h6
- Группирующие элементы – main, p, blockquote, ol, ul, dl, figure, div, ...
- Текстовые элементы – em, br, mark, abbr, code, span, ...
- Ссылочные элементы – a
- Элементы форм – form, input, select, ...
- Элементы встраиваемого содержимого – audio, canvas, iframe, img, svg, video, ...

За каждым элемент скрывается вполне опредлённая задача. Чем точнее вы подберёте
элемент под задачу, тем дружелюбнее будет разметка как для пользователей, так
и для поисковых систем.

### Метаэлементы – title, meta, link, ... [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

#### title [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [title](https://webref.ru/html/title) определяет заголовок документа.  
Не виден в тексте, но используется для отображения на вкладке браузера
или в истории посещений.

```html
<html lang="en">
    <head>
         <title>CERN</title>
    </head>
</html>
```
[demo](http://codepen.io/anon/pen/yYaBjQ?editors=100)

`<title>` единственный обязательный тег, и он не должен быть пустым.
Поэтому минимально возможный корректный HTML документ выглядит так:

```html
<!DOCTYPE html>
<title> </title>
```
[demo](http://codepen.io/anon/pen/Zbpzow?editors=100)

Проверить HTML документ на корректность (валидность) можно на сайте W3C:
https://validator.w3.org/nu/#textarea

*Валидный HTML документ* – это документ, который строго удовлетворяет спецификации,
по которой он был создан.

#### base [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [base](https://webref.ru/html/base) определяет базовый адрес
для всех ссылок документа, а так же как они будут открываться
(в текущем окне `target="_self"` или в новом `target="_blank"`)  

```html
<html lang="en">
    <head>
         <base target="_blank" /> <!-- Все ссылки будут открываться в новом окне -->
    </head>
    <a href="http://home.web.cern.ch/">Homepage</a>
</html>
```
[demo](http://codepen.io/anon/pen/EVgYLq?editors=100)

```html
<html lang="en">
    <head>
         <base target="_blank" href="http://home.web.cern.ch/" />
    </head>
    <a href="about">About</a>
    <!-- Интепретируется как http://home.web.cern.ch/about -->
</html>
```
[demo](http://codepen.io/anon/pen/LpRPrp?editors=100)

#### link [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [link](https://webref.ru/html/link) устанавливает связь
с внешним документом, например с СSS файлом (где хранятся стили).

```html
<html lang="en">
    <head>
         <meta rel="stylesheet" href="styles.css">
         <meta rel="stylesheet" href="print-styles.css" media="print">
    </head>
</html>
```

Аттрибут `href` описывает путь к файлу стилей, `rel` (relationship) описывает
тип связи – «по ссылке файл со стилями», а `media` описывает устройство,
для которого следует применять стилевое оформление:

- `all` – все устройства (по умолчанию);
- `screen` – экран монитора;
- `print` – печатающие устройства;
- `speech` – речевые синтезаторы;
- `braille` – устройства, основанные на системе Брайля – для слепых людей.

Ещё один пример:

```html
<html lang="en">
    <head>
         <link
            rel="alternate"
            type="application/rss+xml"
            href="rss.xml">
    </head>
</html>
```

Элемент описывает, что есть альтернативный формат у документа `rel="alternate"`,  
типа RSS `type="application/rss+xml"` по ссылке `href="rss.xml"`.

Кстати, [RSS](http://cyber.law.harvard.edu/rss/rss.html)
тоже один из видов разметки информации, используемый для описания лент новостей,
анонсов статей, изменений в блогах.

[Список доступных типов связей](http://www.w3.org/TR/html5/links.html#linkTypes).

#### script [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [script](https://webref.ru/html/script) предназначен для описания скриптов,
может содержать ссылку на скрипт или его текст на определённом языке.

```html
<html lang="en">
    <head>
         <script src="path/to/my-jquery-plugin.js" type="text/javascript"></script>
    </head>
    <body>
        <script>
           console.log('Hello!');
        </script>
    </body>
</html>
```
[demo](http://codepen.io/anon/pen/yYaBEQ?editors=100)

Атрибут `type` имеет значение `text/javascript` по умолчанию, и его можно не указывать:

```html
 <script src="path/to/my-jquery-plugin.js"></script>
```

Ранее предпологалось, что javascript будет не единственный скриптовым языком
для браузеров. Был ещё VBScript (язык от Microsoft), его тип был `text/vbscript`.
На сегодняшний день javascript единственный выбор.

#### style [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [style](https://webref.ru/html/style) предназначен для определения стилей.

```html
<html lang="en">
    <head>
        <style type="text/css" media="screen">
            p { color: red; }
        </style>
    </head>
    <p>Important red text here!</p>
</html>
```
[demo](http://codepen.io/anon/pen/XmjrYL?editors=100)

Атрибут `type` имеет значение `text/css` по умолчанию, и его можно не указывать,
а `media` описывает устройство, для которого следует применять стилевое оформление.

#### meta [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [meta](https://webref.ru/html/meta)(метатег) определяет
метаинформацию документа. Например, ключевые слова, автора документа,
заголовок, кодировку.

```html
<html lang="en">
    <head>
        <meta charset="utf-8">
        <meta name="keyword" content="CERN, European, physics">
    </head>
    <p>CERN is a European research organization that operates
    the largest particle physics laboratory in the world.</p>
</html>
```

Атрибут `name` задаёт название, `content` – значение. Наиболее известны:

- `author` – имя автора документа;
- `description` – описание текущего документа;
- `keywords` – список ключевых слов.

Особый метатег `<meta charset="utf-8">` задаёт кодировку всего документа.  
Его рекомендуется располагать до любого текста на странице, включая `<title>`.

В исходной спецификации HTML5 не так много метатегов,  
поэтому компания Facebook расширила его спецификацией *Open Graph*:

```html
<html lang="en" prefix="og: http://ogp.me/ns#">
    <head>
        <meta property="og:title" content="CERN">
        <meta property="og:type" content="booring.article">
        <meta property="og:url" content="http://home.web.cern.ch/">
        <meta property="og:image" content="https://upload.wikimedia.org/wikipedia/CERN-Logo.svg.png">
    </head>
    <p>CERN is a European research organization that operates
    the largest particle physics laboratory in the world.</p>
</html>
```

Когда пользователь поделится ссылкой на этот документ,
социальные сети используют разметку Open Graph, чтобы рядом со ссылкой
разместить изображение, краткое описание и другую полезную информацию.

Помимо Facebook разметку Open Graph распознают также Яндекс, Вконтакте,
Google+, Twitter, LinkedIn, Pinterest и другие.

[Подробный список Open Graph тегов](http://fbdevwiki.com/wiki/Open_Graph_protocol).

Помимо информационных метатегов, есть технические. Технические метатеги фактически
копируют HTTP заголовки и **влияют на поведение документа**.

Вместо `name`, в них просто используется атрибут `http-equiv`
(HTTP Header Equivalent).

```html
<html lang="en">
    <head>

        <!-- Документ устареет 1 января 2016 года в 7 утра -->
        <meta http-equiv="expires" content="Sun, 01 Jan 2016 07:01:00 GMT">

        <!-- Страница буедт обновляться браузером раз в 5 секунд -->
        <meta http-equiv="refresh" content="5; url=http://www.example.com/">

    </head>
</html>
```

[Подробный список метатегов](https://ru.wikipedia.org/wiki/%D0%9C%D0%B5%D1%82%D0%B0%D1%82%D0%B5%D0%B3%D0%B8).

### Секционные элементы – article, header, footer, aside, section, ... [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Секционные элементы необходимы для деления документа на смысловые части:
основное содержимое, не основное, навигация, шапка, подвал:

![](http://kcaken.ru/wp-content/uploads/2010/11/html5_structure.png)

#### article [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [article](https://webref.ru/html/article) обозначает законченную
самодостаточную часть документа (self-contained),
которая вполне может существовать независимо (standalone):
пост на форуме или в блоге, новостная статья или виджет (например, календарь).

```html
<article>
    <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
</article>
```
[demo](http://codepen.io/anon/pen/XmjrBL?editors=100)

Элемент может содержать вложенные `<article>`. Так пост в блоге, может включать
в себя комментарии посетителей, каждый из которых – `<article>`

```html
<article> <!-- Пост в блоге -->
    <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
    <section>
        <h1>Комментарии</h1>
        <article> <!-- Комментарий -->
            <p>Отлично!</p>
        </article>
        <article> <!-- Комментарий -->
            <p>Где скачать?</p>
        </article>
    </section>
</article>
```
[demo](http://codepen.io/anon/pen/qOaWMO?editors=100)

#### section [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [section](https://webref.ru/html/section) определяет тематическую
группу элементов (thematic grouping). Например, блок комментариев к посту в блоге,
или главы в статье, или список постов:

```html
<section>
    <article>
      <!-- Первый пост -->
    </article>

    <article>
      <!-- Второй пост  -->
    </article>
</section>
```

#### nav [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [nav](https://webref.ru/html/nav) определяет блок с навигацие по
связанным документам.

```html
<nav>
    <a href="about.html">О компании</a>
    <a href="catalogue.html">Каталог продукции</a>
    <a href="contacts.html">Контакты</a>
</nav>
```
[demo](http://codepen.io/anon/pen/jbMNvv?editors=100)

Рекомендуется использовать только для главной навигации. Например, для ссылок
в подвале документа лучше использовать элемент `<footer>`, а не `<nav>`.

Браузер может использовать ссылки в этом элементе, чтобы предсказывать
дальнейшие действия посетителей и предзагружать страницы.

#### aside [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [aside](https://webref.ru/html/aside) определяет блок с сопуствующим
содержимым. Например, для обозначения выносок или цитат:

```html
<article> <!-- Пост в блоге -->
    <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
    <aside>
        <p>Браузер — прикладное программное обеспечение для просмотра веб-страниц</p>
    </aside>
    <p>Как только пользователь устанавливает курсор мыши в поле для ввода пароля
    на любом сайте, которого нет в списке, активируется система защиты.</p>
    <aside>
        <q>Везде, где есть жизнь, есть и опасность /Эмеpсон/</q>
    </aside>
</article>
```
[demo](http://codepen.io/anon/pen/vNXBzg?editors=100)

Так же этот элемент может использоваться для группировки нескольких элементов `<nav>`.

#### header [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [header](https://webref.ru/html/header) определяет
шапку всего документа или шапку секции.

```html
<header>
    <h1>Блог компании Яндекс</h1>
</header>
<article>
    <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
</article>
```
[demo](http://codepen.io/anon/pen/ZbpzMP?editors=100)

#### footer [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [footer](https://webref.ru/html/footer) определяет
подвал всего документа или подвал секции.

```html
<article>
    <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
</article>
<footer>
    <p>© 2013–2015  ООО «Яндекс»</p>
</footer>
```
[demo](http://codepen.io/anon/pen/XmjrPL?editors=100)

#### address [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [address](https://webref.ru/html/address) определяет блок с
контактной информацией, относящейся к ближайшему `<article>` или `<body>`.

`<address>` не должен содержать другой информации, кроме как контатной:
почтовый адрес, электронная почта, домашняя страницы в интернете.

```html
<article>
    <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
    <address>
        Для получения подробностей пишите на <a href="mailto:help@yandex.ru">help@yandex.ru</a>
    </address>
</article>
```
[demo](http://codepen.io/anon/pen/ojzvQL?editors=100)

### Заголовочные элементы – h1 - h6, hgroup [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

#### h1-h6 [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [h1-h6](https://webref.ru/html/h1) - определяет заголовок для
секционных элементов или `<body>`. Число определяет уровень, 1 – наивысший,
6 – наименьший.

```html
<article>
    <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
</article>
```
[demo](http://codepen.io/anon/pen/GpjKwv?editors=100)

#### hgroup [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [hgroup](https://webref.ru/html/hgroup) определяет группу
**связанных** заголовков: «заголовок – подзаголовок».

Чаще всего используется для двойных названий фильмов, альбомов и книг.

```html
<article>
    <hgroup>
        <h1>Dr. Strangelove or:</h1>
        <h2>How I Learned to Stop Worrying and Love the Bomb</h2>
    </hgroup>
    <p>An insane general triggers a path to nuclear holocaust
    that a war room full of politicians and generals frantically try to stop.</p>
</article>
```
[demo](http://codepen.io/anon/pen/OyRLaz?editors=100)

### Группирующие элементы – main, p, blockquote, ol, ul, dl, figure, div, ... [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Группирующие элементы объъединяют логические блоки внутри секций.

#### main [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [main](https://webref.ru/html/main) определяет главное содержимое страницы.

```html
<nav>
    <a href="/">На главную</a>
    <a href="/new">Свежие посты</a>
    <a href="/archive">Архив по года</a>
</nav>
<main>
    <article>
        <hgroup>
            <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
            <h2>Защита от кражи паролей</h2>
        </hgroup>
        <p>Яндекс.Браузер предостерегает пользователей,
        когда они начинают вводить пароль на подозрительных страницах.</p>
    </article>
</main>
```
[demo](http://codepen.io/anon/pen/dYpbwp?editors=100)

Согласно спецификаци W3C данный элемент может быть только один
(в версии WHATWG такого ограничения нет).

#### p [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [p](https://webref.ru/html/p) (paragraph) определяет параграф текста.

```html
<article> <!-- Пост в блоге -->
    <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
    <p>Как только пользователь устанавливает курсор мыши в поле для ввода пароля
    на любом сайте, которого нет в списке, активируется система защиты.</p>
</article>
```
[demo](http://codepen.io/anon/pen/OyRLrz?editors=100)

Не рекомендуется использовать `<p>`, если есть более подходящий элемент.
Например, для электронной почты лучше использовать `<address>`.

```html
<address>Author: fred@example.com</address>
```

#### hr [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [hr](https://webref.ru/html/hr) (horizontal rule) разделяет параграфы
текста. Например, когда сменилась тема повествования.

```html
<article> <!-- Пост в блоге -->
    <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
    <hr>
    <p>Как только пользователь устанавливает курсор мыши в поле для ввода пароля
    на любом сайте, которого нет в списке, активируется система защиты.</p>
</article>
```
[demo](http://codepen.io/anon/pen/KdgPbr?editors=100)

По умолчанию, браузер рисует горизонтальную линию.

#### pre [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [pre](https://webref.ru/html/pre) (preformatted text)
определяет блок предварительно форматированного текста.
Такой текст отображается моноширинным шрифтом, сохраняя всё форматирование:
пробелы, отступы.

Используется когда необходимо вывести участок кода или ASCII графику

```html
<pre>
,--.   ,--.  ,---.  ,------.  ,---.
|   `.'   | /  O  \ |  .--. ''   .-'
|  |'.'|  ||  .-.  ||  '--'.'`.  `-.
|  |   |  ||  | |  ||  |\  \ .-'    |
`--'   `--'`--' `--'`--' '--'`-----'
</pre>
```
[demo](http://codepen.io/anon/pen/yYaBGZ?editors=100)

```html
<pre>
    <code>function Panel(element, canClose) {
      this.element = element;
      this.canClose = canClose;
    }</code>
</pre>
```
[demo](http://codepen.io/anon/pen/qOaWvZ?editors=100)

#### blockquote [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [blockquote](https://webref.ru/html/blockquote)
предназначен для выделения длинных цитат внутри документа.

```html
<blockquote cite="http://example.com">
    Life is what happens to you while you’re busy making other plans. // Джон Леннон
</blockquote>
```
[demo](http://codepen.io/anon/pen/dYpbrO?editors=100)

Атрибут `cite` определяет ссылку на источник цитаты.

#### ol и li [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [ol](https://webref.ru/html/ol) (ordered list)
определяет упорядоченный список (1, 2, 3).  
Элемент [li](https://webref.ru/html/li) (list item) определяет элемент списка.


```html
<h1>Список покупок</h1>

<ol>
    <li>Молоко</li>
    <li>Хлеб</li>
    <li>Яблоки</li>
    <li>Audi TT</li>
</ol>
```
[demo](http://codepen.io/anon/pen/RWGbdg?editors=100)

Атрибут `reversed` задаёт обратный порядок, а `start` задаёт начальный номер:

```html
<ol start="8" reversed>
    <li>Молоко</li>
    <li>Хлеб</li>
    <li>Яблоки</li>
    <li>Audi TT</li>
</ol>
```
[demo](http://codepen.io/anon/pen/OyRLqQ?editors=100)

Выведет:
```
8. Молоко
7. Хлеб
6. Яблоки
5. Audi TT
```

Атрибут `type` задаёт тип нумерации:

Значение    | Пояснение
----        | ----
A           | заглавные латинские буквы
a           | строчные латинские буквы
I           | заглавные римские цифры
i           | строчные римские цифры
1           | арабские цифры.

```html
<ol type="i">
    <li>Молоко</li>
    <li>Хлеб</li>
    <li>Яблоки</li>
    <li>Audi TT</li>
</ol>
```
[demo](http://codepen.io/anon/pen/QjKLoZ?editors=100)

Выведет:
```
i. Молоко
ii. Хлеб
iii. Яблоки
iv. Audi TT
```

#### ul [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [ul](https://webref.ru/html/ul) (unordered list)
определяет НЕ упорядоченный список.

```html
<h1>Список покупок</h1>

<ul>
    <li>Молоко</li>
    <li>Хлеб</li>
    <li>Яблоки</li>
    <li>Audi TT</li>
</ul>
```
[demo](http://codepen.io/anon/pen/KdgPEb?editors=100)

Списки могут вложены друг в друга.

```html
<h1>Список покупок</h1>

<ul>
    <li>Молоко</li>
    <li>Хлеб</li>
    <ul>
        <li>Яблоки</li>
        <li>Апельсины</li>
    </ul>
    <li>Audi TT</li>
</ul>
```
[demo](http://codepen.io/anon/pen/ojzvOz?editors=100)

#### dl, dt и dd [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [dl](https://webref.ru/html/dl) (definition list)
задаёт список «термин-описание».  
Элемент [dt](https://webref.ru/html/dl) (definition term) задаёт термин.  
Элемент [dd](https://webref.ru/html/dl) (definition description)
задаёт описание термина.

```html
<dl>
    <dt>GIF</dt>
    <dd>Формат графических файлов, широко применяемый при создании сайтов.
    GIF использует 8-битный цвет и эффективно сжимает сплошные цветные области,
    при этом сохраняя детали изображения.</dd>
    <dt>JPEG</dt>
    <dd>Популярный формат графических файлов, широко применяемый при создании
    сайтов и хранения изображений. JPEG поддерживает 24-битный цвет и сохраняет
    яркость и оттенки цветов в фотографиях.</dd>
</dl>
```
[demo](http://codepen.io/anon/pen/YyGKMZ?editors=100)

Каждому термину `<dt>` может соответстовать несколько описаний `<dd>`.

'<dl>' может определять любый списки типа «ключ-значение», а не только «термин-описание».  

```html
<article>
    <h1>Protect — как Яндекс.Браузер защищает пользователей</h1>
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
</article>
<dl>
    <dt>Дата</dt>
    <dd>20 сентября 2015</dd>
    <dt>Автор</dt>
    <dd>Артём</dd>
</dl>
```
[demo](http://codepen.io/anon/pen/merbgM?editors=100)

#### figure и figcaption [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [figure](https://webref.ru/html/figure) используется для группирования
любых элементов и добавления подписи к ним
[figcaption](https://webref.ru/html/figcaption).

Чаще всего используется для добавления подписей к изображениям или коду:

```html
<figure>
    <figcaption>Listing 4. The panel.</figcaption>
    <pre>
        <code>function Panel(element, canClose) {
            this.element = element;
            this.canClose = canClose;
        }</code>
    </pre>
</figure>
<figure>
    <img src="https://images.whatwg.org/logo.svg" alt="bubbles" />
    <figcaption>Bubbles at work</figcaption>
</figure>
```
[demo](http://codepen.io/anon/pen/yYaBrw?editors=100)

#### div [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [div](https://webref.ru/html/div) (division, раздел)
– универсальный группирующий элемент с целью изменения вида содержимого через стили.

```html
<div style="color: red;">
    <p>Яндекс.Браузер предостерегает пользователей,
    когда они начинают вводить пароль на подозрительных страницах.</p>
    <p>Как только пользователь устанавливает курсор мыши в поле для ввода пароля
    на любом сайте, которого нет в списке, активируется система защиты.</p>
</div>
```
[demo](http://codepen.io/anon/pen/rOMBbX?editors=100)

Элемент `<div>` не несёт смысловой нагрузки, поэтому его не рекомендуется
использовать, если есть более подходящий.

### Табличные элементы – table, tr, td, ... [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [table](https://webref.ru/html/table) предназначен для разметки
табличных данных.

```html
<table>
    <thead>
        <tr>
            <th>Game name</th>
            <th>Game publisher</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Diablo</td>
            <td>Blizzard</td>
        </tr>
        <tr>
            <td>Portal</td>
            <td>Valve</td>
        </tr>
    </tbody>
</table>
```
[demo](http://codepen.io/anon/pen/xwEKNw?editors=100)

Game name   | Game publisher
----        | ----
Diablo      | Blizzard
Portal      | Valve

- `<thead>` – обозначает шапку таблицы
- `<tr>` – обозначает строку данных
- `<th>` – обозначает ячейку шапки
- `<tbody>` – обозначает данные таблицы
- `<td>` – обозначает ячейку таблицы

Ячейки можно объединять по горизонтали или вертикали при помощи специальных атрибутов:

- colspan – объединяет ячейки по горизонтали
- rowspan – объединяет ячейки по вертикали

```html
<table>
    <thead>
        <tr>
            <th>Game name</th>
            <th>Game publisher</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Half-Life</td>
            <td rowspan="2">Valve</td>
        </tr>
        <tr>
            <td>Portal</td>
        </tr>
    </tbody>
</table>
```
[demo](http://codepen.io/anon/pen/qOaWGZ?editors=100)

<table>
    <thead>
        <tr>
            <th>Game name</th>
            <th>Game publisher</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Half-Life</td>
            <td rowspan="2">Valve</td>
        </tr>
        <tr>
            <td>Portal</td>
        </tr>
    </tbody>
</table>

### Текстовые элементы – em, br, mark, abbr, code, span, ... [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

#### em [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [em](https://webref.ru/html/em) (emphasis, акцент)
предназначен для акцентирования текста.

```html
<p><em>Cats</em> are cute animals.</p>
```
[demo](http://codepen.io/anon/pen/JYRPQX?editors=100)

`<em>` обозначает ключевую часть предложения (не обязательно важного),
в то время как `<strong>` обозначает именно важную информацию.

#### strong [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [strong](https://webref.ru/html/strong)
предназначен для обозначения важной информацию.

```html
<p><strong>Внимание! Идут учения!</strong></p>
```
[demo](http://codepen.io/anon/pen/QjKLXJ?editors=100)

#### ins [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [ins](https://webref.ru/html/ins) (inserted text)
предназначен для выделения текста, который был добавлен к текущему.

```html
<p>С++, python, <ins datetime="2005-03-16">javascript</ins> – классные языки программирования</p>
```
[demo](http://codepen.io/anon/pen/zvKYOx?editors=100)

Атрибут `datetime` указывает на время добавления текста

По умолчанию, браузер выделяет его подчёркиванием.

#### del [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [del](https://webref.ru/html/del) (deleted text)
предназначен для выделения текста, который был удалён.

```html
<p>С++, python, javascript, <del datetime="2005-03-16">PHP</del> – классные языки программирования</p>
```
[demo](http://codepen.io/anon/pen/EVgxxV?editors=100)

Атрибут `datetime` указывает на время удаления текста

По умолчанию, браузер выделяет его зачёркиванием.

Элементы `<del>` и `<ins>` чаще всего используются в wiki, для того, чтобы
показать что изменилось в документе с момента последней его редакции.

#### mark [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [mark](https://webref.ru/html/mark) (marked text)
помечает текст как выделенный.

```html
<p>С++, python, <mark>javascript</mark> – классные языки программирования</p>
```
[demo](http://codepen.io/anon/pen/VvKYgJ?editors=100)

По умолчанию, браузер выделяет его жёлтым маркером.

Удобно использовать это элемент и для выделения участка кода:

```html
<pre>
    <code>function <mark>Panel</mark>(element, canClose) {
      this.element = element;
      this.canClose = canClose;
    }</code>
</pre>
```
[demo](http://codepen.io/anon/pen/wKzBOz?editors=100)

#### small [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [small](https://webref.ru/html/small) предназначен для различных оговорок.
Например, для условий и правовых ограничений в рекламе.

```html
<p>Скидка на все товары 50%</p>
<p><small>При условии покупки на сумму более 1000 рублей</small></p>
```
[demo](http://codepen.io/anon/pen/zvKxXJ?editors=100)

По умолчанию, браузер выделяет его мелким шрифтом.

#### cite [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [cite](https://webref.ru/html/cite) (отсылки) предназначен для выделения
названий книг, песен, фильмов; имён авторов (то есть отсылок к ним).

```html
<p>Роман Замятина <cite>Мы</cite> – одна из лучших книг-антиутопий</p>
```
[demo](http://codepen.io/anon/pen/PPGwvN?editors=100)

По умолчанию, браузер выделяет его курсивом.

#### q [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [q](https://webref.ru/html/q) (quote, цитата)
предназначен для выделения цитат или обозначения прямой речи.

```html
<p><q>Le  général  Koutouzoff,</q> -- сказал  Болконский,  ударяя на последнем
  слоге zoff, как  француз</p>
```
[demo](http://codepen.io/anon/pen/KdgwLX?editors=100)

По умолчанию, браузер выделяет текст кавычками.

#### dfn [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [dfn](https://webref.ru/html/dfn) (definition, определение)
предназначен для выделения определений, терминов.

```html
<p><dfn>Гипотенуза</dfn> – Сторона прямоугольного треугольника,
лежащая против прямого угла.</p>
```
[demo](http://codepen.io/anon/pen/wKzawg?editors=100)

По умолчанию, браузер выделяет текст курсивом.

#### abbr [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [abbr](https://webref.ru/html/abbr) (abbreviation)
предназначен для выделения аббревиатур.

```html
<abbr title="Conseil Européen pour la Recherche Nucléaire">CERN</abbr>
```
[demo](http://codepen.io/anon/pen/GpjJgZ?editors=100)

Браузер при наведении покажет подсказку с рашифровкой.

#### ruby, rt [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [ruby](https://webref.ru/html/ruby) (ruby annotations, сноски)
предназначен для добавления небольшой
аннотации сверху или снизу от заданного текста.

```html
<!-- Выводим транскрипцию английских букв над ними -->
<ruby>A<rt>[ei]</rt></ruby>
<ruby>B<rt>[bi:]</rt><ruby>
<ruby>C<rt>[si:]</rt><ruby>

<!-- Добавляем перевод слова верху-->
<ruby lang="ja">編集者<rt lang="ru">Редактор</ruby>
```

![](https://img-fotki.yandex.ru/get/4005/32167648.0/0_133481_6d8b04e1_S)

[demo](http://codepen.io/anon/pen/JYRdKQ?editors=100)

#### time [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [time](https://webref.ru/html/time)
предназначен для выделения дат.

```html
<article>
   <p><time>1957-10-04</time> запущен первый искусственный спутник Земли.</p>
   <p><time>1960-08-19</time> первый полёт собак в космос.</p>
   <p><time>1961-04-12</time> первый полёт человека в космос.</p>
   <p><time>1963-06-16</time> первый полёт женщины-космонавта.</p>
   <p><time>1969-07-21</time> высадка человека на Луну.</p>
</article>
```
[demo](http://codepen.io/anon/pen/LpRVxP?editors=100)

 Можно использовать атрибут `datetime` для указание даты программам машинной
 обработки текста – поисковым системам.

 ```html
<time datetime="2011-11-18T14:54:39Z">November 11</time>
 ```
[demo](http://codepen.io/anon/pen/bVwdgr?editors=100)

#### samp, kbd [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [samp](https://webref.ru/html/samp) (sample output)
используется для отображения текста, который является результатом вывода
компьютерной программы или скрипта.

Элемент [kbd](https://webref.ru/html/kbd) (keyboard)
используется для обозначения текста, который набирается на клавиатуре
или для названия клавиш.

```html
<article>
    <p>Нажмите <kbd>CTRL</kbd> + <kbd>S</kbd> на клавиатуре.
    <p>Компьютер должен ответить <samp>Document was saved successfuly</samp>.</p>
</article>
```
[demo](http://codepen.io/anon/pen/bVwdqo?editors=100)

#### var, code [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [code](https://webref.ru/html/code)
используется для отображения текста, который является результатом вывода
компьютерной программы или скрипта.

```html
<pre>
    <code>function Panel(element, canClose) {
      this.element = element;
      this.canClose = canClose;
    }</code>
</pre>
```
[demo](http://codepen.io/anon/pen/yYaNqQ?editors=100)

Элемент [var](https://webref.ru/html/var) (variable)
используется для выделения переменных в компьютерных программах или
математических выражениях.

```html
<p>
     Формула эквивалентности массы и энергии:
    <var>E</var> = <var>m</var> <var>c</var><sup>2</sup>
</p>
```
[demo](http://codepen.io/anon/pen/bVwdxv?editors=100)

Но, в перспективе для написания формул лучше использовать язык MathML.
Сейчас он ещё не широко поддерживается браузерами.

#### sup, sub [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [sup](https://webref.ru/html/sup) (superscript)
обозначает текст как верхний индекс. Например, для обозначения степени:

```html
<p>
    Формула эквивалентности массы и энергии:
    <var>E</var> = <var>m</var> <var>c</var><sup>2</sup>
</p>
```
[demo](http://codepen.io/anon/pen/bVwdxv?editors=100)

Элемент [sub](https://webref.ru/html/sub) (subscripts)
обозначает текст как нижний индекс.

```html
<p>
    Формула воды: H<sub>2</sub>O.
</p>
```
[demo](http://codepen.io/anon/pen/RWGPEV?editors=100)

#### br, wbr [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [br](https://webref.ru/html/br) (break line)
устанавливает перевод строки в том месте, где он находится.

```html
<p>
Варкалось. Хливкие шорьки<br>
Пырялись по наве,<br>
И хрюкотали зелюки,<br>
Как мюмзики в мове.<br>
</p>
```
[demo](http://codepen.io/anon/pen/dYporp?editors=100)

`<br>` не рекомендуется использовать для разделение текста на тематический группы,
для этого рекомендуется использовать элемент `<p>` (параграф)

Элемент [wbr](https://webref.ru/html/wbr) (word break) указывает браузеру место,
где допускается делать перенос строки в длинном слове:

```html
<p>метоксихлор<wbr>диэтиламино<wbr>метил<wbr>бутил<wbr>амино<wbr>акридин</p>
```
[demo](http://codepen.io/anon/pen/ZbpGPN?editors=100)

#### span [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

Элемент [span](https://webref.ru/html/span) (span, интервал)
– универсальный текстовый элемент с целью изменения вида содержимого через стили.

```html
<span style="color: red;">Яндекс.Браузер предостерегает пользователей,
когда они начинают вводить пароль на подозрительных страницах.</span>
```
[demo](http://codepen.io/anon/pen/vNXOEO?editors=100)

Элемент `<span>` не несёт смысловой нагрузки, поэтому его не рекомендуется
использовать, если есть более подходящий.

#### Визуальная разметка i, b, center, s, u [⇡](part-1.md#html-i-%D1%87%D0%B0%D1%81%D1%82%D1%8C)

- `<b>` (bold) – выделяет текст жирным шрифтом
- `<i>` (italic) – выделяет текст курсивом
- `<center>` – размещает текст по центру
- `<s>` (strikethrough) – выводит текст зачёркнутым
- `<u>` – выводит текст подчёркнутым

Напомню, что визуальная разметка появилась до широкого распространения стилей CSS,
но в на сегодняшний день её уже рекомендуется не использовать. Вместо элементов:

```html
<p><center>centered text</center></p>
```
[demo](http://codepen.io/anon/pen/zvKORV?editors=100)

Рекомендуется использовать стили:  

```html
<p style="text-align: center">centered text</p>
```
[demo](http://codepen.io/anon/pen/VvKZXj?editors=100)

[Список всех текстовых элементов](https://html.spec.whatwg.org/multipage/semantics.html#usage-summary).

## Ссылки [⇡](text.md#html)

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
  http://schema.org/docs/schemas.html

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

**Интернационализация**

- Юникод  
  https://ru.wikipedia.org/wiki/%D0%AE%D0%BD%D0%B8%D0%BA%D0%BE%D0%B4

- UTF-8  
  https://ru.wikipedia.org/wiki/UTF-8

**Книги**

- **HTML & XHTML The Definitive Guide (Chuck Musciano and Bill Kennedy)**  
  http://shop.oreilly.com/product/9780596527327.do

- HTML & CSS: The Complete Reference (Thomas A. Powel)  
  http://www.amazon.com/HTML-CSS-Complete-Reference-Edition/dp/0071496297

- Using HTML and XHTML (Special Edition) (Molly E. Holzschlag)  
  http://www.amazon.com/Using-HTML-XHTML-Special-Edition/dp/0789727315
