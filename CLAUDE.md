# FitFocus-policy — инструкции для Claude

Статический сайт на GitHub Pages для приложения **FitFocus** (основной код — `D:\git\RuStore\FitFocus`). Репозиторий: `p1r4te/FitFocus-policy`.
Подробности — [docs/CONTEXT.md](docs/CONTEXT.md).

## Что здесь
- `privacy-policy.html` — политика конфиденциальности (ссылка указана в карточке RuStore). Исходник-близнец лежит в `FitFocus/docs/privacy-policy.html`.
- `remote-config.json` — remote config приложения; его URL прописан как `REMOTE_CONFIG_URL` в `keys.properties` приложения. **Меняя этот файл, меняешь поведение у всех пользователей сразу** (частота рекламы, лимиты бесплатной версии).
- `index.html` — простая страница со ссылками.
- `aso.md` — старая копия ASO-текстов (актуальная — `FitFocus/docs/aso.md`).

## Правила
- `remote-config.json` должен оставаться валидным JSON; неизвестные ключи приложение игнорирует, отсутствующие берёт из вшитых Defaults (`RemoteConfigValues.kt`). Перед изменением — сверить имена ключей с кодом и предупредить Павла о последствиях.
- Политику держать синхронной с `FitFocus/docs/privacy-policy.html` и с реальным набором SDK/разрешений приложения.
- Не публиковать сюда секреты: файл публичный.
- Всё на русском, коммиты — «Что сделано».
