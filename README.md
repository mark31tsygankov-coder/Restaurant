# OMNIRO VPN bot (улучшенная версия)

## Что нового
- **Mini App** — чёрно-белый дизайн, скруглённые кнопки, анимации, ripple-эффект
- Рабочие разделы: **Купить**, **Подарить**, **Мои подписки** (с ключом и копированием), **Поддержка**
- Получение ключа прямо в приложении
- API `/api/user` и `/api/order` с проверкой Telegram initData
- Бот отвечает быстрее (WAL SQLite, фоновый upsert, мгновенный answer callback)

## Render
1. Залей папку в GitHub (без .env).
2. New Web Service / Blueprint → `pip install -r requirements.txt`, start `python main.py`.
3. Env: BOT_TOKEN, ADMIN_IDS, ROLLYPAY_*, H1CLOUD_API_TOKEN, SUPPORT_USERNAME.
4. Disk mount `/data`, DB_PATH=/data/bot.db.
5. MINI_APP_URL = `https://ТВОЙ-СЕРВИС.onrender.com` (тот же домен).
6. После деплоя проверь /admin → Диагностика H1Cloud.

Бесплатный план Render засыпает — для нормальной скорости нужен Starter+.
