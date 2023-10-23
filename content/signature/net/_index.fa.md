---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:09
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: fa
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: "NET، جاوا، APIهای ابری و برنامه‌های امضای سند آنلاین"
head_description: "راه حل امضای الکترونیک سند یکپارچه برای دات نت، جاوا و برنامه های کاربردی مبتنی بر ابر دریافت کنید. با استفاده از قابلیت ساده کشیدن و رها کردن، فرمت های رایج اسناد را به صورت آنلاین امضا کنید"

############################# Header ############################
title: "اسناد را امضا کنید<br>از طریق NET API"
description: "با استفاده از APIهای منعطف و راه حل های مبتنی بر برنامه برای برنامه نویسان و کاربران نهایی، اسناد و تصاویر دیجیتال را روی هر پلتفرمی امضا کنید."
words:
  for: "برای"

actions:
  main: "دانلود رایگان NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "صدور مجوز"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "برای شروع آماده اید؟"
  description: "ویژگی های GroupDocs.Signature را به صورت رایگان امتحان کنید یا درخواست مجوز کنید"

release:
  title: "نسخه {0} منتشر شد"
  notes: "ببینید چه چیز جدیدی است"
  downloads: "دانلودها"

code:
  title: "ثبت فایل های PDF در سی شارپ"
  more: "نمونه های بیشتر"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // سند PDF را انتخاب کنید
    using (Signature signature = new Signature("sample.pdf"))
    {
        // متن ارائه دهید
        var options = new TextSignOptions("John Smith")
        {
            // تنظیم رنگ
            ForeColor = Color.Red
        };
        // سند را امضا کرده و در فایل ذخیره کنید
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "نمای کلی GroupDocs.Signature"
  description: "API برای انجام امضای سند و عملیات مرتبط در برنامه های NET"
  features:
    # feature loop
    - title: "اضافه کردن امضا به اسناد تجاری در سی شارپ"
      content: "امضای اسناد: با GroupDocs.Signature برای دات نت، می توانید انواع مختلفی از امضاها مانند متن، تصاویر، بارکدها و گواهی های دیجیتال را به اسناد PDF و Office اضافه کنید. این API به شما امکان می دهد اسناد خود را با تقریباً هر نوع داده ای از جمله ابرداده پنهان امضا کنید."

    # feature loop
    - title: "پردازش اسناد امضا شده"
      content: "پردازش اضافی: می توانید با استفاده از GroupDocs.Signature عملیات قدرتمندی را روی اسناد امضا شده انجام دهید. این شامل جستجوی امضاهای موجود در اسناد تجاری و تأیید آنها با استفاده از معیارهای خاص است. علاوه بر این، می‌توانید اطلاعات سند و پیش‌نمایش صفحات را از طریق این NET API بازیابی کنید."

    # feature loop
    - title: "سفارشی کردن نتایج"
      content: "GroupDocs.Signature برای دات نت گزینه های سفارشی سازی گسترده ای را ارائه می دهد. شما می توانید امضاها را دقیقاً در هر نقطه از صفحه سند قرار دهید و ظاهر آنها را با استفاده از تنظیمات مختلف تنظیم کنید. علاوه بر این، این API از ذخیره اسناد پردازش شده در طیف گسترده ای از فرمت های پشتیبانی شده پشتیبانی می کند."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال سکو"
  description: "GroupDocs.Signature برای دات نت از سیستم عامل ها، فریم ورک ها و مدیران بسته های زیر پشتیبانی می کند"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت های فایل پشتیبانی شده"
  description: |
    GroupDocs.Signature فرمت های فایل [زیر پشتیبانی می کند](https://docs.groupdocs.com/signature/net/supported-document-formats/) برای دات نت از عملیات با.
  groups:
    # group loop
    - color: "green"
      content: |
        ### فرمت های مایکروسافت آفیس
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### تصاویر و فرمت های دیگر
        * **قابل حمل:** PDF
        * **تصاویر:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **سایر فرمت های اداری:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### فرمت های دیگر
        * **وب:** HTML, MHTML
        * **آرشیوها:** ZIP, TAR, 7Z
        * **گواهینامه ها:** PFX

############################# Features ############################
features:
  enable: true
  title: "ویژگی های GroupDocs.Signature"
  description: "امضای پی دی اف، اسناد آفیس، و تصاویر به سرعت و با دقت"

  items:
    # feature loop
    - icon: "sign"
      title: "امضای سند"
      content: "یک یا چند نوع امضای پشتیبانی شده را با دقت در هر موقعیت مشخصی در اسناد تجاری اضافه کنید."

    # feature loop
    - icon: "custom"
      title: "سفارشی کردن امضاها"
      content: "از ویژگی هایی مانند رنگ، فونت، حاشیه، چرخش و غیره برای پیکربندی ظاهر امضاها استفاده کنید."

    # feature loop
    - icon: "password"
      title: "حفاظت از رمز عبور سند"
      content: "پس از امضا، انواع اسناد خاص را با تنظیم رمز عبور ایمن کنید."

    # feature loop
    - icon: "protect"
      title: "محافظت در برابر تغییرات"
      content: "پس از ضمیمه کردن یک امضا با گواهی دیجیتال، از تغییرات اسناد تجاری مهم جلوگیری کنید."

    # feature loop
    - icon: "convert"
      title: "تبدیل فایل های امضا شده به فرمت های دیگر"
      content: "تبدیل فایل های امضا شده به فرمت های دلخواه، مانند ذخیره یک سند Word به عنوان PDF."

    # feature loop
    - icon: "preview"
      title: "استخراج پیش نمایش صفحه"
      content: "صفحات را از اسناد امضا شده به عنوان تصاویر جداگانه برای پردازش آینده استخراج کنید."

    # feature loop
    - icon: "search"
      title: "جستجوی امضا در اسناد"
      content: "اطلاعات مربوط به امضاهای اضافه شده قبلی در اسناد خاص را بازیابی کنید."

    # feature loop
    - icon: "validate"
      title: "اسناد امضا شده را تأیید کنید"
      content: "با استفاده از ویژگی‌های اعتبارسنجی، امضای صحیح اسناد را تأیید کنید."

    # feature loop
    - icon: "update"
      title: "امضاها را به روز کنید یا حذف کنید"
      content: "امضاهای خاص را به راحتی در یک صفحه تغییر مکان دهید، متن آنها را تغییر دهید یا آنها را بدون هیچ مشکلی حذف کنید."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه کد"
  description: "برخی از موارد معمولی GroupDocs.Signature برای عملیات NET استفاده می کنند"
  items:
    # code sample loop
    - title: "کد QR را به PDF اضافه کنید"
      content: |
        افزودن [QR-codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) به صفحات خاصی از اسناد PDF می‌تواند فرآیندهای تجاری را بهبود بخشد. در زیر مثالی از نحوه افزودن کد QR با استفاده از GroupDocs.Signature آورده شده است.
        {{< landing/code title="نحوه قرار دادن کد QR در PDF.">}}
        ```csharp {style=abap}
        // سند را برای امضا بارگیری کنید
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // گزینه های کد QR را با متن از پیش تعریف شده ایجاد کنید
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // نوع و موقعیت رمزگذاری کد QR را در صفحه پیکربندی کنید
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // سند را امضا کنید و آن را به عنوان فایل نتیجه ذخیره کنید
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "محافظت از یک سند DOCX با استفاده از گواهی دیجیتال"
      content: |
        می‌توانید با استفاده از امضاهای شخصی یا شرکتی که به‌عنوان گواهی‌های دیجیتال ذخیره شده‌اند، [از یک سند محافظت کنید](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/). چنین اسناد محافظت شده را نمی توان بدون باطل کردن امضا تغییر داد.
        {{< landing/code title="در اینجا نحوه اطمینان از یکپارچگی سند آمده است.">}}
        ```csharp {style=abap}   
        // سند را برای امضای دیجیتال بارگیری کنید
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // گزینه های امضای دیجیتال را مشخص کنید و مسیر فایل گواهی را ارائه دهید
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // رمز عبور گواهی را تنظیم کنید
                Password = "1234567890"
            };
            // سند را امضا کرده و در مسیر مورد نظر ذخیره کنید
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
