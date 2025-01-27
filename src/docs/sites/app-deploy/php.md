---
title : "برنامه PHP"
---

# برنامه PHP

### جدول محتوا

## بررسی اجمالی

پَچیم سعی می‌کند فضایی را آماده کند تا با استفاده از آن بتوانید برنامه‌های مختلفی را بر روی سرور خود بالا بیاورید، یکی از این دسته برنامه‌ها، برنامه‌های PHP است، که به سادگی می‌توانید یک وبسایت PHP با پَچیم بالا آوردید و آن را مدیریت کنید.

:::note{.warning}
::title[نکته بسیار مهم]

دقت کنید برای آنکه دامنه شما به سایت‌تان که با پَچیم راه‌اندازی می‌کنید متصل شود، باید دامنه مورد نظرتان را به سرور خود متصل کنید که این کار را از طریق راهنمای [`اتصال دامنه به سایت`](/sites/setup-site/connect-domain-to-site) برای‌تان توضیح داده‌ایم.

:::

## راه‌اندازی برنامه PHP

برای راه‌اندازی یک پروژه PHP ابتدا نیاز است سایت مورد نظر را در سرور خودتان از طریق پنل پَچیم بوجود آورید، بعد از کلیک بر روی دکمه ایجاد سایت جدید، نوع برنامه خود را PHP قرار دهید. اینکار باعث می‌شود امکانات مورد نظر PHP بر روی پنل سایت در اختیار شما قرار بگیرد. 

بعد از وارد کردن مابقی اطلاعات لازم سایت با کلیک بر روی ایجاد کردن سایت، وبسایت شما ایجاد می‌شود و از طریق **[بخش استقرار](/sites/deployments)** می‌توانید به سادگی پروژه خود را بر روی سرورتان قرار دهید.

## اجازه دسترسی پکیج‌های PHP

اگر زمانی از پکیجی از php استفاده می‌کنید که برای نصب آن نیاز به بررسی اجازه دسترسی از طریق Composer است، می‌توانید از بخش [پکیج‌های PHP](/sites/php-packages) در پنل مربوط به سایت خود، این اجازه دسترسی را به composer اضافه کنید. 

## داشتن فایل .env

اگر از سیستم متغیرهای محیط برنامه در فایل `.env` برای پروژه PHP خود استفاده می‌کنید و نیاز به این دارید که متغییرهای فایل `.env` را تغییر دهید یا چیزی را به آن اضافه کنید، می‌توانید از طریق پنل سایت خود در پَچیم وارد بخش **متغیرهای محیط برنامه** شوید و متغیرهای که مد نظر دارید را بر روی آن قرار دهید.

در پروژه‌های php به روش‌های مختلف می‌توان متغیرهای محیطی را به برنامه اضافه کرد اما یکی از ابزارهایی که می‌تواند در PHP کمک کند، استفاده از پکیج [phpdotenv](https://github.com/vlucas/phpdotenv) اگر تا به حال از این ویژگی استفاده نکردید و قصد دارید از این امکان در پَچیم بهرمند شوید می‌توانید مستند این پکیج را مطالعه کنید.

## مشاهده لاگ‌ها

اگر در برنامه خود لاگ‌ها را در فایل خاصی ذخیره سازی می‌کنید، می‌توانید از طریق پنل پَچیم خروجی لاگ‌ها را همیشه مشاهده کنید. برای انجام اینکار تنها کافیست یک [لاگ سفارشی](/sites/logs#لاگهای-سفارشی) در پَچیم بوجود آورید و در قدم بعد آن راه مشاهده کنید.

## اتصال به دیتابیس

برای اتصال پروژه PHP به دیتابیس، نیاز به یک دیتابیس و کاربر دیتابیس و پسورد آن دارید. شما می‌توانید به سادگی از طریق [پنل دیتابیس‌های سرور پَچیم](/servers/databases) و اطلاعات مورد نیاز خود را ایجاد کنید.

در نهایت به سادگی می‌توانید از طریق اطلاعات دیتابیسی که ایجاد کردید و پیکربندی آن در برنامه php به دیتابیس مورد نظر متصل شوید و اطلاعات خود را در آن ذخیره سازی کنید.

## ارسال ایمیل

در حال حاضر بر روی سرور شما sendmail نصب شده و شما می‌توانید به شکل native با استفاده از تابع mail عمل ارسال ایمیل را انجام دهید.

همچنین شما می‌توانید سرویس SMTP ارسال ایمیل را از جاهای دیگر تهیه کنید و از آن برای ارسال ایمیل خود استفاده کنید. 

## کار با صف‌ها

اگر شما در برنامه خود، دستور کامندی را برای اجرای صف دارید ‌می‌توانید از بخش [سرپرست‌های سرور](/servers/supervisor) اقدام به اضافه کردن صف مورد نظر خود برای وبسایت‌تان کنید.
