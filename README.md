# RobloxCheatBot

Telegram бот для раздачи файлов (Solara, Xeno) из канала.

## Запуск на VPS

```bash
apt update && apt install python3 python3-pip screen -y
pip3 install -r requirements.txt

# С Proxy (если нужен)
export BOT_PROXY="socks5h://user:pass@ip:port"

screen -dmS cheatbot python3 bot.py
```

## Запуск на Render.com

1. Создай Web Service
2. Start Command: `python bot.py`
3. Build Command: `pip install -r requirements.txt`
4. Добавь переменные окружения (опционально)

## Переменные окружения

- `BOT_TOKEN` — токен бота (по умолчанию встроен)
- `ADMIN_ID` — ID админа
- `BOT_PROXY` — прокси (socks5h://...)
- `CHANNEL_ID` — ID канала с файлами
