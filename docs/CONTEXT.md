# FitFocus-policy — контекст

## Зачем
RuStore требует публичную ссылку на политику конфиденциальности. Плюс приложению нужен бесплатный хостинг для remote config без своего сервера. Оба файла живут здесь и раздаются через GitHub Pages.

## Состояние (на 17.10.2026)
- Два коммита от 13.09.2026: политика + remote config + index, затем ASO-тексты. С тех пор репозиторий **не обновлялся**.
- `privacy-policy.html` по содержанию совпадает с `FitFocus/docs/privacy-policy.html` (отличие только в переводах строк). В ней упомянуты Яндекс (РСЯ), AppMetrica, RuStore, уведомления; контакт — почта Павла.
- `remote-config.json` содержит только ручки рекламы и лимит пресетов: `interstitialMinIntervalMinutes` 8, `interstitialSkipFirstSessions` 3, `bannerEnabled` true, `interstitialAfterWorkout` true, `freeMaxPresets` 3.
- Ручки, добавленные в приложение позже, сюда **не добавлены** и берутся из вшитых значений: `reviewEnabled` (true), `reviewMinWorkouts` (3), `reviewIntervalDays` (30), `updatePromptEnabled` (true), `updateDeclineCooldownDays` (3). Чтобы управлять ими удалённо — дописать в JSON.
- `aso.md` устарел (название «FitFocus: таймер HIIT и Табата»); актуальная версия v2 — в `FitFocus/docs/aso.md`.

## Возможные задачи
- Синхронизировать `aso.md` с репозиторием приложения или удалить, чтобы не путать.
- Проверить, что политика упоминает всё, что есть в текущей версии: точные будильники (SCHEDULE_EXACT_ALARM / USE_EXACT_ALARM), RuStore Review/Update, изображения из галереи; бренд Postscript Apps.
- Дописать в `remote-config.json` ручки отзывов и обновлений.

## Похожее у других проектов
У «I love crosswords» есть свой аналогичный репозиторий `I-love-crosswords-policy` (политика + страницы-мостики для дуэлей и приглашений), локально его в `D:\git\RuStore` нет.
