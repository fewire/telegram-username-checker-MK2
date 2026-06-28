# Telegram Username Checker MK2

**MK2** — find available Telegram usernames using an English dictionary or random strings.

A Jupyter notebook that generates username candidates, checks availability via the Telegram API ([Telethon](https://github.com/LonamiWebs/Telethon)), and saves free usernames to a file. Designed for **Google Colab**, works in any Jupyter environment with network access.

> Unofficial tool. Not affiliated with Telegram. Use at your own risk.

---

## Features

- **Dictionary mode** — pick random English words (`@apple`, `@dragon`)
- **Random mode** — random character strings (`@xK9mP`)
- Saves results to `Input.txt` and `Available.txt`
- Skips already checked words (`checked_words.txt`)
- Session persistence (`telegram.session`)

---

## Quick Start

1. Open `username_checker.ipynb` in [Google Colab](https://colab.research.google.com)
2. Fill in the **Config** cell:
   - `API_ID` and `API_HASH` from [my.telegram.org](https://my.telegram.org)
   - `PHONE` and `PASSWORD_2FA`
3. Run **Config**, then **Run**
4. Enter the Telegram login code on first run

---

## Config

| Setting | Description |
|---|---|
| `GENERATION_MODE` | `"dictionary"` or `"random"` |
| `WORDS_PER_RUN_MIN/MAX` | How many words to check per run (dictionary mode) |
| `SKIP_ALREADY_CHECKED` | Skip words already in `checked_words.txt` |
| `APPEND_AVAILABLE` | `False` = overwrite `Available.txt`; `True` = append |

---

## Files

| File | Description |
|---|---|
| `username_checker.ipynb` | Main notebook |
| `words_alpha.txt` | English wordlist (~370k words) |
| `Input.txt` | Generated usernames (gitignored) |
| `Available.txt` | Available usernames (gitignored) |
| `checked_words.txt` | Already checked words (gitignored) |
| `telegram.session` | Auth session (gitignored) |

---

## Disclaimer

**Unofficial tool. Use at your own risk.**

- Not affiliated with Telegram
- Mass username checking may violate Telegram's Terms of Service
- You may get rate-limited (FloodWait) or face account restrictions
- The author is not responsible for any consequences of using this script

You are solely responsible for how you use this tool.

---

# Проверка ников Telegram MK2

**MK2** — поиск свободных ников в Telegram через английский словарь или случайные строки.

Jupyter-ноутбук: генерирует варианты ников, проверяет доступность через Telegram API ([Telethon](https://github.com/LonamiWebs/Telethon)) и сохраняет свободные в файл. Рассчитан на **Google Colab**, работает в любом Jupyter с доступом в сеть.

> Неофициальный инструмент. Не связан с Telegram. Используйте на свой страх и риск.

---

## Возможности

- **Режим словаря** — случайные английские слова (`@apple`, `@dragon`)
- **Режим рандома** — случайные символы (`@xK9mP`)
- Сохранение в `Input.txt` и `Available.txt`
- Пропуск уже проверенных слов (`checked_words.txt`)
- Сохранение сессии (`telegram.session`)

---

## Быстрый старт

1. Откройте `username_checker.ipynb` в [Google Colab](https://colab.research.google.com)
2. Заполните ячейку **Config**:
   - `API_ID` и `API_HASH` с [my.telegram.org](https://my.telegram.org)
   - `PHONE` и `PASSWORD_2FA`
3. Запустите **Config**, затем **Run**
4. При первом входе введите код из Telegram

---

## Конфиг

| Параметр | Описание |
|---|---|
| `GENERATION_MODE` | `"dictionary"` или `"random"` |
| `WORDS_PER_RUN_MIN/MAX` | Сколько слов проверять за запуск |
| `SKIP_ALREADY_CHECKED` | Пропускать слова из `checked_words.txt` |
| `APPEND_AVAILABLE` | `False` = перезаписать `Available.txt`; `True` = дописать |

---

## Отказ от ответственности

**Неофициальный инструмент. Используйте на свой страх и риск.**

- Не связан с Telegram
- Массовая проверка ников может нарушать правила Telegram
- Возможны ограничения (FloodWait) или проблемы с аккаунтом
- Автор не несёт ответственности за последствия использования

Вы сами отвечаете за то, как используете этот скрипт.
