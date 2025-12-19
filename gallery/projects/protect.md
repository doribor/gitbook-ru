# Защита галерей и фотографий

Галереи доступны по уникальной прямой ссылке, которой вы делитесь с клиентами. Галереи, в отличие от страниц на сайте, нельзя найти через поиск в интернете благодаря **защите от индексации**.

### Защитный ключ в ссылке

Применяется ко всем галереям. К ссылкам в адресе галереи добавляется уникальный защитный ключ, который защищает от несанкционированного доступа к файлам путем перебора ссылок. Пример того, как выглядит **ключ**: `https://mydomain.ru/disk/alexander`**`-7dks03`**.

Эта настройка по умолчанию активна. Управлять защитным ключом можно в разделе **«Настройки диска»**.



### Водяной знак

Настраивается отдельно для каждой галереи. Перейдите в раздел настроек **«Настройки диска»**. Загрузите водяной знак **с прозрачным фоном в формате PNG**.

После загрузки можно настроить размер знака и его непрозрачность.

<figure><img src="../../.gitbook/assets/watermark drive.png" alt="" width="563"><figcaption></figcaption></figure>

Чтобы включить водяной знак в галерее, перейдите в настройки проекта и запретите скачивание оригиналов. После этого активируйте опцию **«Добавить на фотографии водяной знак»**.

<figure><img src="../../.gitbook/assets/project enable watermark.png" alt="" width="563"><figcaption></figcaption></figure>

При [продаже цифровых фотографий](../../shop/gallery/digital-photos.md) водяной знак активируется автоматически.

<figure><img src="../../.gitbook/assets/photo sell.png" alt="" width="563"><figcaption></figcaption></figure>

Знак накладывается сеткой на все фотографии в галерее. Посмотрите на примеры галерей с водяным знаком:

<table data-card-size="large" data-view="cards" data-full-width="false"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-cover data-type="files"></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>Продажа фотографий</td><td></td><td></td><td></td><td><a href="https://demo.wfolio.pro/disk/nature">https://demo.wfolio.pro/disk/nature</a></td></tr><tr><td>Клиентская галарея</td><td></td><td></td><td></td><td><a href="https://demo.wfolio.pro/disk/red-mood">https://demo.wfolio.pro/disk/red-mood</a></td></tr></tbody></table>



### Пароль

Настраивается отдельно для каждой галереи. В настройках проекта перейдите во вкладку **«Пароль»**. Активируйте опцию **«Защитить проект паролем»** и установите нужную комбинацию.

<figure><img src="../../.gitbook/assets/set password ru.png" alt="" width="563"><figcaption></figcaption></figure>

При входе в галерею потребуется ввести указанный вами пароль.

<figure><img src="../../.gitbook/assets/pasword-protected gallery.png" alt=""><figcaption></figcaption></figure>

Если нужно дать заказчику доступ к скрытым папкам в галерее, но показать папки в открытом доступе для всех, воспользуйтесь функцией [гостевого доступа](hidden-folders.md).

{% hint style="info" %}
Пароль настраивается один раз для всей галереи. Если в галерее несколько папок, все они будут доступны по одному паролю — отдельные пароли для доступа к разным папкам не настраиваются.
{% endhint %}
