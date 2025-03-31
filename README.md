# Russian Stocks Price Database

![PostgreSQL Version](https://img.shields.io/badge/postgresql-17.4-blue)
![Python Version](https://img.shields.io/badge/python-3.8-blue)

## 📑 Описание проекта

Russian Stocks Price Database — это проект, направленный на сбор, хранение и анализ данных о стоимости акций российских компаний. Цель проекта — предоставить доступный и удобный инструмент для инвесторов, аналитиков и исследователей, позволяющий отслеживать изменения на рынке акций и принимать обоснованные решения. Он позволяет добавлять, обновлять, удалять и запрашивать стоимость акций с использованием SQL-запросов. Проект построен с использованием **PostgreSQL** и **Python** для управления базой данных.

## 🧰 Основные функции

**Сбор данных**: Автоматическое обновление данных о стоимости акций с ведущих финансовых платформ.
**Хранение данных**: Использование реляционной базы данных для эффективного хранения и управления данными.
**Аналитика**: Возможность выполнения базовых аналитических операций, таких как расчет доходности, волатильности и корреляции.
**Экспорт данных**: Возможность экспорта данных в различных форматах (CSV, Excel) для дальнейшего анализа.

## ⚙️ Технологии

**Языки программирования**: Python, SQL
**База данных**: PostgreSQL
**Фреймворки и библиотеки**: Pandas, NumPy, Matplotlib, Django
**Инструменты**: Git, Docker

## ✈️ Установка и запуск

1. Клонируйте репозиторий:

```bash
git clone https://github.com/yourusername/russian-stocks-price-db.git
```

2. Установите зависимости:

```bash
pip install -r requirements.txt
```

3. Настройте базу данных и запустите сервер:

```bash
python manage.py migrate
python manage.py runserver
```

## 🎰 Примеры использования

Получение данных о стоимости акций:

```bash
from database import get_stock_price

price = get_stock_price('AAPL', '2023-01-01')
print(f"Стоимость акции AAPL на 2023-01-01: {price}")
```

Расчет доходности:

```bash
from analysis import calculate_return

return_value = calculate_return('AAPL', '2023-01-01', '2023-12-31')
print(f"Доходность акции AAPL за 2023 год: {return_value}%")
```