---
description: Как подключить Яндекс Вебмастер и Google Search Console
---

# Инструменты вебмастера

Сервисы для вебмастеров позволяют узнать, как «видят» ваш сайт поисковые системы, и настроить его индексирование. С их помощью можно сообщить поисковой системе о новых или удаленных страницах и улучшить отображение вашего сайта в результатах поиска.

## Как подключить Яндекс Вебмастер <a href="#yandex" id="yandex"></a>

{% hint style="info" %}
Инструкция ниже — для пользователей из России, Беларуси и Казахстана.

Если вы находитесь в другом регионе, подключите Вебмастер, вставив **метатег** в раздел настроек **«Интеграция с сервисами»**.
{% endhint %}

* [**Добавьте сайт**](https://webmaster.yandex.ru/sites/add/) в Яндекс Вебмастер. На странице введите полный адрес сайта, начиная с `https://`.

{% hint style="info" %}
Посмотреть адрес сайта можно в разделе настроек **«Адрес сайта»**.
{% endhint %}

<figure><img src="../../.gitbook/assets/ya webm add site ru.png" alt=""><figcaption></figcaption></figure>

* Для подтверждения прав на сайт выберите **«Метатег»** и скопируйте его. Метатег выглядит как `<meta name="yandex-verification" ...>`.

<figure><img src="../../.gitbook/assets/ya webm tag ru.png" alt=""><figcaption></figcaption></figure>

* На Wfolio перейдите в раздел настроек **«Инструменты вебмастера»**. Вставьте скопированный метатег в поле «Яндекс Вебмастер» и сохраните изменения.

<figure><img src="../../.gitbook/assets/ya webm add wfolio.ru.png" alt="" width="563"><figcaption></figcaption></figure>

* Вернитесь на страницу в Яндекс Вебмастере и нажмите на кнопку **«Подтвердить»**. Яндекс проверит наличие метатега на вашем сайте и подтвердит ваши права.

<figure><img src="../../.gitbook/assets/ya webm confirm ru.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Сайт будет проиндексирован вебмастером в течение 2-3 недель. Если в течение этого времени вам будут приходить сообщения об ошибках вебмастера, то их можно игнорировать.
{% endhint %}



## **Как подключить Google Search Console** <a href="#google-search-console" id="google-search-console"></a>

* Перейдите в сервис [**Google Search Console**](https://search.google.com/search-console/) и выполните вход. На открывшейся странице выберите **правую колонку «Ресурс с префиксом в URL»** и введите полный адрес своего сайта, начиная с `https://`.

{% hint style="info" %}
Посмотреть адрес сайта можно в разделе настроек **«Адрес сайта»**.
{% endhint %}

<figure><img src="../../.gitbook/assets/gsc add ru.png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
Обязательно выберите вариант добавления ресурса **«Ресурс с префиксом в URL»**.
{% endhint %}

* В окне «Подтверждение права собственности» перейдите к разделу **«Другие способы подтверждения»** и выберите **«Тег HTML»**.  Скопируйте его. Тег выглядит как `<meta name="google-site-verification" ...>`.

<figure><img src="../../.gitbook/assets/gsc tag ru.png" alt="" width="561"><figcaption></figcaption></figure>

* Передите на страницу настроек **«Инструменты вебмастера»** в панели управления Wfolio.  **Вставьте скопированный тег** в поле **«Google Search Console»** и сохраните изменения.

<figure><img src="../../.gitbook/assets/gsc add wfolio.ru.png" alt="" width="563"><figcaption></figcaption></figure>

* **Вернитесь** в Google Search Console **и нажмите** на кнопку **«Подтвердить»**. Google проверит наличие метатега на вашем сайте и подтвердит ваши права.

<figure><img src="../../.gitbook/assets/gsc tag confirm ru.png" alt="" width="561"><figcaption></figcaption></figure>

{% hint style="info" %}
Сайт будет проиндексирован вебмастером в течение 4-5 недель. Если в течение этого времени вам будут приходить сообщения об ошибках вебмастера, то их можно игнорировать.
{% endhint %}
