# @read_books_bro_bot


Находиться в стадии разработки, есть начальный репозиторий, 
[Bookstore_Program](https://github.com/Not-user-1984/Bookstore_Program)

### Идея проекта

Идея проекта сначала это был pet - project простое API для резюме типа смотрите, я знаю fast api и пишу асинхронно , но он быстро мне наскучил и по сути, был еще одной интерпретацией на тему API  магазин , блог и прочие .

 Подумав, я решил, что сделать полезное для себя,  пришел к такой идеи.
 Главная идея это телеграмм бот решает такие задачи:

1. Напоминать читать книгу
2. Показать прогресс чтения
3. Делать заметки по каждой прочитанной главе книге
4. Можно добавлять книгу самому
5. Добалять книгу из база данных книг , что было с чего начать ( на ранних этапах она простая и небольшая)
6. Также можно будет скачать свои заметки по книгам,  думаю в Markdown файл(что бы можно было интегрировать в Obsidian)
 
 



### Запуск
``` cmd
cd infra
развернуть базу данных через докер
docker compose up -d --build
залить по желанию свои данные в .env

установить витруалку и все зависимости

запуск FastAPI
cd src
uvicorn main:app --reload

запуск tg-bot:
cd telegram_bot
python main.py

дока к api тут:
http://127.0.0.1:8000/docs/

```

- [x] api Подключение базы, миграции и urls.
- [x] api grud проекта(асинхронно, пока создание Book не работает)
- [x] tg-bot работает регистрация.
- [ ] tg-bot работает вход.
- [ ] tg-bot работает добавление книги.




