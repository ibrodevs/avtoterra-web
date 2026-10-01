# АвтоТерра — legal website

Публичный статический сайт для мобильного приложения **«АвтоТерра»**, подготовленный для деплоя на Vercel.

## Страницы

- `/` — главная страница правовой информации.
- `/privacy` — политика конфиденциальности для Google Play.
- `/delete-account` — внешний ресурс для запроса удаления аккаунта.

Исходные файлы `privacy.html` и `delete-account.html` автоматически доступны по чистым URL благодаря `cleanUrls` в `vercel.json`.

## Деплой на Vercel

1. Откройте Vercel Dashboard.
2. Нажмите **Add New → Project**.
3. Импортируйте GitHub-репозиторий **ibrodevs/avtoterra-web**.
4. В настройках проекта:
   - **Framework Preset:** Other;
   - **Root Directory:** `./`;
   - **Build Command:** оставить пустым;
   - **Output Directory:** оставить пустым;
   - **Install Command:** оставить пустым.
5. Нажмите **Deploy**.

Сайт полностью статический, поэтому Node.js, npm и переменные окружения не нужны.

## После первого деплоя

Vercel выдаст production URL. Используйте:

- `https://<ваш-домен>/privacy` — в Google Play Console → **Политика конфиденциальности**;
- `https://<ваш-домен>/delete-account` — для раздела удаления аккаунта/Data safety.

Если вы подключите собственный домен, используйте именно его постоянные production URL.

## Vercel configuration

`vercel.json` включает:

- clean URLs без `.html`;
- единый формат URL без завершающего слэша;
- дополнительные совместимые URL `/privacy-policy` и `/account-deletion`;
- security headers: CSP, X-Content-Type-Options, X-Frame-Options, Referrer-Policy и Permissions-Policy.

## SEO

`robots.txt` разрешает индексацию. После выбора постоянного production-домена можно добавить `sitemap.xml` и canonical URL с этим доменом. Не следует хранить sitemap с временным или неверным доменом.

## Важно

Текст политики синхронизирован с правовыми документами мобильного приложения в ветке `adilhan_new` на редакцию от 15 сентября 2026 г. При изменении состава собираемых данных, сторонних сервисов, способов оплаты, push-уведомлений или сроков хранения необходимо одновременно обновлять политику в приложении, на этом сайте и декларацию Data safety в Google Play.
