# Используем официальный образ Node.js
FROM node:14

# Устанавливаем рабочую директорию
WORKDIR /app

# Копируем package.json и package-lock.json для установки зависимостей
COPY package*.json ./

# Устанавливаем зависимости
RUN npm install

# Копируем остальные файлы приложения
COPY . .

# Указываем порт, который будет использоваться приложением
EXPOSE 3000
EXPOSE 8000

# Команда для запуска приложения
CMD ["node", "index.js"]
