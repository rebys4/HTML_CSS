# HTML_CSS
Конспект по курсу HTML/CSS/JS

## Краткая информация про HTML
**HTML** - это язык разметки, который используется для создания веб-страниц. Он представляет собой способ **описания** структуры и содержания веб-страницы, **позволяя** браузерам интерпретировать и отображать:
1) Текст;
2) Изображения;
3) Ссылки;
4) Видео и другие элементы на веб-сайте.

HTML **использует** специальные **теги** (кодовые метки в угловых скобках <>), чтобы определить, какой текст должен быть заголовком, параграфом, изображением, ссылкой и т. д. Эти теги **позволяют** создавать структуру страницы, делая её более понятной для браузеров и поисковых систем.

## HTML: Теги
Пример **двойного тега**:
```
<p>
    Привет, мир!
</p>
```
В данном примере двойной тег - это ```<p>```. Двойные теги показывают начало и конец элемента. 
>[!WARNING]
> - **Начало** элемента обозначают - открывающимся тегом <...>
> - **Конец** элемента - закрывающим </...>
> - **Текст "Привет мир" в данном случае является контентом(Content)**. Это контент элемента, который в данном случае является просто текстом.
> - **Элемент (Element)**: Открывающий тег, закрывающий тег и контент вместе составляют элемент

**Помимо двойных тегов существуют одинарные, и они не имеют пары.**

## HTML: Атрибуты
**Атрибуты** - это дополнительная **информация**, которая присваивается HTML-элементам, чтобы **определить** их свойства или параметры.
>[!WARNING]
> Они **указываются внутри открывающего** тега элемента и предоставляют браузеру или другим программам дополнительные инструкции о том, как элемент должен вести себя или как его следует отображать на веб-странице.

**Синтаксис атрибута**:
```HTML
<элемент атрибут="значение">
```
- ```<элемент>``` - это HTML-элемент, к которому применяется атрибут.
- ```атрибут``` - имя атрибута, указывающее, какое свойство элемента будет изменено.
- ```значение``` - значение атрибута, которое определяет, каким образом будет изменено свойство элемента.


## HTML: Заголовки
**Заголовки** являются важной частью **HTML** документа, обычно **заголовок** — это краткое описание того, что будет представлено ниже на странице

>[!Warning]
>Заголовки в HTML создаются с помощью тега ```h``` после которого идет цифра от 1 до 6, например ```<h1>```, где:
> - ```h``` - сокращение от английского heading (заголовок);
> - 1..6 - уровни заголовка;
> - Все теги являются парными.

**Верхним** уровнем является - 1 (```<h1>```), самым **нижним** - уровень 6 (```<h6>```).

## HTML: Параграфы
**Параграф** - это один из **основных** HTML-элементов, используемых для оформления и структурирования текста на веб-странице. Элемент ```<p>``` обозначает абзац текста и позволяет создавать разделение между разными абзацами контента.

**Синтаксис** тега параграфа:
```HTML
<p>
    Ваш текст здесь
</p>
```
- ```<p>``` - это **открывающий** тег параграфа.
- ```</p>``` - это **закрывающий** тег параграфа.

>[!WARNING]
> Текст, который находится **между** этими тегами, будет рассматриваться как отдельный абзац и отображаться соответствующим образом на веб-странице.

## HTML: Списки
**Список** - это набор взаимосвязанных элементов, которые используются для группировки какой либо информации.

**Списки** бывают следующих видов:
- Нумерованный
- Маркированный
- Вложенный
- Список определений

*Разберем каждый подробнее*

### **Нумерованный**

В **нумерованном** списке перед каждым элементом списка идет **номер**.

Он **создается** при помощи тега ```<ol>``` — ordered list (упорядоченный список). Каждый пункт списка создаётся с помощью элемента ```<li>``` — list item (пункт списка).

### **Маркированный**

В **маркированном** списке перед каждым элементом списка идет маркер.

Маркированный список **создается** с помощью тега ```<ul>``` — unordered list (неупорядоченный список). Стандартный маркер — точка. Каждый пункт списка также создаётся с помощью элемента ```<li>``` — list item (пункт списка).

### **Вложенный**
У нас на очереди **вложенный** список, с помощью **вложенных** списков можно вкладывать одни элементы в другие, тем самым у нас получаются подпункты.

Чтобы создать **вложенный** список в HTML нужно использовать все те же элементы. Суть проста, в элемент ```<li>...</li>``` вкладывается новый маркированный или нумерованный список, начиная с элемента ```<ul>``` или ```<ol>```.

### **Список определений**
**Список определений** (Definition List) - это структура в HTML, которая используется для **представления** определений или терминов вместе с их описаниями.

>[!WARNING]
> Список определений состоит из пар "термин - описание" и предоставляет удобный способ организации информации.

Он использует следующие теги:

1) ```<dl>``` **(Definition List)**: Этот тег представляет собой обертку для всего списка определений. Он обрамляет все пары "термин - описание".
2) ```<dt>``` **(Definition Term)**: Этот тег используется для определения термина или того, что вы хотите определить. Он идет внутри тега ```<dl>```.
3) ```<dd>``` **(Definition Description)**: Этот тег используется для предоставления описания или определения для соответствующего термина, который находится в теге ```<dt>```. Тег ```<dd>``` также идет внутри тега ```<dl>```.

## HTML: Тег переноса
Перенос строк текста в HTML через тег ```<br/>```

```<br/>``` этот тег указывающий на место разрыва строки и принудительного переноса текста на новую строку. И только для этих целей он должен применяться.

## HTML: Блочные теги

**Блочные теги** (или блочные элементы) - это одна из двух **основных** категорий HTML-элементов, которые используются для организации и структурирования содержимого на веб-страницах.

Блочные элементы **характеризуются** следующими особенностями:

1) **Основная черта блочных элементов** - они **занимают всю доступную горизонтальную ширину на странице** и начинаются с **новой** строки после себя. Это означает, что каждый блочный элемент начинается с новой строки и занимает всю доступную горизонтальную ширину на странице, что делает их подходящими для организации больших блоков контента.
2) **Примеры блочных элементов**: Некоторые популярные блочные элементы в HTML включают ```<div>, <p>, <h1> до <h6>, <ul>, <ol>, <li>, <table>, <form>``` и многие другие.
3) **Вложенность**: Блочные элементы могут **вкладываться** друг в друга, что позволяет создавать сложные структуры и макеты веб-страниц.

## СТРОЧНЫЕ ТЕГИ ДЛЯ РАБОТЫ С ТЕКСТОМ
- ```<b>``` - Определяет жирное начертание шрифта.
- ```<strong>``` - Этот тег делает текст жирным и обычно используется для выделения важных слов или фраз.
- ```<em>``` - Этот тег придает тексту курсивное начертание и используется для выделения текста с эмоциональным акцентом или подчеркивания важности.
- ```<del>``` - Этот тег перечеркивает текст и используется для обозначения удаленных или устаревших частей текста.
- ```<abbr>``` - Этот тег используется для обозначения аббревиатур, и при наведении курсора показывает расшифровку аббревиатуры.
- ```<mark>``` - Этот тег используется для выделения текста ярким цветом, обычно для подчеркивания важных фрагментов текста.
- ```<i>``` - Устанавливает курсивное начертание шрифта.
- ```<u>``` - Этот тег подчеркивает текст и может использоваться для обозначения подчеркнутых слов или фраз.
- ```<span>``` - Универсальный тег, предназначенный для определения строчного элемента внутри документа.
- ```<sub>``` - Отображает шрифт в виде нижнего индекса. Текст при этом располагается ниже базовой линии остальных символов строки и уменьшенного размера — H<sub>2</sub>O.
- ```<sup>``` - Отображает шрифт в виде верхнего индекса. По своему действию похож на ```<sub>```, но текст отображается выше базовой линии текста — м<sup>2</sup>.
- ```<big>``` - Увеличенный текст.
- ```<small>``` - Уменьшенный текст.


## HTML: АТРИБУТЫ (ДОДЕЛАТЬ!)


