---
date: 2020-06-30T21:32:11+03:00
modified: 2021-09-05T10:59:16+03:00
title: Markdown. Упрощенный язык разметки текста
---

Здесь краткая инфа по markdown - упрощенному языку разметки документов. Он компилится в HTML. В сыром виде тоже сохраняет человекочитаемость. Используется повсеместно, где нужно писать много и по сути.  
Для преобразования из .md в .html используется [**kramdown**](https://devhints.io/kramdown)

* Навигация по разделам
{:toc}

## Общее

Здесь немножко о переменных и других програмных фишках, которые использует компилятор страниц на GitHub Pages.

При публикации страниц на Github Pages - HTML так и остается в исходном формате, а вот Markdown-файлы преобразовываются в HTML.  
Преобразование происходит с помощью Jekyll - это генератор статических сайтов. Широко используется там где не нужно динамически менять контент. Позволяет сэкономить тонну ресурсов на поддержание сервера.

Существуют аналоги:  Например Hugo. (больше можете нагуглить)  
Все они как и Jekyll могут быть установлены на локальную машину для преобразования локальных файлов в HTML пригодный для публдикации.  Но я считаю что Markdown уже пригоден для публикации, это его основная фишка - сохранение читаемости в нескомпилированном виде. А поэтому предпочитаю предоставить процесс сборки страниц серверам ГитХаба. Тем более это бесплатно и дает преимущество в виде возможности исполшьзовать сам GitHub в качестве CMS для ручного редактирования контента на сайте с любого устройства где есть браузер.

В Jekyll и на Github Pages можно менять предпочтительный метод компиляции файлов markdown путем изменения конфигурации в файле \_config.yml. Я оставил kramdown, поскольку лень.
* kramdown (по умолчанию)
* CommonMarkGhPages (как на самом гитхаб)
* (добавить)

## Шпаргалка Markdown


**[Markdown][1]{: rel="nofollow"}** — это облегченный язык разметки, призванный облегчить подготовку текстов для публикации в Интернете. Был создан для удобства чтения и написания размеченных текстов. Движок markdown генерирует валидный XHTML. Авторы - John Gruber и Aaron Swartz. 
Собственно, Markdown — это простой текст. 

**Jekyll** использует *markdown* нативно, вообще данный язык разметки очень любят на *[GitHub][2]{: rel="nofollow"}*, используют его везде, где только
можно (и в комментариях, и в отчетах, и в readme файлах). Данный блог использует *jekyll*, потому этот пост - это маленькая шпаргалка по Markdown.
 
### Синтаксис
Оригинальное описание синтаксиса находится здесь (англ.): <http://daringfireball.net/projects/markdown/syntax>{: rel="nofollow"}
 
Ниже следует краткое описание синтаксиса.
 
* Абзацы разделяются пустой строкой
* Два или более пробела на конце строки задают разрыв строки
* Шрифты: **жирный**: `**жирный**`, _курсив_:`_курсив_`, ***жирный и курсив***: `***жирный и курсив***`, `моноширинный`:`` `моноширинный` ``
* Заголовки:
  + Atx-style: `#первый уровень#`, `##второй уровень##` и т.д.
  + Setext-style: подчеркивание знаками `=` задает первый уровень, дефисами `-` — второй
* Цитаты: `> текст цитаты`
* Списки:
  + неупорядоченные: `* элемент списка` (также могут использоваться символы `-` или `+`).
  + упорядоченные: `1. элемент списка`
* Блок кода — каждая строка начинается с 4 или более пробелов
* Горизонтальная черта: три или более дефиса или звездочки
* Ссылки:
  + встроенные `[label](url "url title")`
  + автоматические `<url>`
  + в виде сносок
* Изображения:
  + встроенные `![alt text](url "image title")`
  + в виде сносок
* Экранирование символов — чтобы вставить спецсимвол, используемый в разметке, как обычный символ, его нужно предварить
символом обратной косой черты. Экранироваться должны следующие символы: `* _ { } [ ] ( ) # + - . !` 

Таблицы:  

        | First Header  | Second Header |
        | ------------- | ------------- |
        | Row1 Cell1    | Row1 Cell2    |
        | Row2 Cell1    | Row2 Cell2    |  

Результат:

| First Header  | Second Header |
| ------------- | ------------- |
| Row1 Cell1    | Row1 Cell2    |
| Row2 Cell1    | Row2 Cell2    |

Наглядная визуальная шпаргалка:
![image_picker4286818869274656233](https://user-images.githubusercontent.com/17731587/140794493-35babddd-9bfb-4fb6-a26f-3c3f89ff9ce4.jpg)


[1]: http://ru.wikipedia.org/wiki/Markdown "Markdown"
[2]: https://www.github.com/ "GitHub"




## Полезные ссылки
- [официальная дока от github](https://guides.github.com/features/mastering-markdown/)
- kramdown: <https://kramdown.gettalong.org/converter/html.html>  
- <http://bustep.ru/markdown/shpargalka-po-markdown.html#tables>
- на русском <https://gist.github.com/Jekins/2bf2d0638163f1294637>
