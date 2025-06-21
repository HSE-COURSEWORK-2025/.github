Сервис для анализа данных с носимых датчиков для мониторинга здоровья. Платформа собирает, обрабатывает и визуализирует медицинские показатели, выявляет аномалии и прогнозирует риски для здоровья.

![Kubernetes](http://img.shields.io/badge/kubernetes-%23326ce5.svg?style=flat&logo=kubernetes&logoColor=white) ![Python](http://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54) ![React](http://img.shields.io/badge/react-%2320232a.svg?style=flat&logo=react&logoColor=%2361DAFB)

**Демо**: [http://hse-coursework-health.ru/](http://hse-coursework-health.ru/)
> Если сайт не открывается по доменному имени, пожалуйста, напишите автору в Telegram: [@igmalysh](https://t.me/igmalysh)

## 🎬 Демонстрация работы сервиса (тут gif большого размера, может сразу не прогрузиться)

<p align="center">
  <img src="https://raw.githubusercontent.com/HSE-COURSEWORK-2025/.github/main/demo.gif" alt="Demo GIF" width="600" />
</p>

## 🚀 Доступ к демо

### Для тестирования системы:
1. **Вы можете создать/войти в тестовый аккаунт на странице входа**
   - будут работать все функции, кроме выгрузки из Google Fitness API; можно будет выгружать данные со смартфона

2. **Доступ через Google OAuth**:
   - Для входа через Google аккаунт необходимо связаться с автором проекта
   - Автор добавит ваш email в whitelist Google Cloud Console
   - Контакт для доступа: [@igmalysh](https://t.me/igmalysh)

3. **Демо-аккаунт**
   — На странице входа просто нажмите кнопку **«Войти в демо-аккаунт»**.

## 🧩 Основные компоненты системы

### Пользовательские интерфейсы
- **Веб-приложение**: [http://hse-coursework-health.ru/](http://hse-coursework-health.ru/)
- **Мобильное приложение**: Доступно для Android 

<p align="center">
  <img src="https://github.com/HSE-COURSEWORK-2025/.github/blob/main/image.png?raw=true" alt="Мобильное приложение" width="300"  />
</p>

### API сервисы
| Сервис                | URL                                                    | Документация                                               |
|-----------------------|--------------------------------------------------------|------------------------------------------------------------|
| Auth API              | http://hse-coursework-health.ru/auth-api               | [Swagger](http://hse-coursework-health.ru/auth-api/docs)    |
| Data Collection API   | http://hse-coursework-health.ru/data-collection-api    | [Swagger](http://hse-coursework-health.ru/data-collection-api/docs) |
| Results Provider API  | http://hse-coursework-health.ru/results-provider       | [Swagger](http://hse-coursework-health.ru/results-provider/docs) |
| Notifications API     | http://hse-coursework-health.ru/notifications-api      | [Swagger](http://hse-coursework-health.ru/notifications-api/docs) |
| Ratings API           | http://hse-coursework-health.ru/ratings-api            | [Swagger](http://hse-coursework-health.ru/ratings-api/docs)  |

### Инструменты администрирования
| Инструмент            | URL                                                    | Доступ       |
|-----------------------|--------------------------------------------------------|--------------|
| Apache Airflow        | http://hse-coursework-health.ru/airflow                | `admin:admin`|
| Kafka UI              | http://hse-coursework-health.ru/kafka-ui               | Публичный    |
| Grafana               | http://hse-coursework-health.ru/grafana                | `admin:admin`|

> Если какой-то из сервисов не открывается, пожалуйста, напишите автору в Telegram: [@igmalysh](https://t.me/igmalysh)

## 🛠️ Технологический стек

- **Бекенд**: Python 3.10, FastAPI
- **Фронтенд**: React, TypeScript, Recharts
- **Мобильное приложение**: Kotlin, Android SDK
- **Базы данных**: PostgreSQL, Redis
- **Очереди**: Apache Kafka
- **Оркестрация**: Kubernetes, Docker
- **ML**: Scikit-learn, Pandas, NumPy
- **Мониторинг**: Grafana, Prometheus

## 🗂️ Репозитории проекта

### API-сервисы
| Репозиторий | Описание |
|-------------|----------|
| [hse-coursework-auth-api](https://github.com/HSE-COURSEWORK-2025/hse-coursework-auth-api) | Сервис аутентификации и авторизации пользователей |
| [hse-coursework-notifications-api](https://github.com/HSE-COURSEWORK-2025/hse-coursework-notifications-api) | Сервис для отправки уведомлений пользователям |
| [hse-coursework-backend-data-collection-service](https://github.com/HSE-COURSEWORK-2025/hse-coursework-backend-data-collection-service) | Сервис сбора и хранения данных с устройств |
| [hse-coursework-ratings-api](https://github.com/HSE-COURSEWORK-2025/hse-coursework-ratings-api) | Сервис рейтингов и отзывов пользователей |
| [hse-coursework-backend-fetch-google-api-data](https://github.com/HSE-COURSEWORK-2025/hse-coursework-backend-fetch-google-api-data) | Импорт данных из Google Fitness API |
| [hse-coursework-backend-ml-predictions](https://github.com/HSE-COURSEWORK-2025/hse-coursework-backend-ml-predictions) | ML-сервис для предсказаний рисков |
| [hse-coursework-backend-find-outliers](https://github.com/HSE-COURSEWORK-2025/hse-coursework-backend-find-outliers) | Сервис для поиска аномалий в данных |
| [hse-coursework-backend-prepare-data](https://github.com/HSE-COURSEWORK-2025/hse-coursework-backend-prepare-data) | Препроцессинг и подготовка данных |

### Фронтенд и мобильное приложение
| Репозиторий | Описание |
|-------------|----------|
| [hse-coursework-front](https://github.com/HSE-COURSEWORK-2025/hse-coursework-front) | Веб-интерфейс пользователя |
| [hse-coursework-android-app](https://github.com/HSE-COURSEWORK-2025/hse-coursework-android-app) | Мобильное приложение для Android |

### DAG-и и асинхронные задачи
| Репозиторий | Описание |
|-------------|----------|
| [hse-coursework-dags](https://github.com/HSE-COURSEWORK-2025/hse-coursework-dags) | DAGs для Apache Airflow, автоматизация ETL и ML пайплайнов |
| [hse-coursework-drammatiq-data-collector](https://github.com/HSE-COURSEWORK-2025/hse-coursework-drammatiq-data-collector) | Асинхронный сбор данных с помощью Dramatiq |

### Инфраструктурные сервисы
| Репозиторий | Описание |
|-------------|----------|
| [hse-coursework-airflow](https://github.com/HSE-COURSEWORK-2025/hse-coursework-airflow) | Деплой и конфигурация Apache Airflow |
| [hse-coursework-redis](https://github.com/HSE-COURSEWORK-2025/hse-coursework-redis) | Конфигурация и деплой Redis |
| [hse-coursework-kafka](https://github.com/HSE-COURSEWORK-2025/hse-coursework-kafka) | Деплой и настройка Apache Kafka |
| [hse-coursework-kubernetes-config](https://github.com/HSE-COURSEWORK-2025/hse-coursework-kubernetes-config) | Kubernetes-манифесты для развертывания сервисов |
| [hse-coursework-grafana](https://github.com/HSE-COURSEWORK-2025/hse-coursework-grafana) | Дашборды и мониторинг в Grafana |
| [network-stuff](https://github.com/HSE-COURSEWORK-2025/network-stuff) | Сетевые настройки |

### ML, данные и документация
| Репозиторий | Описание |
|-------------|----------|
| [hse-coursework-ml-models](https://github.com/HSE-COURSEWORK-2025/hse-coursework-ml-models) | ML-модели и эксперименты |
| [docs](https://github.com/HSE-COURSEWORK-2025/docs) | Документация и примеры отчетов |

## 📄 Пример PDF-отчета

Пример отчета, сгенерированного приложением:

[Пример отчета (PDF)](https://github.com/HSE-COURSEWORK-2025/docs/blob/main/report_example.pdf)

## ⚠️ Важная информация

**Данный проект является учебной работой. Автор не несёт ответственности за:**

1. Точность медицинских прогнозов и рекомендаций
2. Сохранность персональных данных пользователей
3. Стабильность работы системы в production-среде
4. Любые последствия использования данного ПО

**Использование системы осуществляется на свой страх и риск.** Данное программное обеспечение не является медицинским устройством и не может использоваться для диагностики или лечения заболеваний.

Все данные в системе являются тестовыми и не содержат реальной медицинской информации о пациентах.

## 📬 Контактная информация

По всем вопросам обращайтесь к автору проекта:
- **Telegram**: [@igmalysh](https://t.me/igmalysh)
- **Email**: [iimalysh@edu.hse.ru](mailto:iimalysh@edu.hse.ru)
