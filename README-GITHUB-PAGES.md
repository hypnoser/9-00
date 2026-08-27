# Запуск сайту на GitHub Pages

Цей архів уже підготовлений як статичний сайт. Сервер, база даних і встановлення програм не потрібні.

## Поточне розміщення

Сайт розміщено в репозиторії `hypnoser/9-00` і він доступний за адресою:

https://hypnoser.github.io/9-00/

## Покроково

1. Увійдіть у GitHub і відкрийте репозиторій `hypnoser/9-00`.
2. Повністю розпакуйте ZIP-архів сайту.
3. На сторінці репозиторію натисніть **Add file → Upload files**.
4. Завантажте весь вміст розпакованої папки із заміною попередніх файлів. `index.html` має бути в корені репозиторію.
5. Натисніть **Commit changes**.
6. Якщо Pages ще не налаштовано, відкрийте **Settings → Pages**.
7. У **Build and deployment** оберіть **Deploy from a branch**, гілку `main`, папку `/(root)` і натисніть **Save**.
8. Дочекайтеся публікації та відкрийте `https://hypnoser.github.io/9-00/`.
9. Перевірте повний режим за адресою `https://hypnoser.github.io/9-00/?test=1`.

Офіційна документація:
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Коли буде власний домен

1. Відкрийте **Settings → Pages → Custom domain**.
2. Введіть придбаний домен і збережіть.
3. У кабінеті реєстратора домену додайте DNS-записи за актуальною інструкцією GitHub.
4. Після перевірки DNS увімкніть **Enforce HTTPS**.
5. Замініть тимчасову адресу в `index.html`, `pro-khvylynu-movchannia.html`, `robots.txt`, `sitemap.xml`, `llms.txt` і `llms-full.txt` на власний домен.

Офіційна документація:
https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

## Важливо про robots.txt у проєктному репозиторії

Файл доступний за адресою `https://hypnoser.github.io/9-00/robots.txt`, але стандарт robots.txt передбачає файл у корені домену: `https://hypnoser.github.io/robots.txt`. Щоб правила для AI-ботів діяли на рівні всього домену, додайте такий самий файл до репозиторію користувацького сайту `hypnoser.github.io`. `sitemap.xml` у цьому пакеті вже містить правильні адреси сторінок `/9-00/`.

## Звук на телевізорі або інформаційній панелі

Браузер може заблокувати звук до першої взаємодії користувача. Перед постійним показом:

1. Відкрийте `?test=1`.
2. Натисніть червоний індикатор тестового режиму.
3. Переконайтеся, що метроном чути.
4. Для керованих пристроїв попросіть IT-адміністратора додати домен до корпоративного списку дозволеного автоматичного відтворення звуку.

## Індексація

Можна під’єднати Google Search Console, Bing Webmaster Tools і аналітику та подати `https://hypnoser.github.io/9-00/sitemap.xml` на індексацію.
