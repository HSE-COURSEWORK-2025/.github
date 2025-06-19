# HSE Coursework Health 🩺

[![License](http://img.shields.io/badge/License-Apache_2.0-blue.svg)](http://opensource.org/licenses/Apache-2.0)
![Kubernetes](http://img.shields.io/badge/kubernetes-%23326ce5.svg?style=flat&logo=kubernetes&logoColor=white)
![Python](http://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
![React](http://img.shields.io/badge/react-%2320232a.svg?style=flat&logo=react&logoColor=%2361DAFB)

Сервис для анализа данных с носимых датчиков для мониторинга здоровья. Платформа собирает, обрабатывает и визуализирует медицинские показатели с возможностью выявления аномалий и прогнозирования рисков для здоровья.

**Демо**: [http://hse-coursework-health.ru/](http://hse-coursework-health.ru/)



## Основные компоненты системы

### Пользовательские интерфейсы
- **Веб-приложение**: [http://hse-coursework-health.ru/](http://hse-coursework-health.ru/)
- **Мобильное приложение**: Доступно для Android 

![img](https://github.com/HSE-COURSEWORK-2025/.github/blob/main/image.png?raw=true)

### API сервисы
| Сервис | URL | Документация |
|--------|-----|--------------|
| Auth API | http://hse-coursework-health.ru/auth-api | [Swagger](http://hse-coursework-health.ru/auth-api/docs) |
| Data Collection API | http://hse-coursework-health.ru/data-collection-api | [Swagger](http://hse-coursework-health.ru/data-collection-api/docs) |
| Results Provider API | http://hse-coursework-health.ru/results-provider | [Swagger](http://hse-coursework-health.ru/results-provider/docs) |
| Notifications API | http://hse-coursework-health.ru/notifications-api | [Swagger](http://hse-coursework-health.ru/notifications-api/docs) |
| Ratings API | http://hse-coursework-health.ru/ratings-api | [Swagger](http://hse-coursework-health.ru/ratings-api/docs) |

### Инструменты администрирования
| Инструмент | URL | Доступ |
|------------|-----|--------|
| Apache Airflow | http://hse-coursework-health.ru/airflow | `admin:admin` |
| Kafka UI | http://hse-coursework-health.ru/kafka-ui | Публичный |
| Grafana | http://hse-coursework-health.ru/grafana | `admin:admin` |

## Технологический стек

- **Бекенд**: Python 3.10, FastAPI
- **Фронтенд**: React, TypeScript, Recharts
- **Мобильное приложение**: Kotlin, Android SDK
- **Базы данных**: PostgreSQL, Redis
- **Очереди**: Apache Kafka
- **Оркестрация**: Kubernetes, Docker
- **ML**: Scikit-learn, Pandas, NumPy
- **Мониторинг**: Grafana, Prometheus
