# Deploy
kubectl apply -f config.yaml -f postgres.yaml -f initdb.yaml -f deployment.yaml -f service.yaml -f ingress.yaml

##Паттерн кеширования
Данные хранятся в ОЗУ.
Инвалидация происходит по событию.

##Включение/отключение кэширования
Через переменную окружения CACHE_ENABLED
- включен: CACHE_ENABLED = 1
- отключен: CACHE_ENABLED != 1