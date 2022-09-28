# Программа для работы с заметками Evernote с помощью python

Программа позволяет получать список заметок в консоль, копировать заметки и получать GUID и названия блокнотов с заметками 

## Запуск

- Скачайте код
- Для работы программы необходим интерпретатор python версии 2
- Установите зависимости командой `pip install -r requirements.txt`

### Модуль list-notebook

Выводит список блокнотов

- Запуск:
```
python list-notebooks.py
```

### Модуль add_note2journal.py

Копирует заметку

- Запуск:
```
python list-notebooks.py
```

### Модуль dump_nbox.py

Выводит список заметок в консоль

- Запуск:
```
python dump_inbox.py
```

### Модуль config.py

Содержит конфигурационные данные из переменных окружения

## Переменные окружения

Часть настроек проекта берётся из переменных окружения. Чтобы их определить, создайте файл `.env` в директории проекта и запишите туда данные в таком формате: `ПЕРЕМЕННАЯ=значение`.

Доступно 5 переменных:
- `EVERNOTE_CONSUMER_KEY` — API ключ для разработки. Получить можно [тут](https://dev.evernote.com/#apikey).
- `EVERNOTE_CONSUMER_SECRET` — получается вместе с ключом из предыдущего пункта.
- `EVERNOTE_PERSONAL_TOKEN` — токен разработчика для доступа evernote API к аккаунту с заметками. Получить можно по инструкции на этой [странице](https://dev.evernote.com/doc/articles/dev_tokens.php).
- `JOURNAL_TEMPLATE_NOTE_GUID` — [GUID](https://ru.wikipedia.org/wiki/GUID) заметки.
- `JOURNAL_NOTEBOOK_GUID` — [GUID](https://ru.wikipedia.org/wiki/GUID) блокнота с заметками.

## Цели проекта

Код написан в учебных целях — это урок в курсе по Python и веб-разработке на сайте [Devman](https://dvmn.org).

