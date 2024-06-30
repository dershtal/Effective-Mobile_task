# Используем базовый образ с Python
FROM python:3.10

# Устанавливаем рабочую директорию
WORKDIR /app

# Копируем файл requirements.txt в рабочую директорию
COPY requirements.txt .

# Устанавливаем зависимости
RUN pip install --no-cache-dir -r requirements.txt

# Копируем все файлы вашего приложения в рабочую директорию
COPY . .

# Указываем команду для запуска вашего приложения
CMD ["python", "app.py"]
