# JS-Practice-HTTP
задание по модулю HTTP
полученные статусы ответов:

200 OK - https://api.openweathermap.org/data/2.5/weather?lat=54.52&lon=28.41

![image](https://github.com/N01ZY-D/JS-Practice-HTTP/assets/108016067/3d6b0f51-3a5e-4171-88a3-c91130600b6d)


400 "Nothing to geocode" - нет параметров (https://api.openweathermap.org/data/2.5/weather)
![image](https://github.com/N01ZY-D/JS-Practice-HTTP/assets/108016067/36d982f4-1cd9-4d30-9e43-c4e3daabec50)


401 "Invalid API key. Please see https://openweathermap.org/faq#error401 for more info." - нет ключа API или он неправильный (как в этом случае)
![image](https://github.com/N01ZY-D/JS-Practice-HTTP/assets/108016067/09c9c148-7eb4-41b3-9fa2-8fecc1a8fe17)


404 "Not Found" - неправильное значение параметров (https://api.openweathermap.org/data/2.5/weather?lat=55.52&lon=28.41&q=gffhgfhS)
![image](https://github.com/N01ZY-D/JS-Practice-HTTP/assets/108016067/19fa53be-c4bd-4f6c-86cf-87b15080c262)


405 "Method Not Allowed" - если попытаться сделать PUT, PATCH, DELETE, OPTIONS запросы
![image](https://github.com/N01ZY-D/JS-Practice-HTTP/assets/108016067/f3c8590a-61cc-4397-a576-631800855ac5)


429 "To Many Requests" - происходит на бесплатном варианте подписки, если обращаться чаще, чем положено планом подписки. Так и не получилось получить этот код

Коды 100-199 редки в стандартных HTTP-запросах, так как обычно используются в контексте более специфичных процессов, таких как вебсокеты или другие виды долгоживущих соединений.

Коды 300-399 также не получилось получить так как OpenWeatherAPI обычно не использует коды перенаправлений для запросов на получение данных о погоде, потому что: сервер API напрямую отвечает на запросы клиента; данные обычно доступны без необходимости перенаправлений; API сервисы, как правило, сконфигурированы для предоставления точного местоположения запрашиваемых ресурсов.

500, 502, 503, 504 - исходя из документации, API может возвращать, но это ошибки сервера, поэотому получить их в нормальных условиях почти невозможно

Это все коды ответов, что описаны в https://openweathermap.org/faq#error
