Service
======

Описание класса Service
-----------------------

Базовый абстрактный класс для создания сетевых сервисов. Обеспечивает управление сетевыми соединениями.

Методы класса
-------------

- ``__init__(self, ip_: str, port_: int, n_conn_=10)``:
  Инициализация сервиса с указанным IP-адресом, портом и максимальным количеством подключений.

- ``_do_job(self)``:
  Абстрактный метод, который должен быть реализован в производных классах. Определяет основную работу сервиса.

- ``_request_handler(self, request)``:
  Абстрактный метод для обработки входящих запросов.

- ``run_client(self, ip: str, port: int, request: str, response_handler: Optional[Callable] = None)``:
  Запуск клиента для взаимодействия с сервисом.

- ``start(self)``:
  Запуск сервиса и ожидание входящих подключений.

- ``stop(self)``:
  Остановка работы сервиса.

- ``pause(self)``:
  Пауза в работе сервиса.

- ``unpause(self)``:
  Возобновление работы сервиса после паузы.

- ``restart(self)``:
  Перезапуск сервиса.

