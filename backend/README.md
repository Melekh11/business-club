# business-club backend

## Почему база данных не в проекте с ботом?
На мой взгляд сайт интересней и сложнее, чем бот. Взял из заданий самое сложное и совметил в одну задачу.

## Простейшая система безопасности
При регистрации сервис отправляет токен, который при последующих запросах используется для аутентификации (должен быть отправлен в заголовке запроса).
В продвинутой реализации этот токен должен обновляться с какой-то периодиночтью, чтобы не дать много времени злоумышленнику, укравшему ваш токен.
Также злоумышленник не может украсть ваш пароль, ведь вы обмениваетесь с сервисом только обновляемым токеном, а не хэшированным паролем.

## PG-Admin
Для удобного просмотра данных docker-compose поднимает сервер админки, через который удобно отслеживать изменения DB.
