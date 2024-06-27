# JS-Practice-HTTP
задание по модулю HTTP
полученные статусы ответов:
200 OK - https://api.openweathermap.org/data/2.5/weather?lat=54.52&lon=28.41

400 "Nothing to geocode" - нет параметров
401 "Invalid API key. Please see https://openweathermap.org/faq#error401 for more info." - нет ключа API
404 "Not Found" - неправильное значение параметров
405 "Method Not Allowed" - если попытаться сделать PUT, PATCH, DELETE, OPTIONS запросы
429 "To Many Requests" - происходит на бесплатном варианте подписки, но так и не получилось получить этот код

500, 502, 503, 504 - может возвращать, но это ошибки сервера

Это все коды ответов, что описаны в https://openweathermap.org/faq#error
