# Установка и настройка Git

Git — это мощная система контроля версий, которая позволяет разработчикам эффективно работать с кодом. В этом разделе мы разберём, как установить и настроить Git на вашей системе.

---

## 📌 1. Установка Git

### 🔹 Windows

1. Перейдите на [официальный сайт Git](https://git-scm.com/downloads).
2. Скачайте установочный файл для Windows.
3. Запустите установщик и следуйте инструкциям (оставьте параметры по умолчанию).

После установки откройте **Командную строку (cmd)** или **Git Bash** и проверьте версию:

```bash
git --version
```

---

### 🔹 macOS

На macOS Git можно установить через **Homebrew**:

```bash
brew install git
```

Проверить установленную версию:

```bash
git --version
```

Если Homebrew не установлен, скачайте Git с [официального сайта](https://git-scm.com/downloads).

---

### 🔹 Linux (Ubuntu/Debian)

Выполните команду:

```bash
sudo apt update && sudo apt install git
```

Для Fedora и других дистрибутивов:

```bash
sudo dnf install git
```

После установки проверьте версию:

```bash
git --version
```

---

## 📌 2. Первоначальная настройка Git

Перед использованием Git настройте имя пользователя и email:

```bash
git config --global user.name "Ваше Имя"
git config --global user.email "your.email@example.com"
```

Эти данные будут отображаться в каждом коммите.

Чтобы проверить настройки:

```bash
git config --list
```

---

## 📌 3. Создание SSH-ключа (для работы с GitHub/GitLab)

Чтобы работать с удалёнными репозиториями по **SSH**, создайте ключ:

```bash
ssh-keygen -t rsa -b 4096 -C "your.email@example.com"
```

Ключ будет сохранён в `~/.ssh/id_rsa.pub`. Скопируйте его содержимое:

```bash
cat ~/.ssh/id_rsa.pub
```

Добавьте этот ключ в **настройки SSH-ключей на GitHub/GitLab**.

Проверка подключения:

```bash
ssh -T git@github.com
```

Если всё настроено верно, вы увидите сообщение:

```
Hi username! You've successfully authenticated, but GitHub does not provide shell access.
```

---

## 🚀 Готово!

Теперь ваш Git настроен, и вы можете клонировать репозитории, коммитить изменения и работать с ветками! 🎉

