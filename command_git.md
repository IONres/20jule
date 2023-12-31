# Git ***(ИЗМЕНЕНИЕ)***
>**Git** — абсолютный лидер по популярности среди современных систем управления версиями. Это развитый проект с активной поддержкой и открытым исходным кодом. Система Git была изначально разработана в 2005 году **Линусом Торвальдсом** — создателем ядра операционной системы Linux. Git применяется для управления версиями в рамках колоссального количества проектов по разработке ПО, как коммерческих, так и с открытым исходным кодом. Система используется множеством профессиональных разработчиков программного обеспечения. Она превосходно работает под управлением различных операционных систем и может применяться со множеством интегрированных сред разработки (IDE).

Источник: <https://www.atlassian.com/ru/git/tutorials>

## Команды git
|Команда|Назначение |Описание команды|
|:-:|:-:|:-|
|**Настройка репозитория**|
|`git init`|инициализация нового репозитория|для создания нового репозитория используется команда `git init`. Команду `git init` выполняют только один раз для первоначальной настройки нового репозитория. Выполнение команды приведет к созданию нового подкаталога ``.git`` в вашем рабочем каталоге. Кроме того, будет создана новая главная ветка|
|`git clone`|клонирование существующего репозитория|команду `git clone` выполняют для создания копии (клонирования) удаленного репозитория. В качестве параметра в команду `git clone` передается URL-адрес репозитория. Git поддерживает несколько различных сетевых протоколов и соответствующих форматов URL-адресов. Подробнее  <https://www.atlassian.com/ru/git/tutorials/setting-up-a-repository>
|`git push`|совместная работа в разных репозиториях| команда `git push` используется для выгрузки содержимого локального репозитория в удаленный репозиторий. Она позволяет передать коммиты из локального репозитория в удаленный. Подробнее <https://www.atlassian.com/ru/git/tutorials/syncing/git-push>|
|`git config`|конфигурирование и настройка|используется для настройки значений конфигурации Git на глобальном и локальном уровнях проекта. Эти уровни конфигурации соответствуют текстовым файлам ``.gitconfig`` . При выполнении команды git ``config`` происходит изменение текстового файла конфигурации. Подробнее  <https://www.atlassian.com/ru/git/tutorials/setting-up-a-repository/git-config>|
|`git remote`|конфигурирование и настройка|команда `git remote` позволяет создавать, просматривать и удалять подключения к другим репозиториям. Удаленные подключения скорее похожи на закладки, чем на прямые ссылки на другие репозитории. Они служат удобными именами, с помощью которых можно сослаться на не очень удобный URL-адрес, а не предоставляют доступ к другому репозиторию в режиме реального времени. Подробнее <https://www.atlassian.com/ru/git/tutorials/syncing>|
**Сохранение изменений**
|`git add`|индексирование|команда `git add` добавляет изменение из рабочего каталога в раздел проиндексированных файлов. Она сообщает Git, что вы хотите включить изменения в конкретном файле в следующий коммит. Однако на самом деле команда `git add` не оказывает существенного влияния на репозиторий: изменения регистрируются в нем только после выполнения команды `git commit`.
|`git commit`|сохранение|команда `git commit`, добавляет проиндексированный снимок состояния в историю проекта.
|**Проверка репозитория**|
|`git status`|проверка| команда `git status` отображает состояние рабочего каталога и раздела проиндексированных файлов. С ее помощью можно проверить индексацию изменений и увидеть файлы, которые не отслеживаются Git. Информация об истории коммитов проекта ***НЕ*** отображается при выводе данных о состоянии. Для этого используется команда `git log`
|`git log`|история коммитов|команда `git log` отображает отправленные снимки состояния и позволяет просматривать и фильтровать историю проекта, а также проводить поиск по ней.
|`git tag`|точечная история|теги — это ссылки, указывающие на определенные точки в истории Git. Команда `git tag` обычно используется для захвата некой точки в истории, которая используется для релиза нумерованной версии (например, v1.0.1).
|`git blame`|отображение метаданных|общее назначение `git blame` — отображение метаданных автора, связанных со строками, которые были внесены в файл при коммите. Таким образом можно проследить историю кода и выяснить, какой именно код был внесен в репозиторий, как это было сделано и по какой причине.
**Отмена изменений**
|`git checkout`|переходов и просмотра истории коммитов|команда `git checkout` позволяет перемещаться между ветками, созданными командой git branch . При переключении ветки происходит обновление файлов в рабочем каталоге в соответствии с версией, хранящейся в этой ветке, а Git начинает записывать все новые коммиты в этой ветке.
|`git revert`|отмена общих публичных изменений|операция для безопасной отмены изменений, действие которой направлено в будущее. Для отката изменений команда не удаляет из истории коммиты или родительские элементы, a создает новый коммит с отменой нужных действий.
|`git reset`|отмена локальных частных изменений|Команда `git reset` — это сложный универсальный инструмент для отмены изменений. Она имеет три основные формы вызова, соответствующие аргументам командной строки `--soft`, `--mixed`, `--hard`. Каждый из этих трех аргументов соответствует трем внутренним механизмам управления состоянием Git: дереву коммитов (HEAD), разделу проиндексированных файлов и рабочему каталогу.


*таблица составлена по <https://www.atlassian.com/ru/git/tutorials>*
