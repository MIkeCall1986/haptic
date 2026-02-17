<!-- Header -->
<div align="center" style="margin-top: 120px">
  <a href="https://haptic.md/app">
    <img
      src="./.github/assets/icon.svg"
      alt="Haptic"
      height="100"
    />
  </a>

  <h3 align="center">Haptic
  </h3>
  <b>
    Open-Source markdown editor - your new home for notes
  </b>
</div>

<!-- TOC -->
<p align="center">
    <a href="https://haptic.md"><strong>Learn more »</strong></a>
    <br />
    <br />
    <a href="https://github.com/chroxify/haptic/tree/main#introduction">Introduction</a>
    ·
    <a href="https://github.com/chroxify/haptic/tree/main#tech-stack">Tech Stack</a>
    ·
    <a href="https://github.com/chroxify/haptic/tree/main#deploy-your-own">Deploy Your Own</a>
    ·
    <a href="https://github.com/chroxify/haptic/tree/main#roadmap">Roadmap</a>

  17.02.26
  Ось результати аналізу та стратегія трансформації для проекту **Haptic**, підготовлені у форматі для копіювання в Notion.

---

# 📑 Звіт AI-консультанта: Проект "Haptic"

**Haptic** — це сучасний open-source редактор для Markdown-нотаток, що фокусується на принципах **local-first** (локальне зберігання) та приватності користувача.

## 🧬 Частина 1: "ДНК" Проекту

Логіку коду проекту **Haptic** можна розбити на такі **атомарні функції**:

*   **Локальна персистентність (PGlite):** Використання вбудованої бази даних Postgres (PGlite) для збереження нотаток безпосередньо у браузері або додатку без необхідності зовнішнього сервера.
*   **Кросплатформна оболонка (Tauri):** Забезпечення роботи веб-технологій (Svelte) як нативного десктопного додатка за допомогою Rust.
*   **Markdown-процесинг (Svelte + TypeScript):** Функції парсингу, редагування та рендерингу тексту у форматі Markdown у реальному часі.
*   **Система розгортання та хостингу:** Підтримка швидкого деплою через Vercel та контейнеризацію Docker для веб-версії.
*   **Синхронізація та обмін (Roadmap):** Майбутні функції Haptic Sync та note sharing для передачі даних між пристроями.

### 💎 Головна технічна цінність
Головна цінність проекту полягає в архітектурі **"local-first & privacy-focused"**. На відміну від більшості редакторів, Haptic використовує **PGlite** — повноцінну SQL-базу даних, що працює локально. Це дозволяє користувачу мати повний суверенітет над своїми даними, забезпечуючи високу швидкість роботи та можливість складних вибірок без доступу до інтернету.

---

## 🚀 Частина 2: "Трансформація" (Інтеграція з Gemini LLM)

Інтеграція з **Gemini** (через інструменти **GitHub Models** або **GitHub Spark**) перетворює статичний блокнот на **активну базу знань**.

### Як зміниться функціонал?
1.  **Семантичний аналіз нотаток:** Gemini зможе аналізувати контекст ваших Markdown-файлів, автоматично створюючи зв'язки між схожими ідеями в різних документах.
2.  **Інтелектуальне резюмування:** Функція автоматичного створення стислого викладу (summary) для довгих записів одним натисканням.
3.  **AI-автодоповнення:** Написання коду або тексту безпосередньо в редакторі, спираючись на контекст усієї бази нотаток користувача.

### Сценарій сервісу "Smart Knowledge Base" (Haptic + Gemini + ID_{$})

Створення персоналізованого сервісу збору знань на вашому сайті.

**Алгоритм роботи:**
1.  **Збір (ID_{$}):** Ваш базовий Python-скрипт `ID_{$}` автоматично парсить цікаві статті або технічну документацію з мережі.
2.  **Обробка (Gemini):** Через **GitHub Models** дані передаються до Gemini. ШІ очищує текст від "сміття", форматує його в ідеальний Markdown та виділяє головні тези.
3.  **Збереження (Haptic):** Скрипт `ID_{$}` через API або локальний імпорт додає ці Markdown-файли до бази даних **Haptic** (PGlite).
4.  **Візуалізація:** Ви використовуєте **GitHub Spark** для швидкого деплою веб-інтерфейсу Haptic на вашому сайті, де користувач бачить уже структуровані, "розумні" нотатки.
5.  **Результат:** Ви отримуєте автономну систему, яка самостійно наповнюється знаннями, обробленими AI, але при цьому зберігає їх локально та приватно.

---

## 📋 План дій для Notion
| Крок | Дія | Результат |
| :--- | :--- | :--- |
| **1** | Розгортання через Docker: `docker pull chroxify/haptic-web` | Готове середовище для нотаток |
| **2** | Налаштування PGlite для локальної бази | Надійне зберігання без хмари |
| **3** | Підключення Gemini через **GitHub Models** | Додавання інтелектуальних функцій |
| **4** | Створення Python-містка (`ID_{$}`) | Автоматизація наповнення бази даних |

---

### 💡 Резюме

**Суть:** **Приватне локальне сховище Markdown-нотаток**.

**AI-Роль:** **Інтелектуальна обробка та структурування знань** (з використанням можливостей GitHub Spark та Models для розгортання ШІ-додатків).
    ·
    <a href="https://github.com/chroxify/haptic/tree/main#contributing">Contributing</a>
  </p>
</p>

<p>
    <a href="https://haptic.md/app">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="./.github/assets/haptic-dark.png">
        <source media="(prefers-color-scheme: light)" srcset="./.github/assets/haptic-light.png">
        <img alt="Haptic" src="./.github/assets/haptic-dark.png">
      </picture>
    </a>
</p>

## Introduction

Haptic is a new local-first & privacy-focused, open-source home for your markdown notes. It's minimal, lightweight, efficient and aims to have _all you need and nothing you don't_.

If you'd like to learn more about Haptic, why it's being built, what its goals are and how it differs from all the other markdown editors out there, you can read more about it [here](https://haptic.md/app).

## Tech Stack

- [Tauri](https://tauri.app/) – Desktop App
- [PGlite](https://pglite.dev/) – Local Database
- [Svelte](https://kit.svelte.dev/) – Framework
- [Tailwind](https://tailwindcss.com/) – CSS
- [Shadcn/ui](https://www.shadcn-svelte.com/) – Component Library
- [Vercel](https://vercel.com/) – Hosting

## Deploy Your Own

If you're interested in self-hosting your own web instance of Haptic, you can do so with these two options:

### Vercel

You can one-click deploy your own instance of Haptic on Vercel. Just click the button below and follow the instructions:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/chroxify/haptic&project-name=haptic-web&repository-name=haptic-web&root-directory=apps/web)

### Docker

1. Pull the image from the docker hub

```bash
docker pull chroxify/haptic-web:latest
```

2. Run the container

```bash
docker run -d -p 3000:80 chroxify/haptic-web:latest
```

3. Visit `http://localhost:3000` in your browser

## Roadmap

Haptic is currently still in active development. Here are some of the features planned for the future:

- [ ] Haptic Sync - Sync your notes across devices
- [ ] Note sharing - Share single notes or entire collections via link
- [ ] Mobile support for the web app - Currently dependent on PGlite support for mobile
- [ ] Native mobile apps for iOS & Android
- [ ] Windows & Linux support for the desktop app

and much much more, so stay tuned!

## Contributing

We would love to have your help in making haptic better!

Here's how you can contribute:

- [Report a bug](https://github.com/chroxify/haptic/issues/new?labels=bug) you found while using Haptic
- [Request a feature](https://github.com/chroxify/haptic/issues/new?labels=enhancement) that you think will be useful
- [Submit a pull request](https://github.com/chroxify/haptic/pulls) if you want to contribute with new features or bug fixes

## License

Haptic is licensed under the [GNU Affero General Public License Version 3 (AGPLv3)](https://github.com/chroxify/haptic/blob/main/LICENSE).

---
