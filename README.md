# Библиотека всяких полезностей

1. [HTML&CSS](#htmlcss)
2. [JavaScript](#javascript)
3. [Automation](#automation)
4. [Design](#design)

## HTML&CSS

* [HTML5 Boilerplate](https://html5boilerplate.com) - стартовый шаблон для верстки.
* [Центрирование в CSS: полное руководство](http://frontender.info/centering-css-complete-guide/) - подробная статья.
* [Центрирование в CSS](http://howtocenterincss.com) - подбор нужного способа центрирования в зависимости от ситуации.

### Эффекты

* [Эффекты клика](http://tympanus.net/Development/ClickEffects/)

## JavaScript

* [fullPage.js](http://alvarotrigo.com/fullPage/#firstPage) - плагин для прокрутки в виде слайдов.
* [liMarquee](http://masscode.ru/index.php/k2/item/44-limarquee) - бегущая строка на jQuery.

## Automation

* [Grunt для начинающих](http://frontender.info/a-beginners-guide-to-grunt-redux/) - руководство по использованию Grunt для начинающих: пересмотренное издание.
* [Приятная сборка frontend проекта](http://habrahabr.ru/post/250569/) - организация сборки проекта на Gulp.
* [Оптимизация производительности веб-страниц:CSS](http://forwebdev.ru/css/optimiziruem-proizvoditelnost-veb-stranicy-css/) - в том числе при помощи автоматизации.

## Design

* [Pixabay](https://pixabay.com/ru/) - один из лучших фотостоков.
* [Prototype Tools](https://xakep.ru/2014/09/09/prototype-tools/) - обзор инструментов для прототипирования пользовательских интерфейсов.




# Пример форматирования

# HTML Inspector

1. [Getting Started](#getting-started)
2. [Configuring HTML Inspector](#configuring-html-inspector)
3. [Built-in Rules](#built-in-rules)

## Getting Started

The easiest way to try out HTML Inspector is to link to the source file hosted on [CDNJS](http://cdnjs.com/):

```html
<script src="http://cdnjs.cloudflare.com/ajax/libs/html-inspector/0.8.2/html-inspector.js"></script>
```

It can also be installed

The `inspect` method takes a config object to allow you to change any of this behavior. Here are the config options:

- **domRoot**: (selector | element) the DOM element to start traversing from
- **useRules**: (Array) a list of rule names to run when inspecting. Defaults to running all rules not excluded via `excludeRules`

### Best Practices

Some markup may be perfectly valid but uses practices that are commonly considered to be poor or outdated. The following rules check for these types of things. (Note that everything in this list is subjective and optional.)

*(Note: there are a few different BEM naming conventions out there. HTML Inspector support the [three most common](https://github.com/philipwalton/html-inspector/blob/master/src/rules/convention/bem-conventions.js#L3-L29))*

## Third Party Rules

- [Large Viewstate](https://github.com/palewar/html-inspector/blob/master/src/rules/best-practices/large-viewstate.js) - warn if View State takes up more than 50KB (configurable) in ASP.NET generated HTML
- [Voice Input](https://googledrive.com/host/0B8yu2s4Q9YD8VEZNUHJaV3BkSzA/File.htm) - warn when input fields are inaccessible to voice input

folowing:

	a {
		font-family: Arial;
		font-style: italic;
		font-size: 14px;
		line-height: 18px;
		font-weight: bold;
		background-image: url('example.png');
		background-color: red;
		background-size: cover;
		background-repeat: no-repeat;
	}

	=>

    a {
      font: italic bold 14px/18px Arial;
      background: red url('example.png') no-repeat / cover;
    }

##HTML&CSS
[autoprefixer](https://github.com/postcss/autoprefixer) - parse CSS and add vendor prefixes to rules by Can I Use.


* [gulp-less](https://github.com/plus3network/gulp-less) - LESS in CSS.
* [gulp-sass](https://github.com/dlmanning/gulp-sass) - SASS/SCSS in СSS.

<p align="right">
<a href="README.md">English description</a> | Описание на русском
</p>

Далее необходимо установить gulp глобально. (Возможно потребуются права суперюзера или администратора)

```shell
npm install -g gulp
```

Ключи, доступные при любом режиме сборки:

* `--ie8` – включить в сборку стили для ie8.
* `--ie9` – включить в сборку стили для ie9.
* `--ie` – включить в сборку стили для ie9 и ie8.

`gulp update-deps` – обновление всех зависимостей сборщика до последних стабильных. Может потребоваться какое-то время на выполнение данной команды. Желательно выполнять раз в неделю. Команда скопирует текущий package.json, добавит к его имени подчеркивание, скачает новый package.json с репозитория и выполнит npm install. Таким образом, если у вас что-то сломалось с новыми пакетами, то всегда можно вернуться на прошлую версию, просто вернув прошлый package.json