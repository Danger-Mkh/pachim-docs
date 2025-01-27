---
title : 'مدیریت مخزن‌ها'
---
# مدیریت مخزن‌ها 

### جدول محتوا 

## معرفی 

ارائه کننده‌های repository این اجازه را به پَچیم می‌دهند تا با دسترسی پیدا کردن به اطلاعات کلی repository، برنامه شما را به سادگی در سرور شما مستقر کند. پَچیم از ارائه کننده‌های معرف Git در کنار حالت‌های سفارشی و Self-hosted پشتیبانی می‌کند.

## ارائه کننده‌های پشتیبانی شده 

در حال حاضر ما در پَچیم ارائه کننده‌های مخزن‌ Git زیر را پشتیبانی می‌کنیم

- گیت هاب
- گیت لب (شامل سایت اصلی و self-hosted)
- ریپازیتوری git سفارشی

:::note{.tip}
در توضیحات این صفحه منظور از **ارائه کننده** وبسایت‌های همچون گیت‌هاب یا گیت‌لب یا مواردی که از آن‌ها پشتیبانی می‌کنیم هستند.
:::
### استفاده از ارائه کننده سفارشی

منظور از ارائه کننده سفارشی چیست؟ زمانی که شما به دلایل مختلف مایل نیستید دسترسی ارائه کننده Git خود را از طریق گیت هاب و گیت لب به پَچیم دهید یا اصلا در حال استفاده از یک ارائه کننده کاملا شخصی هستید، در پَچیم قابلیتی را آماده سازی کرده‌ایم که با استفاده از آن و بدون دادن هیچ دسترسی به پَچیم می‌توانید مستقیما تنها به سرور خود اجازه دسترسی به Repository مورد نظرتان را دهید.

برای انجام این کار، بعد از اینکه سایت خود را ایجاد کردید وارد بخش اپلیکیشن شوید و گزینه ارائه کننده سفارشی را انتخاب کنید. زمانی که این گزینه را انتخاب می‌کنید پَچیم از شما می‌خواهد کلید SSH سرور مورد نظرتان را در ارائه کننده مخزن GIT در بخش SSHها وارد کنید

در قدم بعد در قسمت آدرس Repository باید یک آدرس به شکل `(git@provider.com:user/repository.git)` در قسمت مورد نظر در نصب اپلیکیشن وارد کنید.

بعد از مقدار دهی کردن آدرس git سفارشی، نیاز است نام شاخه (branch) موجود در پروژه که قصد دارید بر روی سایت بارگذاری کنید، را وارد کنید 

## مدیریت ارائه کننده‌ها

### اتصال به ارائه کننده جدید

برای اتصال ارائه کننده‌هایی مثل Github و Gitlab که خودتان میزبانی می‌کنید، می‌توانید به بخش [مدیریت مخزن‌ها](https://app.pachim.sh/panel/user-profile/providers) در پروفایل کاربری وارد شوید و از طریق این صفحه اتصال به اکانت هر کدام از موارد که نیاز دارید را انجام دهید.

:::note{.tip}

موضوع مهمی که در پَچیم وجود دارد این است که شما می‌توانید اکانت‌های متفاوتی از گیت هاب و گیت لب را به شکل همزمان در اکانت خود داشته باشید و این به شما اجازه می‌دهد به شکل همزمان کلی وبسایت مختلف با مخزن‌های مختلف در اکانت‌های مختلف را در پَچیم مدیریت کنید.

:::

### اتصال به گیت‌لب Self Hosted

در موارد مختلفی به هر دلیلی ممکن است از ورژن Self-Hosted مربوط به گیت‌لب بر روی سرور خود استفاده کنید تا بتوانید از پروژه‌هایتان نگه‌داری کنید، ما در پَچیم اجازه اتصال این نوع ارائه کننده را هم به شما می‌دهیم تا بتوانید به سادگی گیت‌لب Self-Hosted خود را به پَچیم متصل کنید و وبسایت خود را راه‌اندازی کنید.

برای اتصال تنها کافیست وارد بخش مدیریت مخزن‌ها در پَچیم شوید و بر روی گزینه اضافه کردن مخزن Self-hosted-gitlab کلیک کنید.

از شما چند اطلاعات مهم برای اتصال درخواست خواهد کرد.

- **نام کاربری:** این نام کاربری می‌تواند نام کاربری root یا هر نام کاربری که با گیت‌لب خود میزبان ساخته‌اید باشد.
- **آدرس اصلی:** برای اتصال به api گیت‌لب خود میزبان شما، ما نیاز به دامنه اصلی آن داریم.
- **توکن دسترسی:** شما می‌توانید این توکن را از طریق بخش Personal Access Token ایجاد کنید و نیاز است برای توکن ایجاد شده دسترسی api را انتخاب کنید.
- در نهایت ورژن گیت‌لب شخصی خود را انتخاب کنید (**در حال حاضر ورژن ۴ پشتیبانی می‌شود**)

:::note{.warning}

::title[پورت SSH]

توجه کنید پورت SSH سرور گیت‌لب خود میزبان شما باید 22 باشد در غیر این صورت برای اتصال ارائه کننده به پَچیم و همچنین دریافت پروژه‌ها بر روی سرور خود دچار مشکل خواهید شد.

:::

قبل از آنکه گیت‌لب خود میزبان را به پَچیم متصل کنید ابتدا SSH KEY سیستم خود را در بخش SSH KEY گیت‌لب خود میزبان قرار دهید و در یک ترمینال از سیستم خودتان دستور زیر را اجرا کنید اگر پیام Welcome را مشاهده کردید می‌توانید مطمئن باشید برای ارتباط پَچیم با گیت‌لب خود میزبان شما هم مشکلی وجود ندارد.

```shell
ssh -T git@gitlab.example.com
```

به جای `gitlab.example.com` میتوانید هر دامنه‌ای که مربوط به گیت لب خود میزبان شما هست را وارد کنید.

### بستن دسترسی ارائه کننده

برای قطع کردن ارتباط پَچیم با مخزن مورد نظر شما، تنها کافیست از صفحه مدیریت مخزن‌های پَچیم روی گزینه حذف مخزنی که مورد نظر شماست کلیک کنید تا دسترسی مخزن مورد نظر به شکل کامل از پَچیم حذف شود.

:::note{.warning}

توجه کنید اگر دسترسی به اکانت مخزن را در پَچیم ببندید و اپلیکیشن وبسایتی را که از قبل با آن اکانت بالا آورده باشید، دقت کنید که بستن دسترسی ارائه کننده می‌تواند باعث مشکل در استقرار آپدیت‌های برنامه شما شود.

:::

### ریست کردن دسترسی ارائه کننده

در صورت اینکه مشکلی در دسترسی به مخزن مورد نظر در پَچیم وجود دارد می‌توانید از طریق صفحه مدیریت مخزن‌ها ابتدا اکانت مخزن مورد نظر را حذف کرده و مجددا بر روی اضافه کردن مخزن کلیک کنید تا کلید دسترسی در پَچیم ریست شود. 
