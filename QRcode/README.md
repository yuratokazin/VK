
# QR-код  

  

Для создания QR-кодов из URL в Debian/Linux удобнее всего использовать консольную утилиту [qrencode](https://www.google.com/search?q=qrencode&sca_esv=ad51375bc05ed99f&biw=1251&bih=591&sxsrf=ANbL-n4KM8s-ZnVYy8Bb0E2Bh33f996gbw%3A1773061165560&ei=LcSuaenIIan-wPAP4Zn1iQo&ved=2ahUKEwiJ2sXV8JKTAxX1HRAIHfmUHYcQgK4QegQIARAC&uact=5&oq=QR-коды+из+URL+дебиян&gs_lp=Egxnd3Mtd2l6LXNlcnAiIVFSLdC60L7QtNGLINC40LcgVVJMINC00LXQsdC40Y_QvTIIEAAYgAQYogQyCBAAGIAEGKIEMggQABiABBiiBDIIEAAYgAQYogQyCBAAGIAEGKIESJScAVC1PFiAiwFwBXgAkAEAmAG_AaABjwSqAQMwLjO4AQPIAQD4AQL4AQGYAgigAqIFwgILEAAYgAQYsAMYogSYAwDiAwUSATEgQIgGAZAGBJIHBTUuMi4xoAfID7IHBTAuMi4xuAfNBMIHBTItMS43yAdTgAgA&sclient=gws-wiz-serp&mstk=AUtExfBcyD5m_-lHEMvW8RsFpPIe7BVTEYK8EKaOKO4MiP5IZBDf13VuCVUd9pCG_98SVjkPt-lpjjow71xT-DWs-PCJEuVzFVQUC627MJXmKOH7kwT0qAtocTCj8HNk59ARokjF4uStHrQtXJHeF5_r7YRwsgaeHg5Iug43Btixxd0MC5uKmHvotbPdn8pQAWs9arKpUQdwJ9iZd6AD9CoZFnCeRAUiI0DZXDzK_UV5laJm_4oaw8AU8VeLF7hi8CfUBBK8RQB0pMsH3Rsx3M8AemfQ&csui=3). Она позволяет мгновенно превратить ссылку в код, отображаемый прямо в  терминале или сохраняемый в файл, обеспечивая быструю передачу данных на мобильные устройства. 

Основные способы использования qrencode

**Установка**:

```
sudo apt-get install qrencode
```

**Отображение QR-кода в терминале (ASCII-графика)**:

```
qrencode -t ASCII "https://debian.org"
```

*Для вывода в более читаемом формате (ANSI, если терминал поддерживает):*

```
qrencode -t ANSI256 "https://debian.org"
```

**Создание изображения (PNG)**:

```
qrencode -o vk.com_gitcube.png "https://vk.com/gitcube"
qrencode -o vkvideo.ru_gitcube.png "https://live.vkvideo.ru/gitcube"
qrencode -o vk.com_channel.png "https://vk.com/im/channels/-234893193"
qrencode -o vk.com_max.png "https://web.max.ru/-70603371353470"
```

Альтернативные инструменты 

**[QtQR](https://www.google.com/search?q=QtQR&sca_esv=ad51375bc05ed99f&biw=1251&bih=591&sxsrf=ANbL-n4KM8s-ZnVYy8Bb0E2Bh33f996gbw%3A1773061165560&ei=LcSuaenIIan-wPAP4Zn1iQo&ved=2ahUKEwiJ2sXV8JKTAxX1HRAIHfmUHYcQgK4QegQIBRAB&uact=5&oq=QR-коды+из+URL+дебиян&gs_lp=Egxnd3Mtd2l6LXNlcnAiIVFSLdC60L7QtNGLINC40LcgVVJMINC00LXQsdC40Y_QvTIIEAAYgAQYogQyCBAAGIAEGKIEMggQABiABBiiBDIIEAAYgAQYogQyCBAAGIAEGKIESJScAVC1PFiAiwFwBXgAkAEAmAG_AaABjwSqAQMwLjO4AQPIAQD4AQL4AQGYAgigAqIFwgILEAAYgAQYsAMYogSYAwDiAwUSATEgQIgGAZAGBJIHBTUuMi4xoAfID7IHBTAuMi4xuAfNBMIHBTItMS43yAdTgAgA&sclient=gws-wiz-serp&mstk=AUtExfBcyD5m_-lHEMvW8RsFpPIe7BVTEYK8EKaOKO4MiP5IZBDf13VuCVUd9pCG_98SVjkPt-lpjjow71xT-DWs-PCJEuVzFVQUC627MJXmKOH7kwT0qAtocTCj8HNk59ARokjF4uStHrQtXJHeF5_r7YRwsgaeHg5Iug43Btixxd0MC5uKmHvotbPdn8pQAWs9arKpUQdwJ9iZd6AD9CoZFnCeRAUiI0DZXDzK_UV5laJm_4oaw8AU8VeLF7hi8CfUBBK8RQB0pMsH3Rsx3M8AemfQ&csui=3)**: Графический интерфейс (GUI) для создания и декодирования QR-кодов.

```
sudo apt-get install qtqr
```

**[Zint](https://www.google.com/search?q=Zint&sca_esv=ad51375bc05ed99f&biw=1251&bih=591&sxsrf=ANbL-n4KM8s-ZnVYy8Bb0E2Bh33f996gbw%3A1773061165560&ei=LcSuaenIIan-wPAP4Zn1iQo&ved=2ahUKEwiJ2sXV8JKTAxX1HRAIHfmUHYcQgK4QegQIBRAF&uact=5&oq=QR-коды+из+URL+дебиян&gs_lp=Egxnd3Mtd2l6LXNlcnAiIVFSLdC60L7QtNGLINC40LcgVVJMINC00LXQsdC40Y_QvTIIEAAYgAQYogQyCBAAGIAEGKIEMggQABiABBiiBDIIEAAYgAQYogQyCBAAGIAEGKIESJScAVC1PFiAiwFwBXgAkAEAmAG_AaABjwSqAQMwLjO4AQPIAQD4AQL4AQGYAgigAqIFwgILEAAYgAQYsAMYogSYAwDiAwUSATEgQIgGAZAGBJIHBTUuMi4xoAfID7IHBTAuMi4xuAfNBMIHBTItMS43yAdTgAgA&sclient=gws-wiz-serp&mstk=AUtExfBcyD5m_-lHEMvW8RsFpPIe7BVTEYK8EKaOKO4MiP5IZBDf13VuCVUd9pCG_98SVjkPt-lpjjow71xT-DWs-PCJEuVzFVQUC627MJXmKOH7kwT0qAtocTCj8HNk59ARokjF4uStHrQtXJHeF5_r7YRwsgaeHg5Iug43Btixxd0MC5uKmHvotbPdn8pQAWs9arKpUQdwJ9iZd6AD9CoZFnCeRAUiI0DZXDzK_UV5laJm_4oaw8AU8VeLF7hi8CfUBBK8RQB0pMsH3Rsx3M8AemfQ&csui=3)**: Мощный генератор штрих-кодов, поддерживающий множество форматов.

**Онлайн-генераторы**: Можно использовать консольные утилиты типа `curl` с сервисами вроде `http://qrenco.de/`. 



Для чтения QR-кодов в Linux часто используют [zbar-tools](https://www.google.com/search?q=zbar-tools&sca_esv=ad51375bc05ed99f&biw=1251&bih=591&sxsrf=ANbL-n4KM8s-ZnVYy8Bb0E2Bh33f996gbw%3A1773061165560&ei=LcSuaenIIan-wPAP4Zn1iQo&ved=2ahUKEwiJ2sXV8JKTAxX1HRAIHfmUHYcQgK4QegQIBhAB&uact=5&oq=QR-коды+из+URL+дебиян&gs_lp=Egxnd3Mtd2l6LXNlcnAiIVFSLdC60L7QtNGLINC40LcgVVJMINC00LXQsdC40Y_QvTIIEAAYgAQYogQyCBAAGIAEGKIEMggQABiABBiiBDIIEAAYgAQYogQyCBAAGIAEGKIESJScAVC1PFiAiwFwBXgAkAEAmAG_AaABjwSqAQMwLjO4AQPIAQD4AQL4AQGYAgigAqIFwgILEAAYgAQYsAMYogSYAwDiAwUSATEgQIgGAZAGBJIHBTUuMi4xoAfID7IHBTAuMi4xuAfNBMIHBTItMS43yAdTgAgA&sclient=gws-wiz-serp&mstk=AUtExfBcyD5m_-lHEMvW8RsFpPIe7BVTEYK8EKaOKO4MiP5IZBDf13VuCVUd9pCG_98SVjkPt-lpjjow71xT-DWs-PCJEuVzFVQUC627MJXmKOH7kwT0qAtocTCj8HNk59ARokjF4uStHrQtXJHeF5_r7YRwsgaeHg5Iug43Btixxd0MC5uKmHvotbPdn8pQAWs9arKpUQdwJ9iZd6AD9CoZFnCeRAUiI0DZXDzK_UV5laJm_4oaw8AU8VeLF7hi8CfUBBK8RQB0pMsH3Rsx3M8AemfQ&csui=3). 

В Debian для работы с QR-кодами используются консольные утилиты [qrencode](https://www.google.com/search?q=qrencode&sca_esv=ad51375bc05ed99f&sxsrf=ANbL-n7r6M9UvUUwYqlZL8vh-l12-TQP9A%3A1773061128928&ei=CMSuaditOJerwPAP1aCbgQQ&biw=1251&bih=591&ved=2ahUKEwjcmdLH75KTAxVrExAIHbt0CEYQgK4QegQIARAC&uact=5&oq=QRcodeна+дебиян&gs_lp=Egxnd3Mtd2l6LXNlcnAiF1FSY29kZdC90LAg0LTQtdCx0LjRj9C9MgkQIRigARgKGCoyBxAhGKABGAoyBxAhGKABGApIl-EBUPONAViTwwFwAXgBkAEAmAHFAaABqgyqAQMwLjm4AQPIAQD4AQGYAgqgAvcNwgIKEAAYsAMY1gQYR8ICDRAAGIAEGLADGEMYigXCAgoQABiABBixAxgNwgIHEAAYgAQYDcICCBAAGAgYDRgewgIIEAAYgAQYogTCAgUQABjvBZgDAIgGAZAGCpIHBTEuNC41oAeiKrIHBTAuNC41uAfqDcIHBzItMy41LjLIB3WACAA&sclient=gws-wiz-serp&mstk=AUtExfDxH3PlvvakV6-tkKOspn0E7yXzRC_Ra_29m0k1yRVq7yRdAxR1LkGfctJAfY5UO3yuYJ3F4OT0AzfrpL6oNlRLt0nF6uJOh6l507fepewSinEC2aq72Tn01ZkFg6o1IXMONgRfBj4GFjGAg0l0A5TzKuYkHLdQ_2GoIkNHEFW3feTu5XzwlAgBcVKybSddv0rn3LtPnxwm4ybKOGeTgOyObZPK8Z4YncwvNtCZNw1aRbx-t30DbGkmHLPP6PCN7CUUc7A38zZYlThkTf1wW0ea&csui=3) (генерация) и [zbar-tools](https://www.google.com/search?q=zbar-tools&sca_esv=ad51375bc05ed99f&sxsrf=ANbL-n7r6M9UvUUwYqlZL8vh-l12-TQP9A%3A1773061128928&ei=CMSuaditOJerwPAP1aCbgQQ&biw=1251&bih=591&ved=2ahUKEwjcmdLH75KTAxVrExAIHbt0CEYQgK4QegQIARAD&uact=5&oq=QRcodeна+дебиян&gs_lp=Egxnd3Mtd2l6LXNlcnAiF1FSY29kZdC90LAg0LTQtdCx0LjRj9C9MgkQIRigARgKGCoyBxAhGKABGAoyBxAhGKABGApIl-EBUPONAViTwwFwAXgBkAEAmAHFAaABqgyqAQMwLjm4AQPIAQD4AQGYAgqgAvcNwgIKEAAYsAMY1gQYR8ICDRAAGIAEGLADGEMYigXCAgoQABiABBixAxgNwgIHEAAYgAQYDcICCBAAGAgYDRgewgIIEAAYgAQYogTCAgUQABjvBZgDAIgGAZAGCpIHBTEuNC41oAeiKrIHBTAuNC41uAfqDcIHBzItMy41LjLIB3WACAA&sclient=gws-wiz-serp&mstk=AUtExfDxH3PlvvakV6-tkKOspn0E7yXzRC_Ra_29m0k1yRVq7yRdAxR1LkGfctJAfY5UO3yuYJ3F4OT0AzfrpL6oNlRLt0nF6uJOh6l507fepewSinEC2aq72Tn01ZkFg6o1IXMONgRfBj4GFjGAg0l0A5TzKuYkHLdQ_2GoIkNHEFW3feTu5XzwlAgBcVKybSddv0rn3LtPnxwm4ybKOGeTgOyObZPK8Z4YncwvNtCZNw1aRbx-t30DbGkmHLPP6PCN7CUUc7A38zZYlThkTf1wW0ea&csui=3) (сканирование), а также графический интерфейс [qtqr](https://www.google.com/search?q=qtqr&sca_esv=ad51375bc05ed99f&sxsrf=ANbL-n7r6M9UvUUwYqlZL8vh-l12-TQP9A%3A1773061128928&ei=CMSuaditOJerwPAP1aCbgQQ&biw=1251&bih=591&ved=2ahUKEwjcmdLH75KTAxVrExAIHbt0CEYQgK4QegQIARAE&uact=5&oq=QRcodeна+дебиян&gs_lp=Egxnd3Mtd2l6LXNlcnAiF1FSY29kZdC90LAg0LTQtdCx0LjRj9C9MgkQIRigARgKGCoyBxAhGKABGAoyBxAhGKABGApIl-EBUPONAViTwwFwAXgBkAEAmAHFAaABqgyqAQMwLjm4AQPIAQD4AQGYAgqgAvcNwgIKEAAYsAMY1gQYR8ICDRAAGIAEGLADGEMYigXCAgoQABiABBixAxgNwgIHEAAYgAQYDcICCBAAGAgYDRgewgIIEAAYgAQYogTCAgUQABjvBZgDAIgGAZAGCpIHBTEuNC41oAeiKrIHBTAuNC41uAfqDcIHBzItMy41LjLIB3WACAA&sclient=gws-wiz-serp&mstk=AUtExfDxH3PlvvakV6-tkKOspn0E7yXzRC_Ra_29m0k1yRVq7yRdAxR1LkGfctJAfY5UO3yuYJ3F4OT0AzfrpL6oNlRLt0nF6uJOh6l507fepewSinEC2aq72Tn01ZkFg6o1IXMONgRfBj4GFjGAg0l0A5TzKuYkHLdQ_2GoIkNHEFW3feTu5XzwlAgBcVKybSddv0rn3LtPnxwm4ybKOGeTgOyObZPK8Z4YncwvNtCZNw1aRbx-t30DbGkmHLPP6PCN7CUUc7A38zZYlThkTf1wW0ea&csui=3). Установка выполняется командой `sudo apt install qrencode zbar-tools qtqr`. Основные инструменты позволяют создавать коды из текста/ссылок и декодировать изображения через веб-камеру. 

**Основные инструменты в Debian:**

- **Генерация (CLI):** `qrencode` — создает QR-коды из текста или URL и сохраняет их в PNG или EPS.
  - *Пример:* `qrencode -o test.png "Hello World"`
- **Сканирование/Чтение (CLI):** `zbar-tools` (команда `zbarimg` или `zbarcam`) — позволяет считывать коды с файлов изображений или через веб-камеру.
- **Графический интерфейс (GUI):** `qtqr` — удобная программа на базе Qt для создания и декодирования QR-кодов, включая настройку уровня коррекции ошибок.
- **Библиотеки:** `libqrencode-dev` — для разработчиков. 

**Установка:**

```
sudo apt update
sudo apt install qrencode zbar-tools qtqr
```
