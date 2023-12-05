.. _objectDetectionService:

Object Detection Service
========================

Добро пожаловать в документацию Object Detection Service!

Общее описание
--------------

Object Detection Service - это программный сервис, предназначенный для определения, является ли объект перед камерой живым, и для распознавания объектов с использованием YOLOv5.

Требования
----------

- Python версии 3.9 или выше.

Установка и запуск
------------------

1. Склонировать ветку проекта.
2. Выполнить в консоли команду для настройки окружения:

   .. code-block:: bash

      pip install -r requirements.txt

3. Запустить сервис командой:

   .. code-block:: bash

      python run.py

   При первом запуске автоматически скачаются веса для YOLOv5.

Классы и методы

.. toctree::
   :maxdepth: 2


   service
   service_od
   camera
