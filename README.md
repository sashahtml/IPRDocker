# 1
Команды запуска:
docker build -t counter-app .
docker run -d --name my-counter -p 8080:8000 -e GREETING="пр" counter-app

Проверка и логи сохранены в файле 1.txt.

## 2
Запуск: docker compose up -d
Остановка: docker compose down.

Проверка сохранения данных:
1. Сделали POST-запросы (счетчик увеличился до N).
2. Выполнили docker compose down.
3. Выполнили docker compose up -d.
4. Счетчик остался равен N. Данные сохраняются в volume counter-data.
Логи сохранены в 2.txt.