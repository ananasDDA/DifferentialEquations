# Дифференциальные уравнения
Cайт посвященный курсу дифференциальных уравнений. Сайт создан с использованием MkDocs Material и размещен на GitHub Pages.

🌐 [Перейти на сайт](https://ananasdda.github.io/DifferentialEquations/)

## 🚀 Возможности

- 📚 Подробные конспекты лекций

- ✍️ Интерактивные примеры и графики

- 🔬 Поддержка сложных математических формул (LaTeX)

- 🌙 Темная и светлая темы

- 📱 Адаптивный дизайн

- 🔍 Встроенный поиск

- 📝 Интеграция с Google Drive для доступа к лекционным материалам


## 📋 Структура сайта


## 🛠 Технологии

- MkDocs Material

- Python

- JavaScript (MathJax, GeoGebra)

- GitHub Actions для автоматического деплоя

- Google Drive API для хранения документов


## 💻 Локальный запуск


1. Клонируйте репозиторий:

```bash
git clone https://github.com/yourusername/repo-name.git
```

2. Установите зависимости:
```bash
pip install -r requirements.txt
```

3. Запустите локальный сервер:
```bash
mkdocs serve
```

4. Откройте http://localhost:8000 в браузере


## 🔄 Обновление контента

1. Добавьте или измените файлы в директории `docs/`

2. Закоммитьте изменения:
```bash
git add .
git commit -m "Обновление контента"
git push origin main
```

3. GitHub Actions автоматически обновит сайт

## 📝 Как внести вклад

1. Создайте форк репозитория

2. Создайте ветку для ваших изменений

## 🚀 Деплой

GitHub Actions автоматически разворачивает сайт при пуше в ветку main. Рабочий процесс настроен следующим образом:

```yaml
name: Deploy MkDocs
on:
  push:
    branches:
      - main
permissions:
  contents: write
jobs:
  deploy:
    runs-on: ubuntu-22.04
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-python@v4
        with:
          python-version: '3.x'
      - run: pip install mkdocs-material
      - run: pip install pillow cairosvg
      - name: Deploy
        run: mkdocs gh-deploy --force
```

Для ручного деплоя выполните:

```bash
mkdocs gh-deploy
```

## 📋 Требования

- Python 3.x
- pip
- git

## 📦 Зависимости

Создайте файл requirements.txt со следующим содержимым:

```text
mkdocs-material
pillow
cairosvg
mkdocs-glightbox
```

## 📞 Контакты

[Telegram](https://t.me/ananasDDA)
