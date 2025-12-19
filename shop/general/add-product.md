---
description: Как создать карточку товара в магазине
---

# Добавление товара

Вы можете продавать товары и услуги прямо на сайте или в галереях, настроив оплату и форму заказа. Это может быть физический товар или цифровой продукт, консультация, заявка на съемку и т.д.

### Как создать товар <a href="#add" id="add"></a>

* Перейдите в магазин и нажмите на кнопку **«Добавить товар»**.
* Напишите название и описание товара/услуги, добавьте изображения.

<figure><img src="../../.gitbook/assets/add product ru.png" alt="" width="563"><figcaption></figcaption></figure>

* Выберите способ оплаты:

1. **Онлайн-оплата** — если вы хотите принимать платежи на сайте. Не забудьте подключить [платежную систему](../payment/payment-systems.md).
2. **Оплата наличными** — клиент сделает заказ, а вы свяжетесь с ним лично.

<figure><img src="../../.gitbook/assets/choose payment options ru.png" alt="" width="563"><figcaption></figcaption></figure>

* Укажите цену товара или услуги. Можно добавить несколько цен для разных версий: [#variations](add-product.md#variations "mention").
* Включите переключатель **«Разрешить выбор количества»** для заказа нескольких позиций товара сразу.
* Нажмите на кнопку **«Добавить»**, чтобы сохранить товар. Если нужно, настройте сбор контактов или действия после заказа по инструкциям ниже.

### Варианты цены для товара <a href="#variations" id="variations"></a>

Перейдите во вкладку **«Цена за варианты»**, чтобы установить разные цены в зависимости от версии товара или услуги. Это могут быть разные размеры для печати, пакетов услуг и т.д.

Можно добавить до 7-ми вариантов.

<figure><img src="../../.gitbook/assets/add product variations ru.png" alt="" width="563"><figcaption></figcaption></figure>

Посмотрите страницу с примером такого товара:

{% embed url="https://demo.wfolio.pro/fotokartiny" %}

### Как настроить сбор данных в форме заказа <a href="#form" id="form"></a>

Форма заказа позволяет собирать нужную информацию от клиента. По умолчанию запрашивается **имя клиента** (и **email** при онлайн-оплате).

Чтобы получить дополнительную информацию о клиенте, перейдите во вкладку **«Настройки формы заказа»** и добавьте другие поля:

* Телефон.
* Текстовое поле — для коротких ответов (например, страница клиента в соцсетях).
* Выпадающий список — если клиенту нужно выбрать одну из опций.
* Комментарий — для развернутого сообщения от клиента.

<figure><img src="../../.gitbook/assets/product form settings ru.png" alt="" width="563"><figcaption></figcaption></figure>

Пример настройки формы: при заказе клиент указывает номер телефона, профиль в соцсети, выбирает нужную опцию и пишет адрес доставки.

<figure><img src="../../.gitbook/assets/product form settings example ru.png" alt="" width="563"><figcaption></figcaption></figure>

### Как настроить действие после заказа <a href="#actions" id="actions"></a>

✔ Можно перенаправить покупателя на нужную страницу или специальный адрес (где можно что-то скачать или посмотреть).\
✔ Или отправить письмо с подтверждением заказа и дополнительной информацией.

Для этого в карточке перейдите во вкладку **«После заказа»**.

<figure><img src="../../.gitbook/assets/after order settings ru.png" alt="" width="563"><figcaption></figcaption></figure>

* **Переход на страницу**:
  * На внешний адрес — вставьте любую ссылку. Например: на [файл](../../site/content/add-file.md), на закрытый чат в Telegram, на другой сайт.
  * На страницу сайта — выберите уже созданную страницу. Доступно на тарифах с [конструктором сайта](../../billing/plans.md#site-and-drive).

<figure><img src="../../.gitbook/assets/move to page after order setting ru.png" alt="" width="563"><figcaption></figcaption></figure>

* **Письмо после оплаты.** Напишите текст письма, которое будет направлено клиенту после покупки. Используйте панель форматирования текста, чтобы сделать текст жирным <mark style="background-color:blue;">**(B)**</mark>, курсивом <mark style="background-color:blue;">**(I)**</mark>, подчеркнутым <mark style="background-color:blue;">**(U)**</mark>, зачеркнутым <mark style="background-color:blue;">**(S)**</mark> или [вставить ссылку](../../site/content/links.md#text).

<figure><img src="../../.gitbook/assets/letter after order settings ru.png" alt="" width="563"><figcaption></figcaption></figure>



### Где разместить товар или услугу?

✔ **На странице сайта**. Смотрите подробнее здесь: [products.md](../site/products.md "mention")

✔ **В галерее на диске**. Смотрите инструкцию: [products.md](../gallery/products.md "mention")

✔ А ещё можно **поделиться ссылкой на отдельную страницу с товаром**. Для этого после добавления товара нажмите на стрелку возле нужного товара и скопируйте ссылку на него.

#### Похожие статьи

{% content-ref url="../gallery/" %}
[gallery](../gallery/)
{% endcontent-ref %}

{% content-ref url="../site/" %}
[site](../site/)
{% endcontent-ref %}

{% content-ref url="../site/client-account.md" %}
[client-account.md](../site/client-account.md)
{% endcontent-ref %}

{% content-ref url="../site/certificates.md" %}
[certificates.md](../site/certificates.md)
{% endcontent-ref %}

{% content-ref url="../site/thank-you-page.md" %}
[thank-you-page.md](../site/thank-you-page.md)
{% endcontent-ref %}

{% content-ref url="../../site/content/add-file.md" %}
[add-file.md](../../site/content/add-file.md)
{% endcontent-ref %}
