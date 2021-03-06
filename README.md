# instagram_followers_parser
Скрипт для парсинга подписчиков страницы в Instagram.

<b>ВНИМАНИЕ! Использование данного скрипта может привести к блокировке вашего аккаунта!</b>

# Инструкция
1) Открыть https://instagram.com в браузере на ПК (и войти в аккаунт).
2) Открыть профиль, с которого будут собираться данные подписчиков.
3) Открыть окно со списком подписчиков.
4) Нажать Ctrl+Shift+J (по умолчанию в Chrome), чтобы открылась вкладка "Console".
5) Копировать и вставить код "instagramFollowersParser.js" в консоль.
6) Нажать Enter.

После этого, должен начаться процесс сбора данных подписчиков.

# Отличия от <a href="https://github.com/leoneedpro/instagram-parser">этого скрипта</a>:
1) <b>Работает в версии Instagram от 12.07.2022.</b>
2) <b>При возникновении ошибки, выводит собранные данные подписчиков.</b>
3) <b>Удаляет элементы с подписчиками, данные которых уже получены - потребляется меньше оперативной памяти.</b>
4) Использует <a href="https://developer.mozilla.org/ru/docs/Web/API/MutationObserver">MutationObserver</a>, который позволяет прокручивать список сразу после его подгрузки.
5) Можно остановить и вывести собранные данные в любой момент, введя `onFinish()` в консоль.
6) Ошибки описываются более подробно.
7) Код легче читать - RegEx использован по минимуму, уменьшена громоздкость комментариев.
