# 🐘 Yii2 — Учебный проект на PHP Yii2

Проект на базе Yii2 Basic Template для изучения MVC-архитектуры на PHP и принципов работы с Yii2.

---

## Стек технологий

| Компонент | Технология |
|-----------|-----------|
| Backend | PHP 8.x, Yii2 |
| ORM | Active Record |
| База данных | MySQL |
| Тестирование | Codeception |
| Запуск | Docker Compose |

---

## Изученные концепции

- MVC-архитектура на Yii2
- Active Record: модели, связи, валидация
- Контроллеры и действия (actions)
- Представления (views) и виджеты
- Авторизация и регистрация
- Тестирование: unit, functional (Codeception)

---

## Запуск через Docker

```bash
docker-compose run --rm php composer install
docker-compose up -d
```

Приложение: **http://127.0.0.1:8000**

---

## Запуск без Docker

```bash
composer install

# Настройте config/db.php, затем:
mysql -u root -p yii2basic < yii2basic.sql

php yii serve
```

---

## Тесты

```bash
vendor/bin/codecept run
