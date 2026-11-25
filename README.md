# راهنمای جامع انتخاب و کاربرد وریستور | Varistor Selection & Application Guide

<p align="center">
  <img src="Images/GitHub-Assets/MES-Hero-Banner.svg" width="100%" alt="MEMAR ELECTRONIC SANAT — MES">
</p>

<p align="center">
  <strong>انتخاب زبان / Language / 语言:</strong><br>
  <a href="README.md">🇮🇷 فارسی</a> |
  <a href="README_EN.md">🇬🇧 English</a> |
  <a href="README_ZH.md">🇨🇳 简体中文</a>
</p>

## معرفی راهنما

**از پارامترهای دیتاشیت تا طراحی عملی حفاظت در برابر اضافه‌ولتاژ**

این مخزن به معرفی وریستور، به‌ویژه **وریستور اکسید فلزی (MOV)**، ساختار و سازوکار عملکرد آن و کاربردش در مدارهای حفاظت در برابر اضافه‌ولتاژهای گذرا می‌پردازد. محتوای راهنما برای مهندسان، طراحان الکترونیک، دانشجویان و علاقه‌مندان به طراحی مدار تهیه شده است.

<p align="center">
  <img src="Images/GitHub-Assets/MES-Section-Header.svg" width="90%" alt="سرفصل‌های راهنمای وریستور">
</p>

## سرفصل‌های آموزشی

1. وریستور چیست و چگونه از مدار محافظت می‌کند؟
2. ساختار MOV و سازوکار فیزیکی دانه‌ها و مرزدانه‌های اکسید روی (ZnO)
3. منحنی مشخصه ولتاژ–جریان (V–I) و نواحی عملکرد
4. پارامترهای مهم دیتاشیت و روش تفسیر آن‌ها
5. انواع وریستور و مقایسه MOV با TVS و GDT
6. کاربردها و اصول پیاده‌سازی مدارهای حفاظتی
7. چهار معیار کلیدی انتخاب: ولتاژ کاری پیوسته، ولتاژ کلمپینگ، جریان ضربه‌ای و انرژی
8. مثال عملی انتخاب وریستور برای برق شهر
9. مدل‌های پیشنهادی برای ولتاژهای متداول DC و سیستم سه‌فاز 380 ولت
10. جمع‌بندی، واژه‌نامه و نکات ایمنی

## دریافت مستندات

- 📘 [دانلود راهنمای فارسی وریستور — PDF، نسخه 1.4](./MES-Varistor-Guide-FA%20v1_4.pdf)
- 🖼️ [مشاهده تصاویر و اینفوگرافیک‌های آموزشی](./Images/README.md)
- 🎨 [مشاهده مجموعه فایل‌های گرافیکی MES](./Images/GitHub-Assets/README.md)

> **وضعیت فایل‌ها:** در حال حاضر فایل PDF فارسی در شاخه اصلی مخزن موجود است. نسخه PDF انگلیسی در این شاخه قرار نگرفته است؛ بنابراین برای جلوگیری از ایجاد پیوند خراب، لینک دانلود آن در این README درج نشده است.

## چهار معیار اصلی انتخاب وریستور

| پارامتر | مفهوم و نکته انتخاب |
|---|---|
| **MCOV** — حداکثر ولتاژ کاری پیوسته | باید از بیشینه ولتاژ عادی مدار، با درنظرگرفتن تلرانس و شرایط شبکه، بیشتر باشد. |
| **Clamping Voltage (V₍C₎)** — ولتاژ کلمپینگ | ولتاژ باقی‌مانده روی وریستور هنگام عبور جریان ضربه‌ای است؛ باید با تحمل ولتاژ تجهیز حفاظت‌شونده سازگار باشد. |
| **Peak Surge Current (Iₚₑₐₖ)** — جریان ضربه‌ای بیشینه | باید از جریان ضربه‌ای مورد انتظار در محل نصب و برای شکل موج آزمون مربوط بیشتر باشد. |
| **Energy Rating (J)** — انرژی قابل جذب | باید با انرژی و شکل موج گذرا و تعداد تکرار مورد انتظار سازگار باشد. |

علاوه بر این چهار معیار، ولتاژ وریستور در جریان آزمون مشخص (مانند V₁mA)، ظرفیت خازنی، ابعاد دیسک، دمای محیط، فاصله‌های ایزولاسیون و هماهنگی با فیوز یا قطع‌کن حرارتی نیز باید بررسی شوند.

## نکات مهم طراحی و ایمنی

- وریستور معمولاً به‌صورت **موازی با ورودی یا بار حفاظت‌شونده** قرار می‌گیرد.
- ولتاژ کلمپینگ مقدار ثابتی مستقل از جریان نیست؛ مقدار آن به جریان ضربه‌ای و شکل موج آزمون وابسته است.
- برای مدارهای متصل به برق شهر، هماهنگی وریستور با فیوز یا قطع‌کن حرارتی ضروری است. خرابی وریستور ممکن است به اتصال کوتاه و افزایش دما منجر شود.
- انتخاب قطعه باید بر اساس دیتاشیت دقیق همان سازنده و شماره فنی انجام شود؛ مقایسه اعداد بدون توجه به شکل موج و شرایط آزمون معتبر نیست.
- برای حفاظت در برابر صاعقه و گذراهای پرانرژی، ممکن است به طراحی چندمرحله‌ای و هماهنگی MOV، TVS و GDT نیاز باشد.
- مثال‌ها و مدل‌های معرفی‌شده در راهنما جنبه آموزشی دارند و جایگزین ارزیابی ایمنی، استانداردهای محصول و بررسی دیتاشیت قطعه نهایی نیستند.

## تصاویر و دیاگرام‌های راهنما

تصاویر آموزشی موجود در مخزن فعلاً به زبان فارسی هستند. برای مشاهده پیش‌نمایش‌ها و دریافت فایل‌های اصلی به پوشه تصاویر مراجعه کنید.

<p align="center">
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-00.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-00.jpg" width="30%" alt="معرفی وریستور"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-01.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-01.jpg" width="30%" alt="ساختار و عملکرد"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-02.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-02.jpg" width="30%" alt="پارامترهای دیتاشیت"></a>
</p>
<p align="center">
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-03.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-03.jpg" width="30%" alt="ولتاژ کاری و کلمپینگ"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-04.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-04.jpg" width="30%" alt="جریان ضربه‌ای و انرژی"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-05.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-05.jpg" width="30%" alt="ابعاد و قطر وریستور"></a>
</p>

<p align="center">
  <img src="Images/GitHub-Assets/MES-Divider.svg" width="100%" alt="MES Divider">
</p>

## تهیه و تدوین

**معمار الکترونیک صنعت**  
**MEMAR ELECTRONIC SANAT (MES)**

همراه شما در مسیر طراحی و ساخت مدارهای مطمئن

- کانال تلگرام: [Memar Electronic](https://t.me/Memar_Electronic)
- پیج اینستاگرام: [Memar Electronic](https://www.instagram.com/Memar.Electronic)
- GitHub: [MEMAR-ELECTRONIC-SANAT](https://github.com/MEMAR-ELECTRONIC-SANAT)

<p align="center">
  <img src="Images/GitHub-Assets/MES_Animated_Logo_640x480.svg" width="120" alt="MES Animated Logo">
</p>
