# deepmint vpn — Telegram bot

Telegram-бот сервиса **deepmint vpn** ([@deepmintvpn_bot](https://t.me/deepmintvpn_bot)).

## Возможности

- Онбординг: подписка на канал [@deepmintvpn](https://t.me/deepmintvpn), принятие условий сервиса
- Главное меню: покупка подписки, открытие приложения (Telegram Mini App), баланс, реферальная программа, поддержка, документы
- Тарифы: Пробная 48 ч (0 ₽), 30/90/180/360 дней
- Реферальная система: 20% с оплат приглашённых

## Запуск

```bash
pip install -r requirements.txt
export DEEPMINT_BOT_TOKEN="токен от @BotFather"
python bot.py
```

Токен берётся из переменной окружения `DEEPMINT_BOT_TOKEN`, в коде не хранится.

## Структура

- `bot.py` — весь код бота (polling через Telegram Bot API, без сторонних библиотек-обёрток)
- `documents.json` — ссылки на документы (telegra.ph)
- `requirements.txt` — зависимости

Данные пользователей хранятся в `users.json` (исключён из репозитория).