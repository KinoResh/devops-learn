# Git команди

---

## git init
Створює новий репозиторій в поточній папці.
Створює приховану папку `.git` де Git зберігає всю історію.

**Використання:**
\```bash
git init
\```

**Коли використовувати:**
Тільки один раз на початку проекту.
Якщо клонуєш з GitHub — не потрібен.

---

## git config
Налаштування Git — імʼя, email, поведінка.

**Використання:**
\```bash
git config --global user.name "Твоє Імʼя"
git config --global user.email "email@gmail.com"
git config --global credential.helper store
git config --list
\```

**Рівні налаштувань:**
- `--global` — для всіх проектів
- `--local` — тільки для одного проекту
- `--system` — для всіх користувачів

**Пріоритет:** system < global < local

---

## git reset
Прибирає файли з індексу. Скасовує `git add`.

**Використання:**
\```bash
git reset notes.txt
git reset
\```

---

## .gitignore
Файл в якому пишеш що Git має ігнорувати.

**Як створити:**
\```bash
touch .gitignore
nano .gitignore
\```

**Що писати:**
\```
secrets.txt
*.log
node_modules/
\```

**Коли використовувати:**
- Паролі і токени
- Тимчасові файли
- Великі папки 
привіт
