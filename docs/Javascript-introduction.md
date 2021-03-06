---
id: javascript-introduction
title: معرفی جاوا‌اسکریپت
sidebar_label: معرفی Javascript
---

## ظهور

جاوا اسکریپت یکی از معروف ترین زبان های برنامه نویسی دنیاست که حدودا ۲۰ سال پیش به وجود اومد
 و زمان نسبتا زیادی هم طول کشید تا به یک زبان خوب و قابل اعتماد تبدیل بشه.

> جاوا اسکریپت اولین و تنها زبان برنامه‌ نویسی هست که به صورت native در مرورگرها مورد استفاده قرار می‌گیره.

یادتونه همین چند سال پیش وبلاگ‌ها پر بودن از انیمیشن‌های عجیب و غریب، مثل بارش برف، جوونورهایی که دنبال موس راه میوفتادن و برامون خیلی عجیب و جذاب بودن؟ خوب این ها تقریبا بیشترین و اصلی‌ترین استفاده هایی بود که از جاوا اسکریپت میشد!

ولی کم کم با توسعه پیدا کردن و همه‌گیر شدن وب، جاوا اسکریپت هم احتیاج به رشد داشت تا بتونه نیازهای بزرگترین و پر‌ استفاده ترین اکوسیستم دنیا (یعنی) وب رو پاسخ‌گو باشه.

خیلی از چیزها در این پلتفرم، توسط API مرورگرها فراهم شد، ولی خود زبان جاوا اسکریپت هم رشد وسیع و سریعی شاهد بود.

جاوا اسکریپت در حال حاضر به شکل وسیعی در خارج از مرورگرها مورد استفاده قرار می‌گیره. ظهور Node.js در سال‌های اخیر باعث شده این زبان در کنار زبان های Server side مطرحی همچون Java, Ruby, Python, Php و ... دیده بشه.

> در حال حاضر جاوا اسکریپت به شکل گسترده ای در دیتابیس ها، سخت افزارها، ساخت نرم افزارهای قابل اجرا در سیستم عامل‌های مختلف، موبایل ها و ... مورد استفاده قرار گرفته، زبانی که روزی فقط در مرورگرها استفاده می‌شد، حالا به معروف‌ترین و پر استفاده ترین زبان برنامه نویسی دنیا تبدیل شده.

## تعریف اولیه

جاوا اسکریپت زبانی هست که:

High level: به این معنی که این زبان فضایی برای شما فراهم کرده که به جای درگیر شدن با کارهای پیچیده، مثل مدیریت حافظه، یا مفاهیم پیچیده تر، تمرکزتون رو روی کار اصلی بذارید.

**Dynamic**: برعکس زبان های برنامه نویسی `static`, زبان جاوا اسکریپت خیلی از چیزهایی که زبان های استاتیک در زمان کامپایل آماده می‌کنند رو در زمان اجرا آماده می‌کنه. این مورد فواید و اشکالاتی داره و به ما قابلیت‌های مفیدی مثل، `dynamic typing`, `late binding`, `reflection`,
`functional programming`, `object runtime alteration`, `closures` و خیلی چیزهای دیگه میده.

**Dynamically typed**: به این معنا که متغیرها ما را وادار به داشتن type مشخص نمی‌کنند.
شما می‌تونید هروقت مایل بودید هر نوع `type` دیگری رو به یک `variable` assign کنید، به عنوان مثال یک `number` رو به `var` که یک رشته رو نگه داری می‌کنه assign کنید.

**Weakly typed**: برعکس زبان های `strong type`, زبان های `weakly typed` هیچ اجباری برای `type` های یک آبجکت ندارن.
این امکان به دستمون رو باز میذاره، ولی امکان  `type checking` رو از ما میگره، چیزی که با کمک `Flow` یا `TypeScript` قابل حله.

**Interpreted**: به این معنی که برعکس زبان هایی مثل `C`, `Java` یا `Go`, جاوا اسکریپت قبل از اجرا نیازی به کامپایل شدن ندارد و به اصلاح یک زبان مفصری‌ست. مرورگر قبل از اجرای کدهای جاوااکریپت آن را کامپایل می کند و شما لازم نیست هیچ کار اضافه ای انجام دهید.

**Multi-paradigm**: جاوا اسکریپت برنامه نویسانش را به سبک خاصی از برنامه نویسی وادار نمی‌کند. به این معنا که برعکس زبانی مثل `Java` که برنامه نویسان را به سبک نوشتن `Object oriented` وادار میکند، یا زبان `C` که شما را به نوشتن `Impretive` سوق می‌دهد، در جاوا اسکریپت شما می توانید هر سبکی را که می پسندید انتخاب نمایید. مثل شی گرایی، دستوری (مثل `C`) و `Functional`.

> جالبه بدانید زبان `Javascript` هیچ ربطی به `Java` نداره. متاسفانه این فقط یک انتخاب بد برای این زبان به حساب می‌یاد.

## نسخه های مختلف جاوا اسکریپت

اجازه بدید اصطلاح `ECMAScript` را همین‌جا معرفی کنم. ما یک [بخش کامل](javascript-ecmascript.md) رو به معرفی و آموزش `ECMAScript` اختصاص دادیم. ولی فقط برای آشنایی این را بدانید که اکمااسکریپت که به `ES` هم معروفه یک استاندارد برای زبان جاوا اسکریپت به حساب می‌یاد.

جاوا اسکریپت یک پیاده سازی از این استاندارد محسوب می‌شه و به خاطر همینه که شما اصطلاحاتی مثل ES6, ES2015, ES2019 و ... را زیاد می‌شنوید.

برای مدت زمان طولانی نسخه ES3 جاوا اسکریپت در مرورگرها اجرا می‌شد. بعد از اون پروژه نسخه 4 به علت تغییرات بسیار زیادی که یکباره اعمال کرده بودند متوقف شد. سپس نسخه 5 که بزرگترین آپدیت به حساب می آمد معرفی و مورد استفاده قرار گرفت. بعد از آن در سال 2015 نسخه E2015 که به ES6 هم شناخته می‌شه وارد صحنه شد که انقلابی بزرگ برای این زبان به حساب می آمد.

> در حال حاضر آخرین نسخه جاوا اسکریپت `ES2018` است.