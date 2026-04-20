Theatre Padida App

Файлы:
- index.html — основное приложение
- manifest.json — установка как приложение
- sw.js — офлайн кэш
- apps-script.gs — backend для Google Apps Script
- icon-192.png, icon-512.png — иконки приложения

Как подключить Google Sheets, бэкап и Telegram:
1. Откройте apps-script.gs
2. Вставьте Spreadsheet ID, Telegram Bot Token и Chat ID
3. Разверните Apps Script как Web App
4. Скопируйте URL веб-приложения
5. В приложении нажмите Интеграции и вставьте этот URL

Как это работает:
- приложение сохраняет заявки локально
- каждое изменение ставится в очередь
- при наличии интернета очередь отправляется в Apps Script
- Apps Script обновляет лист Bookings
- Apps Script пишет журнал в Audit
- Apps Script сохраняет JSON-снимок в Backup
- Apps Script отправляет уведомление в Telegram
