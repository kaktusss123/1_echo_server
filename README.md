# Простенький клиент-сервер

- Запуск сервера, потом клиента
- Сервер сообщит о параметрах для подключения
- Все логи выводятся соответственно в server.log и client.log
- Отключение клиента по ключевому слову `exit`
- Пароли сохраняются в md5

Сервер работает одновременно с двумя клиентами, но обновление сообщений происходит только при запуске. Множественная отправка-получение недоступны, только последовательно получил-отправил-получил.

## Данные для тестового входа

Login:      vladik  
Password:   12345


Login:      vladik1  
Password:   12345

## Отправка и прием сообщений

Чтобы отправить сообщение, достаточно послать серверу 
```python
    sendto username message
```
