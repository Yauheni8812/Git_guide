# Git Status

Команда `git status` используется для проверки состояния рабочего каталога и индекса. Она показывает, какие файлы изменены, добавлены в индекс или не отслеживаются.

---

## 📌 Синтаксис  

```bash
git status
```

Эта команда не вносит изменений в файлы, а только **отображает текущий статус репозитория**.

---

## 🔹 Примеры использования  

### 1️⃣ Проверка статуса репозитория  

Выполните команду:

```bash
git status
```

Пример вывода:

```bash
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  modified:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
  new-file.txt
```

---

### 2️⃣ Опции команды `git status`  

- **Отображение краткого статуса:**  
  ```bash
  git status -s
  ```

  Вывод в кратком формате:

  ```bash
  M  index.html
  ?? new-file.txt
  ```

  - `M` — изменённый файл (modified)
  - `??` — неотслеживаемый файл (untracked)

---

## 🚀 Полезные советы  

- **Перед коммитом всегда проверяйте статус репозитория:**  
  ```bash
  git status
  ```

- **Чтобы отслеживать новые файлы, добавьте их в индекс:**  
  ```bash
  git add <файл>
  ```

- **Если нужно быстро проверить изменения, можно использовать `git diff`:**  
  ```bash
  git diff
  ```

---

Теперь вы знаете, как использовать `git status` для проверки состояния репозитория! 🚀
