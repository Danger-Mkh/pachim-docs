---
title : "اجازه دسترسی پکیج‌های PHP"
---

# اجازه دسترسی پکیج‌های PHP 

### جدول محتوا 

## بررسی اجمالی

هماهنطور که در بخش [**اجازه‌دسترسی پکیج‌های PHP**](/servers/php-packages) در سرور توضیح داده‌ایم، شما می‌توانید اجازه دسترسی‌های کلی را برای نصب پکیج‌های مختلف با PHP برای همه سایت‌های یک نام کاربری سیستم عامل خود اعمال کنید. اما گاهی اوقات داستان متفاوت می‌شود و برای هر سایت، شما نیاز دارید اجازه دسترسی متفاوتی را به یک پکیج یکسان به composer اضافه کنید.

برای همین ما بخش اختصاصی اجازه دسترسی پکیج‌های PHP به هر سایت را هم اضافه کردیم که می‌توانید به شکل اختصاصی برای هر سایتی این اجازه دسترسی را ثبت کنید.

### اجازه دسترسی در سایت

زمانی که وارد پنل هر سایت در پَچیم شوید بخشی با عنوان **پکیج‌های PHP** مشاهده می‌کنید که اگر وارد آن شوید، می‌بینید که پَچیم سعی می‌کند فایل `auth.json` مربوط به composer را دریافت کند و به شما نمایش دهد. همانطور که در بررسی اجمالی هم توضیح دادیم از طریق این بخش شما می‌توانید اجازه دسترسی به پکیج‌های مختلف composer را به شکل جداگانه‌ای برای هر یک از سایت‌های خود اضافه کنید.

### اضافه کردن گواهی اجازه دسترسی قبل از نصب پکیج

برای آنکه مشکلی برای نصب پکیجی که نیاز به اجازه دسترسی از طریق Composer دارد پیش نیاید، پیشنهاد می‌کنم ابتدا اجازه دسترسی مورد نظر را در قسمت پکیج‌های PHP وارد کنید و در نهایت درخواست نصب پکیج‌های خود بر روی سایت را بدهید.

## ویرایش فایل auth.json

فایل auth.json همان فایل اصلی composer است که با آن اجازه دسترسی پکیج‌های شما انجام می‌شود زمانی که وارد صفحه پکیج‌های سرور شوید در ابتدا اطلاعات auth.json از سرور شما دریافت می‌شود و در نهایت شما می‌توانید با استفاده از گزینه اضافه کردن دسترسی، دسترسی مورد نظر خود را اضافه کنید و بعد از اضافه کردن نیاز است درخواست آپدیت کردن فایل مورد نظر را ارسال کنید تا تغییرات به شکل کامل ثبت شوند.

:::note{.tip}

توجه کنید فایل auth.json و اطلاعات داخل آن به هیچ وجه در پَچیم ذخیره سازی نمی‌شوند و اگر به هر دلیلی از طریق ssh آن را حذف کنید مجددا باید اطلاعات مورد نظر را از طریق پنل پَچیم به auth.json اضافه کنید.

:::
