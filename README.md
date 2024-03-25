сылка для тестирования: curl http://arch.homework/otusapp/denisfrunza/health



Предварительные требования

Перед тем, как начать, убедитесь, что у вас установлены:
    Helm 3.x+


Установка Чарта

Для установки чарта с именем релиза my-release:

helm install my-release /path/to/chart -f /path/to/custom/values.yaml -n otus --create-namespace


http://arch.homework/user/

Создать юзера:

    curl -X POST http://arch.homework/user      -H 'Content-Type: application/json'      -d '{
    "username": "johndoe",
    "firstName": "John",
    "lastName": "Doe",
    "email": "john.doe@example.com",
    "phone": "123-456-7890"
    }'

Получить юзера:
    curl -X GET http://arch.homework/user/<user_id>

Удалить юзера:
    curl -X DELETE http://arch.homework/user/<user_id>

Обновить
curl -X PUT -H "Content-Type: application/json" -d '{
    "username": "alicedoe",
    "firstName": "Alice",
    "lastName": "Doe",
    "email": "alice.doe@example.com"
}' http://arch.homework/user/<user_id>
