[FinalTaskFirstSprint-main.zip](https://github.com/user-attachments/files/18223084/FinalTaskFirstSprint-main.zip)
Всё решение там
# Сервис подсчёта арифметических выражений
## О проекте
Веб-сервис: пользователь отправляет арифметическое выражение по протоколу HTTP и получает в ответ его результат. Калькулятор обрабатывает только однозначные числа, скобки вида '(' ')' и арифметические операции:
1) Сложение (+)
2) Вычитание (-)
3) Умножение (*)
4) Деление (/)

В случае с неоднозначными числами и арифметическими операциями, не входящими в этот список, сервис выдаст ошибку: {«ошибка»: «Выражение неверно»}

Не обрабатываются отрицательные числа.

Также веб-сервис не обрабатывает выражения, содержащие символы английского, русского или других языков.

Обработка выражений с пробелами производится корректно.
## Технологии и библиотеки
Веб-сервис написан на языке Go и использует следующие библиотеки и инструменты:

Язык программирования:
* Go (версия 1.23.2)
### Основные библиотеки:
* **net/http:** Базовый HTTP-сервер для обработки запросов.
* **errors:** Библиотека для работы с ошибками.
* **io:** Базовые интерфейсы для работы с вводом и выводом.
* **bytes:** Утилиты для работы с байтовыми срезами.
* **encoding/json:** Кодирование и декодирование JSON.
* **fmt:** Форматированный ввод/вывод.
* **net/http/httptest:** Инструменты для тестирования HTTP-серверов и клиентов.
* **testing:** Предоставляет инструменты для написания и организации модульных, интеграционных и нагрузочных тестов.
* **strings:** Утилиты для работы со строками.
* **strconv:** Преобразование строк в числа, булевые значения и обратно.
* **unicode:** Работа с символами Unicode.
* **os:** Работа с операционной системой.
## Архитектура проекта
* **cmd/**
  * **main.go**
* **internal/**
  * **application/**
* **pkg/**
  * **calculation/**
    * **calculation.go**
    * **errors.go**
    * **calculation_test.go**
