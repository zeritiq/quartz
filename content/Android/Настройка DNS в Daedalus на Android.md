---
tags:
  - inbox
  - android/networks
sr-due: 2025-04-30
sr-interval: 192
sr-ease: 290
created: 2024-08-26T19:07:16+03:00
modified: 2024-10-20T11:37:47+03:00
publish: true
---
### Установка

Скачиваем с [[F-droid]] Daedalus:

[Daedalus | F-Droid - Free and Open Source Android App Repository](https://f-droid.org/packages/org.itxtech.daedalus/)

### Настраиваем домены через правила hosts

>*По большей части это имеет смысл только в сопоставления ip адресов в рамках локальной сети.*

>*Вряд ли это потребуется для удаленного сервера с белым ip, но без домена, так как домены дешевые и не сложны в настройке, а также настроить сертификат много проще для домена нежели для ip адреса.*

Создаем папку с правилами **Resolv/Rules**.

Создаем в папке файл `host.txt`:

```ini title:host.txt
127.0.0.1 mysite.room
```

Заходим в правила, нажимаем на добавление, выбираем тип **Hosts**, заполняем наименование правила и экспортируем файл.

Активируем правило.

Заходим в настройки, включаем расширенные настройки и включаем **Use System DNS as upstream DNS**.

Активируем и пробуем зайти на домен.

### Похожие статьи

[[Переключение systemd-resolved в режим stub]]