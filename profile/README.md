# HSE Coursework Health 🩺

![Kubernetes](http://img.shields.io/badge/kubernetes-%23326ce5.svg?style=flat&logo=kubernetes&logoColor=white)
![Python](http://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
![React](http://img.shields.io/badge/react-%2320232a.svg?style=flat&logo=react&logoColor=%2361DAFB)

Сервис для анализа данных с носимых датчиков для мониторинга здоровья. Платформа собирает, обрабатывает и визуализирует медицинские показатели, выявляет аномалии и прогнозирует риски для здоровья.

**Демо**: [http://hse-coursework-health.ru/](http://hse-coursework-health.ru/)
> Если сайт не открывается по доменному имени, напишите автору в Telegram: [@igmalysh](https://t.me/igmalysh)

## 🚀 Доступ к демо

### Для тестирования системы:
1. **Вы можете создать/войти в тестовый аккаунт на странице входа**
  - будут работать все функции кроме выгрузки из google fitness api, можно будет выгружать данные со смортфона

2. **Доступ через Google OAuth**:
   - Для входа через Google аккаунт необходимо связаться с автором проекта
   - Автор добавит ваш email в whitelist Google Cloud Console
   - Контакт для доступа: [Telegram](https://t.me/igmalysh)

3. **Демо-аккаунт**  
   — На странице входа просто нажмите кнопку **«Войти в демо-аккаунт»**.
   
## Основные компоненты системы

### Пользовательские интерфейсы
- **Веб-приложение**: [http://hse-coursework-health.ru/](http://hse-coursework-health.ru/)
- **Мобильное приложение**: Доступно для Android 

<p align="center">
  <img
    src="https://github.com/HSE-COURSEWORK-2025/.github/blob/main/image.png?raw=true"
    alt="Мобильное приложение"
    width="300"
  />
</p>

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

## ⚠️ Важная информация

**Данный проект является учебной работой. Автор не несёт ответственности за:**

1. Точность медицинских прогнозов и рекомендаций
2. Сохранность персональных данных пользователей
3. Стабильность работы системы в production-среде
4. Любые последствия использования данного ПО

**Использование системы осуществляется на свой страх и риск.** Данное программное обеспечение не является медицинским устройством и не может использоваться для диагностики или лечения заболеваний.

Все данные в системе являются тестовыми и не содержат реальной медицинской информации о пациентах.

## Контактная информация

По всем вопросам обращайтесь к автору проекта:
- **Telegram**: [@igmalysh](https://t.me/igmalysh)
- **Email**: [igmalysh@gmail.com](mailto:igmalysh@gmail.com)
