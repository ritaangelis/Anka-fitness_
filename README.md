# M&M's Fitness — Telegram міні-додаток (прототип)

Один файл `index.html` — це весь застосунок (розклад, запис, правила, ціни, кабінет тренера-демо).
Дані поки умовні, бази й бота ще немає.

## Як запустити (по порядку)

### 1. GitHub
1. github.com → **New repository** → назва, наприклад `mm-fitness-app` → **Create**.
2. **Add file → Upload files** → перетягни `index.html`, `netlify.toml`, `.gitignore`, `README.md` → **Commit changes**.

### 2. Netlify (звідси береться посилання!)
1. app.netlify.com → **Add new site → Import an existing project → GitHub** → обери репозиторій.
2. Build command залиш порожнім, Publish directory — `.` → **Deploy**.
3. Отримаєш адресу виду `https://назва.netlify.app` — це і є посилання на застосунок.
   Після кожної правки в GitHub сайт оновлюється сам.

### 3. Бот у Telegram
1. У Telegram відкрий **@BotFather** → `/newbot` → ім'я бота → username (закінчується на `bot`).
2. BotFather дасть **токен**. Нікому його не показуй і **не клади в GitHub**.
3. `/mybots` → твій бот → **Bot Settings → Menu Button → Configure menu button** → встав адресу з Netlify.
4. Відкрий бота в Telegram, натисни кнопку меню — застосунок відкриється всередині Telegram.

### 4. Анна як головна
- Передати бота Анні: `/mybots` → бот → **Bot Settings → Transfer Ownership** (перевір цей пункт у меню).
- Анна має відкрити бота й натиснути **Start**, інакше бот не зможе їй писати.
- Її Telegram ID можна дізнатися через бота **@userinfobot**. За цим ID застосунок покаже їй кабінет тренера.

## Що буде далі
Сервер і база: справжні записи, повідомлення «Ви записані» клієнту й заявка Анні в Telegram, нагадування перед заняттям, адмінка (відмінити заняття, змінити ціни).
