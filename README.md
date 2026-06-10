# Audioplayer (MVP)

## Описание

Приложение «Аудиоплеер»: frontend + backend API.

Функционал:

* Регистрация и авторизация пользователей
* Список треков
* Избранное
* Воспроизведение аудио
* Перемотка трека
* Поиск и сортировка
* Пагинация

## Демо

Frontend:
https://audioplayer-js.vercel.app

Backend API:
https://audioplayer-js.onrender.com
## Технологии

### Frontend

* TypeScript
* Vite
* Redom

### Backend

* Express
* JWT
* bcryptjs

### Deploy

* Vercel (Frontend)
* Render (Backend)

## Требования

* Node.js (LTS)
* npm

## Структура проекта

```text
audioplayer/      — фронтенд (Vite + TypeScript + Redom)
express-backend/  — backend (Express + JWT + bcrypt) и раздача mp3
```

## Запуск backend

```bash
cd express-backend
npm install
npm start
```

Сервер будет доступен по адресу:

```text
http://localhost:8000
```

## Запуск frontend

```bash
cd audioplayer
npm install
npm run dev
```

Приложение будет доступно по адресу:

```text
http://localhost:5173
```

## Переменные окружения

### Frontend (.env)

```env
VITE_API_URL=https://audioplayer-backend-26ar.onrender.com
```

### Backend (Render Environment Variables)

```env
BASE_URL=https://audioplayer-backend-26ar.onrender.com
```

## Использование

1. Зарегистрироваться
2. Авторизоваться
3. Перейти на страницу «Треки»
4. Воспроизводить композиции
5. Добавлять композиции в избранное

## Возможности

* Поиск по названию, альбому и артисту
* Сортировка по названию и альбому
* Добавление в избранное
* Плеер с перемоткой ±10 секунд
* Пагинация

## Примечание

Frontend размещён на Vercel, backend — на Render.

На бесплатном тарифе Render сервер может переходить в спящий режим. Первый запрос после периода бездействия может занимать до 30–60 секунд.
