Лабораторная работа №6: Автоматизация тестирования веб-форм с использованием Selenium WebDriver

Описание проекта
Автоматизированные тесты для проверки функциональности поиска на сайте Яндекс с использованием:
- Selenium WebDriver
- Паттерна Page Object Model (POM)
- Фреймворка pytest
- Системы отчётности Allure

Технологический стек
- Python 3.8+
- Selenium WebDriver
- pytest + pytest-xdist
- Allure Framework
- webdriver-manager (автоматическая установка драйвера)

Установка зависимостей
1. Клонируйте репозиторий
2. Создайте и активируйте виртуальное окружение (рекомендуется):
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate  # macOS / Linux

Запуск тестов

Обычный запуск
python3 -m pytest tests/test_yandex_form.py -v

Параллельный запуск (2 потока)
python3 -m pytest tests/test_yandex_form.py -n 2 -v

Запуск с генерацией Allure-отчёта
allure generate allure-results --clean -o allure-report
