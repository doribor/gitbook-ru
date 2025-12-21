---
description: Подключение платежной системы Stripe
---

# Подключение Stripe

[**Stripe**](https://stripe.com/) — это платежная система для предпринимателей в [более чем 40 странах](https://stripe.com/global), которая позволяет принимать платежи от клиентов по всему миру.

{% hint style="info" %}
Stripe не работает в России и странах СНГ. Для приема платежей от иностранных клиентов в России подключите платежную систему [Robokassa](robokassa.md).
{% endhint %}



### Список доступных валют <a href="#currencies" id="currencies"></a>

Доступные валюты включают  EUR, USD, GBP, CHF, DKK, SEK, AUD, KZT, ILS, INR, RON, PLN, BGN, THB, AED, CZK, CAD, BRL. Всего доступно более 130 валют. **Российские рубли не поддерживаются.** Минимальная сумма к оплате варьируется в зависимости от валюты.

<a href="https://docs.stripe.com/currencies?presentment-currency" class="button secondary">Все валюты</a>   <a href="https://docs.stripe.com/currencies?presentment-currency=AU#minimum-and-maximum-charge-amounts" class="button secondary">Минимальная сумма платежа</a>

### Как подготовиться к подключению

Добавьте товары или услуги [на сайт](../shop/site/products.md) или [в галерею](../shop/gallery/products.md). Для успешного прохождения проверки платежной системы важно, чтобы были указаны:

* **Описание товаров и услуг.**
* **Стоимость.** Цены и тарифы должны быть видны пользователю перед оформлением заказа.
* **Способы доставки и получения.** Как пользователь получит товар или услугу после оплаты.
* **Контакты и реквизиты.** ФИО, телефон, адрес электронной почты, реквизиты самозанятого или ИП.
* **Ссылка на** [**оферту с юридической информацией**](../legal/terms.md)**.**

### Как подключить Stripe

* Зайдите на сайт [**Stripe**](https://stripe.com/) и зарегистрируйтесь. Заполните все требуемые поля.
* После регистрации вам на почту придет письмо подтверждения — перейдите по ссылке в письме.
* После подтверждения почты заполните информацию о вашем бизнесе для активации аккаунта. Подробно опишите вашу компанию в каждом пункте. Для этого перейдите по кнопке [**«Add business information»**](https://dashboard.stripe.com/account/onboarding).
* После активации компании перейдите во вкладку **«Developers»** → [**«Webhooks»**](https://dashboard.stripe.com/webhooks). Нажмите на кнопку **«Add destination»**.

<figure><img src="../.gitbook/assets/stripe add destination.png" alt=""><figcaption></figcaption></figure>

* В **«Events»** в поиске найдите и выберите события **«checkout.session.completed»** и **«checkout.session.expired»**.

<figure><img src="../.gitbook/assets/stripe select events.png" alt=""><figcaption></figcaption></figure>

* В «Destination types» выберите **«Webhook endpoint»**.

<figure><img src="../.gitbook/assets/stripe webhook endpoint.png" alt=""><figcaption></figcaption></figure>

* В пункте **«Endpoint URL»** пропишите этот адрес:

```
https://wfolio.com/gateway/integrations/stripe/notify
```

{% hint style="danger" %}
#### Почему важно вставить правильный адрес в **«**&#x45;ndpoint UR&#x4C;**»**

Если не указать его или указать неверный адрес, данные об оплаченном заказе не поступят на сервер Wfolio.

Статус заказа останется незавершенным и [действие после заказа](../shop/general/add-product.md#actions) или [покупка цифровых фото](../shop/gallery/digital-photos.md) не будут выполнены — даже если оплата прошла успешно и вы получили деньги.
{% endhint %}

* Нажмите на **«Create endpoint»**.

<figure><img src="../.gitbook/assets/stripe destination.png" alt=""><figcaption></figcaption></figure>



Для подключения системы Stripe понадобится два ключа: секретный API-ключ и секретный ключ вебхука. Сначала опишем, как скопировать и вставить секретный API-ключ.

* Перейдите в раздел «Developers» → [**«API Keys»**](https://dashboard.stripe.com/apikeys), нажмите на кнопку **«Reveal key»** и **скопируйте «Secret key»**.

<figure><img src="../.gitbook/assets/stripe api key.png" alt=""><figcaption></figcaption></figure>

* Ключ для второго поля находится во вкладке **«Developers»** → [**«Webhooks»**](https://dashboard.stripe.com/webhooks). В разделе **«Webhook endpoints»** перейдите в добавленный endpoint.

<figure><img src="../.gitbook/assets/stripe go to endpoint.png" alt=""><figcaption></figcaption></figure>

* В строке **«Signing secret»** нажмите на **«Reveal»**. Скопируйте его.

<figure><img src="../.gitbook/assets/stripe whkey 2.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
В инструкции прописан способ подключения в **тестовом режиме**. Чтобы отключить тестовый режим, нажмите на переключатель **«Test mode»** в верхнем правом углу и **скопируйте ключи** еще раз.
{% endhint %}



Перейдите в раздел магазина **«Платежные сервисы»**. Вставьте скопированные ключи: API-ключ — в поле **«Секретный ключ»**, ключ вебхука (начинается с `wh`) — в поле **«Секретный ключ вебхука»**.

Если нужно, чтобы покупатель ввел физический адрес в окне оплаты, активируйте переключатель «Запрашивать адрес для биллинга».

<figure><img src="../.gitbook/assets/wfolio stripe keys ru.png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="warning" %}
#### Проведите тестовый платеж после подключения системы

У Stripe есть минимальная для оплаты сумма. Например, для долларов — 0.5 USD. Проверьте сумму для минимального платежа [здесь](https://docs.stripe.com/currencies#minimum-and-maximum-charge-amounts).

Ваш заказ должен отобразиться в разделе **«Магазин» → «Заказы»**.

Если оплата прошла, но заказа нет или спустя несколько часов он появился в разделе «Незавершенные заказы», проверьте настройки платежной системы еще раз. Секретные ключи и адрес в «Endpoint URL» должны быть указаны в соответствии с инструкцией выше.
{% endhint %}
