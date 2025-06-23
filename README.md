# Auth Service

Spring Boot микросервис авторизации, упакованный в Docker-контейнер.

## 🚀 Быстрый старт

### 1. Сборка JAR

Выполните команду в терминале из корня проекта:

```bash
./gradlew clean build
Если получите ошибку Permission denied, дайте права:

bash
Копировать
Редактировать
chmod +x ./gradlew
После сборки JAR-файл будет находиться по пути:

bash
Копировать
Редактировать
target/auth-service-0.0.1-SNAPSHOT.jar
2. Сборка Docker-образа
Убедитесь, что в корне проекта находится файл Dockerfile. Выполните:

bash
Копировать
Редактировать
docker build -t auth-service .
3. Запуск контейнера
bash
Копировать
Редактировать
docker run -p 8080:8080 auth-service
Теперь приложение будет доступно по адресу:

arduino
Копировать
Редактировать
http://localhost:8080
4. Использование Docker Compose (опционально)
Создайте docker-compose.yml:

yaml
Копировать
Редактировать
version: '3'
services:
  auth-service:
    build: ./
    ports:
      - "8080:8080"
Запуск:

bash
Копировать
Редактировать
docker compose up --build -d
📂 Структура проекта
Dockerfile — инструкция сборки образа

docker-compose.yml — опциональный запуск через Compose

target/ — папка со скомпилированным .jar-файлом

🔧 Требования
Java 17+

Gradle

Docker

🧑‍💻 Автор
art4000xxx

yaml
Копировать
Редактировать
