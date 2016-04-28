# Руководство для пользователей, участвующих в редактировании технической документации Azure

Вы попали в репозиторий GitHub, в котором хранится техническая документация, публикуемая в центре документации Azure по адресу [http://azure.microsoft.com/documentation](http://azure.microsoft.com/documentation).

Этот репозиторий также содержит рекомендации по редактированию технической документации. Список статей, которые входят в руководство для пользователей, участвующих в редактировании документации, можно просмотреть в [указателе](https://github.com/Azure/azure-content/blob/master/contributor-guide/contributor-guide-index.md).

## Редактирование документации Azure

Благодарим вас за проявленный интерес к документации Azure.

* [Варианты участия в наполнении документации](#ways-to-contribute)
* [Внесение изменений в содержимое Azure](#about-your-contributions-to-azure-content)
* [Организация репозитория](#repository-organization)
* [Использование GitHub, Git и этого репозитория](#use-github-git-and-this-repository)
* [Использование разметки Markdown для форматирования статьи](#how-to-use-markdown-to-format-your-topic)
* [Дополнительные ресурсы](#more-resources)
* [Указатель всех статей руководства по редактированию документации](./contributor-guide/contributor-guide-index.md) (открывается новая страница)

## Варианты участия в наполнении документации

Дополняйте технические статьи через пользовательский интерфейс GitHub. Найдите нужную статью в этом репозитории или откройте ее на сайте [http://azure.microsoft.com/documentation](http://azure.microsoft.com/documentation) и щелкните ссылку на источник в репозитории GitHub.

##Внесение изменений в содержимое Azure

###Незначительные исправления

Порядок внесения незначительных исправлений или уточнений в документацию и примеры кода из этого репозитория описаны в [условиях использования веб-сайта Azure](http://azure.microsoft.com/support/legal/website-terms-of-use/).


###Значительные изменения

Если вы отправляете запрос на внесение значительных изменений в существующую документацию и примеры кода, в комментариях на сайте GitHub мы попросим вас принять условия лицензионного соглашения участника (CLA). Лицензионное соглашение предлагается всем, кто подпадает под одну из таких категорий:

* члены группы Microsoft Open Technologies;
* участники, не работающие в корпорации Майкрософт.

Вам нужно заполнить интерактивную форму, после чего мы сможем принять ваш запрос на внесение изменений.

Подробные сведения можно найти по адресу [http://azure.github.io/guidelines.html#cla](http://azure.github.io/guidelines.html#cla).

## Организация репозитория

Репозиторий содержимого для Azure организован так же, как документация на сайте [Azure.Microsoft.com](http://azure.microsoft.com). Этот репозиторий содержит две корневые папки:

### \articles

В папке *\articles* содержатся статьи в формате Markdown (файлы с расширением *.md*).

Статьи в корневом каталоге публикуются на сайте Azure.Microsoft.com по адресу *http://azure.microsoft.com/documentation/articles/{article-name-without-md}/*.

* **Имена файлов статей**. См. [руководство по именованию файлов](./contributor-guide/file-names-and-locations.md).

Статьи в служебных папках публикуются на сайте Azure.Microsoft.com по адресу 
*http://azure.microsoft.com/documentation/articles/service-folder/{article-name-without-md}/*.

* **Подпапки для содержимого мультимедиа**. Папка *\articles* содержит папку *\media*, предназначенную для файлов мультимедиа из статей корневого каталога. В папке media хранятся вложенные папки с изображениями для каждой статьи. В служебных папках есть отдельная папка media для статей из каждой служебной папки. Папка с изображениями для статьи называется так же, как и файл статьи, но без расширения *.md*.

### \includes

Вы можете создавать содержимое, которое будет использоваться в нескольких статьях. См. статью [Пользовательские расширения, используемые в наших технических статьях](./contributor-guide/custom-markdown-extensions.md).

### \markdown templates

Эта папка содержит наш стандартный шаблон с основными элементами разметки Markdown, которые могут понадобиться для форматирования статьи.

### \contributor-guide

В этой папке хранятся статьи, которые относятся к руководству по редактированию документации.

## Использование GitHub, Git и этого репозитория

Сведения о том, как участвовать в редактировании, вносить небольшие изменения с помощью пользовательского интерфейса GitHub, создавать отдельные ветви репозитория или клонировать его для более значительных изменений, см. в статье [Установка и настройка средств для создания документации в GitHub](./contributor-guide/tools-and-setup.md).

Если вы установили GitBash и работаете локально, шаги по созданию новой локальной ветви, внесению изменений и их отправке обратно в главную ветвь см. в статье [Команды Git для создания новой или обновления существующей статьи](./contributor-guide/git-commands-for-master.md).

### Ветви

Мы рекомендуем создавать локальные рабочие ветви, в которые входит только определенный тип изменений. Каждая ветвь должна относиться только к одной концепции или статье, что позволит не только оптимизировать рабочий процесс, но и снизить вероятность конфликтов при слиянии. Вот несколько примеров того, когда целесообразно создавать новую ветвь:

* добавление новой статьи (и связанных с ней изображений);
* исправление орфографических и грамматических ошибок в статье;
* унификация форматирования в большом наборе статей (например, добавление нового нижнего колонтитула с информацией об авторских правах).

## Использование разметки Markdown для форматирования статьи

Во всех статьях в этом репозитории используется разметка Markdown, принятая для GitHub. Вот список полезных ресурсов:

- [Основные сведения о разметке Markdown.](https://help.github.com/articles/markdown-basics/)

- [Подсказки по разметке Markdown в печатном формате.](./contributor-guide/media/documents/markdown-cheatsheet.pdf?raw=true)

- Наш список редакторов для Markdown см. в статье [Установка и настройка средств для создания документации в GitHub](./contributor-guide/tools-and-setup.md#install-a-markdown-editor).

## Метаданные статьи

Метаданные статьи предоставляют на веб-сайте azure.microsoft.com некоторые дополнительные возможности. В частности, вы можете указать ссылки на автора и участника, настроить строку навигации, добавить описание статьи и текст для оптимизации поисковой системы. Метаданные также позволяют Майкрософт оценивать содержимое по различным показателям. Как вы видите, метаданные имеют большое значение. [Здесь представлено руководство по проверке правильности метаданных](./contributor-guide/article-metadata.md).

## Дополнительные ресурсы

Список всех статей этого руководства приведен в [указателе](./contributor-guide/contributor-guide-index.md).

<!---HONumber=AcomDC_0307_2016-->