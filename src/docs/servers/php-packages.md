---
title : "اجازه دسترسی پکیج‌های PHP"
---

# اجازه دسترسی پکیج‌های PHP 

### جدول محتوا 

## بررسی اجمالی

ما در پَچیم سعی کرده‌ایم بهترین تجربه کار با PHP و Composer را به شما ارائه دهیم. در حال حاضر پروژه‌های PHP از پکیج‌های زیاد و مختلفی از Composer استفاده می‌کنند که گاهن بعضی از این پکیج‌ها نیاز به اجازه دسترسی دارند ما امکانی را در پَچیم به وجود آورده‌ایم که شما می‌توانید اجازه دسترسی پکیج composer را در سرور انجام دهید.

### اجازه دسترسی کلی سرور

Composer قابلیتی را دارد که به شما اجازه می‌دهد اگر چندین سایت را در یک نام کاربری در سیستم عامل خود ایجاد می‌کنید به شکل واحد هم بتوانید اجازه دسترسی پکیج‌های مجموعه آن سایت‌ها را برای Composer انجام دهید.

یعنی اگر شما چند سایت را به سرورتان در حالت پیش فرض اضافه کنید، این چند سایت توسط کاربر پیشفرض یعنی pachim ایجاد خواهند شد و شما می‌توانید به سادگی با ذخیره سازی کردن توکن یا http-basic مربوط به پکیج خود این اعتبارنامه را برای تمام سایت‌های کاربر مورد نظر استفاده کنید. البته اگر قصد دارید اعتبارنامه‌ها را به شکل اختصاصی تری برای هر سایت استفاده کنید می‌توانید به صفحه [**پکیج‌های PHP**](/sites/php-packages) برای سایت‌ها مراجعه کنید

### تغییر Auth.json برای کاربران مختلف

اگر شما وبسایت‌های مختلفی را در حالت کاربر ایزوله ایجاد کرده باشید در سرور شما چند نام کاربری متفاوت وجود دارد که شما می‌توانید برای هر کدام از این نام‌های کاربری `auth.json` متفاوتی داشته باشید و آن را مدیریت کنید.

## ویرایش فایل auth.json

فایل auth.json همان فایل اصلی composer است که با آن اجازه دسترسی پکیج‌های شما انجام می‌شود زمانی که وارد صفحه پکیج‌های سرور شوید در ابتدا اطلاعات auth.json از سرور شما دریافت می‌شود و در نهایت شما می‌توانید با استفاده از گزینه اضافه کردن دسترسی، دسترسی مورد نظر خود را اضافه کنید و بعد از اضافه کردن نیاز است درخواست آپدیت کردن فایل مورد نظر را ارسال کنید تا تغییرات به شکل کامل ثبت شوند.

:::note{.tip}

توجه کنید فایل auth.json و اطلاعات داخل آن به هیچ وجه در پَچیم ذخیره سازی نمی‌شوند و اگر به هر دلیلی از طریق ssh آن را حذف کنید مجددا باید اطلاعات مورد نظر را از طریق پنل پَچیم به auth.json اضافه کنید.

:::
