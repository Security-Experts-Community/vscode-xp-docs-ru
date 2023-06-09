﻿## Поддержка языка XP в Visual Studio Code

Язык eXtraction and Processing (XP) используется для создания правил преобразования данных в процессе обработки событий. На языке XP вы можете разрабатывать правила нормализации, корреляции и обогащения событий.

Это расширение позволяет разрабатывать и тестировать правила в VSCode и VSCodium, а также публиковать их в необходимом для вашего продукта формате.

Руководство по работе с расширением: [https://vscode-xp.readthedocs.io/](https://vscode-xp.readthedocs.io/)

### Основные возможности

Возможности расширения:
* Просмотр и редактирование правил нормализации, агрегации, корреляции, обогащения и табличных списков.
* Создание из готовых шаблонов правил нормализации, корреляции, обогащения.
* Просмотр, редактирование и создание интеграционных и модульных тестов для правил нормализации, корреляции и обогащения.
* Автоматическое дополнение ключевых слов, функций и типовых конструкций языка XP и полей таксономии.
* Статическая валидация исходного кода на типичные ошибки.
* Заполнение метаданных правил.
* Создание и редактирование правил локализации.
* Сбор графов правил, схемы и БД табличных списков (нужны дополнительные утилиты).
* Проверка срабатываний всего графа корреляций на необработанные события (нужны дополнительные утилиты).
* Импорт и экспорт пакетов экспертизы в файлы формата KB (нужны дополнительные утилиты).

***Примечание.** Для ряда операций расширение использует дополнительные утилиты [из отдельного репозитория](https://github.com/vxcontrol/xp-kbt/releases).*

### Разработчикам

Разработкой расширения занимается сообщество [Security Experts Community](https://github.com/Security-Experts-Community). Вы можете принять участие в проекте и внести свой вклад. Актуальный список задач проекта публикуется [в репозиториях](4507244939#4507248395).

#### Компиляция

Чтобы скомпилировать расширение:

1. Установите [VSCode](https://code.visualstudio.com/).

1. Установите [Node.js](https://nodejs.org/).

1. Создайте локальную копию репозитория:

   ```
   git clone <Адрес проекта>
   ```

   Например:

   ```
   git clone https://github.com/Security-Experts-Community/vscode-xp
   ```

1. В корне проекта выполните команду `npm install`.

#### <a name="4507248395"></a>Репозитории

Основной на GitHub: [https://github.com/Security-Experts-Community/vscode-xp](https://github.com/Security-Experts-Community/vscode-xp)

Зеркало на Codeberg: [https://codeberg.org/Security-Experts-Community/vscode-xp](https://codeberg.org/Security-Experts-Community/vscode-xp)

Зеркало на GitFlic: [https://gitflic.ru/project/security-experts-community/vscode-xp](https://gitflic.ru/project/security-experts-community/vscode-xp)

#### Публикация

Перед публикацией расширения вам нужно в корне проекта выполнить команду `npm install -g vsce`.

Чтобы опубликовать расширение,

1. выполните команду `vsce package -o xpContentEditor.vsix` или запустите скрипт `publish.py` в корне проекта.
