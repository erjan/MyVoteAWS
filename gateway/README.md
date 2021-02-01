# API Gateway

Постарайтесь сконфигурировать API Gateway самостоятельно, используя знания из недавнего модуля. Подсказки можно подсмотреть ниже. 

## Настройки CORS

Настройки Cross-Origin запросов. Обратите внимание, что разрешены и GET, и POST запросы (на запись голоса и получение результатов), а так же подключены два источника запросов: my-vote (голосование) и my-vote-result (результаты). 

![image](https://user-images.githubusercontent.com/1742301/106400513-1b512a80-641f-11eb-8a07-c05b55ca3857.png)

## Маршруты

В данном примере я использовал один путь `/my-vote`, а маршрутизацию сделал на основе метода запроса `GET`/`POST`. Это не является обязательным, можно сделать два разных пути.

![image](https://user-images.githubusercontent.com/1742301/106399262-dfff2d80-6417-11eb-9222-45eea37637e2.png)

## Интеграции

Этот API должен поддерживать в качестве интеграций две функции из AWS Lambda. В этом репозитории приведён их код:

* [Бэкенд голосованя](../voting-backend)
* [Бэкенд результатов](../result-backend)