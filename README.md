# АвтоТерра — legal website

Публичный статический сайт для мобильного приложения **«АвтоТерра»**.

## Страницы

- `index.html` — главная страница правовой информации.
- `privacy.html` — политика конфиденциальности для Google Play.
- `delete-account.html` — внешний ресурс для запроса удаления аккаунта.
- `styles.css` — адаптивные стили без внешних трекеров и библиотек.

## Публикация через GitHub Pages

1. Откройте репозиторий на GitHub.
2. Перейдите в **Settings → Pages**.
3. В разделе **Build and deployment** выберите **Deploy from a branch**.
4. Branch: **main**.
5. Folder: **/ (root)**.
6. Нажмите **Save**.

После публикации ожидаемые URL:

- Сайт: https://ibrodevs.github.io/avtoterra-web/
- Политика: https://ibrodevs.github.io/avtoterra-web/privacy.html
- Удаление аккаунта: https://ibrodevs.github.io/avtoterra-web/delete-account.html

В Google Play Console для поля **«Политика конфиденциальности»** используйте прямой URL `privacy.html`.

Для раздела **Data safety → Account deletion** используйте прямой URL `delete-account.html`.

## Важно

Текст политики синхронизирован с правовыми документами мобильного приложения в ветке `adilhan_new` на редакцию от 15 сентября 2026 г. При изменении состава собираемых данных, сторонних сервисов, способов оплаты, push-уведомлений или сроков хранения необходимо одновременно обновлять политику в приложении, на этом сайте и декларацию Data safety в Google Play.
