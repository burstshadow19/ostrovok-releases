# Островок - политика конфиденциальности

Действует с 28 ноября 2026 г. (версия 4.90 и новее). Приложение: Островок (`com.paperisland.app`).
Связь с разработчиком: burstshadow19@gmail.com.

## Коротко
Уведомления, экран и все, что Островок видит ради капсулы, обрабатываются только на телефоне и никуда не уходят. Рекламы и аналитики нет. Разработчику уходят только отчеты о сбоях (автоматически, можно выключить) и отчет диагностики, если пользователь сам нажмет «Отправить разработчику». В них нет текстов уведомлений, имен, номеров и аккаунтов.

## Что Островок видит и зачем
- Уведомления (доступ к уведомлениям, включает пользователь в настройках Android): заголовок и текст уведомлений, название приложения, сведения о звонке, трек и обложка из плеера. Нужны, чтобы показать в капсуле музыку, звонок, сообщение, таймер или поездку. Не сохраняются и не передаются.
- Спецвозможности (AccessibilityService, включает пользователь в настройках Android): только то, какие окна сейчас на экране и какое приложение открыто. Нужны, чтобы рисовать капсулу поверх строки состояния, прятать ее при открытой шторке и видео на весь экран, не повторять музыку или звонок, когда они и так открыты, и открывать шторку свайпом. Текст на экране и в приложениях Островок не читает и ничего не нажимает за пользователя.
- Календарь (только если пользователь разрешит): название и время ближайшей встречи, чтобы напомнить о ней за 15 минут.
- Bluetooth (только если пользователь разрешит): уровень заряда подключенных наушников.
- Звонки (только если пользователь разрешит): ответить на звонок или сбросить его по нажатию в капсуле, когда Android скрыл кнопки звонилки.
- Состояние сети и батареи: значки связи, заряд и мощность зарядки в капсуле.

## Что хранится
На телефоне: настройки приложения, список приложений, из которых приходили уведомления и музыка (их имена пакетов, для фильтров в настройках), и короткий служебный журнал событий без текста уведомлений. Все это удаляется вместе с приложением или при очистке его данных.

## Что уходит разработчику
- Отчет о сбое - автоматически, если приложение упало или зависло: модель и производитель телефона, версия Android, версия Островка, место сбоя в коде, служебный журнал перед сбоем и случайный идентификатор установки (не связан с аккаунтом или номером телефона). Выключается переключателем «Сообщать о сбоях» в разделе Помощь.
- Отчет диагностики - только когда пользователь сам нажмет «Отправить разработчику» в разделе Помощь: то же, плюс размеры экрана и выреза камеры, состояние островка, служебный журнал (какое приложение прислало уведомление или играет музыку - имя пакета, и что сделал островок) и комментарий, если пользователь его напишет.
В отчетах нет текстов и заголовков уведомлений, имен, номеров телефонов, содержимого экрана, местоположения и аккаунтов.

Отчеты хранятся в Google Firebase (Crashlytics и Cloud Firestore, Google LLC) и используются только для поиска и исправления ошибок. Передача шифруется (HTTPS). Отчеты хранятся до 90 дней, затем удаляются. Удалить отчеты раньше можно, написав на почту разработчика.

## Передача третьим лицам
Нет. Данные не продаются и не передаются третьим лицам, кроме Google как поставщика хранения (Firebase).

## Дети
Приложение не предназначено для детей и не собирает данных о них.

## Изменения
Если политика изменится, новая версия появится по этой же ссылке с новой датой.

---

# Ostrovok - Privacy Policy

Effective November 28, 2026 (version 4.90 and later). App: Ostrovok / Островок (`com.paperisland.app`).
Contact: burstshadow19@gmail.com.

## In short
Notifications, the screen and everything else Ostrovok sees to show the capsule are processed on the device only and never leave it. There are no ads and no analytics. The developer receives only crash reports (automatic, can be turned off) and a diagnostic report when the user taps "Send to developer". They contain no notification text, names, phone numbers or accounts.

## What the app sees and why
- Notifications (notification access, enabled by the user in Android settings): notification title and text, app name, call details, the current track and its cover. Used only to show music, calls, messages, timers or rides in the capsule. Not stored or shared.
- Accessibility (AccessibilityService, enabled by the user in Android settings): only which windows are on screen and which app is in front. Used to draw the capsule above the status bar, hide it while the notification shade or full-screen video is open, avoid repeating music or a call when that app is already open, and open the shade on a swipe. The app does not read on-screen text and does not perform actions on the user's behalf.
- Calendar (only if the user allows it): title and time of the next meeting, for a reminder 15 minutes before.
- Bluetooth (only if the user allows it): battery level of connected headphones.
- Phone calls (only if the user allows it): answer or end a call when the user taps the capsule and Android has hidden the dialer's own buttons.
- Network and battery state: connection icons, battery level and charging power in the capsule.

## What is stored
On the device: the app's settings, the list of apps that posted notifications or played music (their package names, for the filters in settings), and a short diagnostic event log without notification text. All of it is deleted when the app is uninstalled or its data is cleared.

## What is sent to the developer
- Crash report - automatically when the app crashes or freezes: phone make and model, Android version, app version, where in the code it failed, the diagnostic log before the crash and a random installation ID (not linked to any account or phone number). Can be turned off with the "Сообщать о сбоях" (report crashes) switch in Help.
- Diagnostic report - only when the user taps "Отправить разработчику" (send to developer) in Help: the same, plus the screen and camera cutout sizes, the island's state, the diagnostic log (which app posted a notification or plays music - its package name - and what the island did) and the user's comment, if any.
Reports contain no notification text or titles, names, phone numbers, screen content, location or accounts.

Reports are stored in Google Firebase (Crashlytics and Cloud Firestore, Google LLC) and used only to find and fix bugs. They are sent encrypted (HTTPS), kept for up to 90 days and then deleted. To have them deleted sooner, email the developer.

## Sharing with third parties
None. Data is not sold or shared with third parties, except Google as the storage provider (Firebase).

## Children
The app is not directed at children and collects no data about them.

## Changes
If this policy changes, the new version will be published at the same address with a new date.
