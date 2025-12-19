---
description: Как подключить поддомен к сайту или диску
---

# Подключение поддомена

Если у вас есть зарегистрированный домен `mydomain.ru`, вы можете подключить поддомен вида `gallery.mydomain.ru` к сайту или диску. К одному аккаунту (сайту или диску) подключается один домен или поддомен.

{% hint style="success" %}
Если вы регистрировали домен [на Wfolio](new.md#how-to-register) или подключили ваш домен через [DNS-серверы Wfolio](existing-domain.md#dns-records), для подключения поддомена напишите нам в чат поддержки.
{% endhint %}



* Перейдите в раздел настроек **«Адрес сайта»** или **«Веб-адрес диска»** и нажмите на **«У меня уже есть домен»**.

<figure><img src="../.gitbook/assets/connect existing domain ru.png" alt="" width="563"><figcaption></figcaption></figure>

* Введите в поле нужный вам поддомен. Например, `gallery.mydomain.ru`. Нажмите на кнопку **«Подключить»**.

<figure><img src="../.gitbook/assets/connect subdomain ru.png" alt="" width="563"><figcaption></figcaption></figure>

* Настройте поддомен в личном кабинете регистратора.



## Настройка поддомена у регистратора

Добавьте для домена две A-записи с IP-адресом, ведущим на Wfolio:

1. Для первой записи укажите поддомен `gallery` (или любой другой) в имени записи (хоста).
2. Для второй записи укажите имя записи (хост) с `www`: например, `www.gallery`.

Некоторые регистраторы перед добавлением записей для поддомена требуют сначала создать поддомен.



Настроить работу домена можно на серверы в России, Европе (подойдет для работы сайта во всем мире), Казахстане или Беларуси.

#### Серверы России

<table><thead><tr><th width="189">Тип</th><th width="182">Имя (хост)</th><th width="191">Значение</th><th>TTL</th></tr></thead><tbody><tr><td>А</td><td>gallery</td><td><strong>5.188.130.118</strong></td><td>3600</td></tr><tr><td>А</td><td>www.gallery</td><td><strong>5.188.130.118</strong></td><td>3600</td></tr></tbody></table>

#### Серверы Европы

<table><thead><tr><th width="189">Тип</th><th width="182">Имя (хост)</th><th width="191">Значение</th><th>TTL</th></tr></thead><tbody><tr><td>А</td><td>gallery</td><td><strong>103.137.248.164</strong></td><td>3600</td></tr><tr><td>А</td><td>www.gallery</td><td><strong>103.137.248.164</strong></td><td>3600</td></tr></tbody></table>

#### Серверы Казахстана

<table><thead><tr><th width="189">Тип</th><th width="182">Имя (хост)</th><th width="191">Значение</th><th>TTL</th></tr></thead><tbody><tr><td>А</td><td>gallery</td><td><strong>213.148.2.60</strong></td><td>3600</td></tr><tr><td>А</td><td>www.gallery</td><td><strong>213.148.2.60</strong></td><td>3600</td></tr></tbody></table>

#### Серверы Беларуси

<table><thead><tr><th width="189">Тип</th><th width="182">Имя (хост)</th><th width="191">Значение</th><th>TTL</th></tr></thead><tbody><tr><td>А</td><td>gallery</td><td><strong>45.135.234.71</strong></td><td>3600</td></tr><tr><td>А</td><td>www.gallery</td><td><strong>45.135.234.71</strong></td><td>3600</td></tr></tbody></table>

{% hint style="info" %}
После ввода настроек поддомен должен подключиться **в течение 2-х суток**.
{% endhint %}

***

Если в процессе подключения у вас возникла сложность, напишите нам в чат поддержки.
