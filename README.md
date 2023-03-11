[![Typing SVG](https://readme-typing-svg.herokuapp.com?color=%2336BCF7&lines=socket_udp+Найпростіший+веб-додаток )](https://git.io/typing-svg)

Веб-додаток з маршрутизацією для двох html сторінок: index.html та message.html

Також:

- Обробляє під час роботи програми статичні ресурси: style.css, logo.png;
- Організовує роботу з формою на сторінці message.html;
- У разі виникнення помилки 404 Not Found повертайте сторінку error.html

Програма працює на порту 3000.

Алгоритм роботи програми такий:

При вводі данних у форму, вони потрапляють у веб-додаток, який пересилає його далі на обробку за допомогою socket (протокол UDP).

Socket сервер переводить отриманий байт-рядок у словник і зберігає його в json файл data.json в папку storage.

Де ключ кожного повідомлення - це час отримання повідомлення. Тобто кожне нове повідомлення від веб-програми дописується до файлу storage/data.json з часом отримання.
