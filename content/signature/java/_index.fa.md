---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:08
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
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "NET، جاوا، APIهای ابری و برنامه‌های امضای سند آنلاین"
head_description: "راه حل امضای الکترونیک سند یکپارچه برای دات نت، جاوا و برنامه های کاربردی مبتنی بر ابر دریافت کنید. با استفاده از قابلیت ساده کشیدن و رها کردن، فرمت های رایج اسناد را به صورت آنلاین امضا کنید"

############################# Header ############################
title: "اسناد را امضا کنید<br>از طریق Java API"
description: "با استفاده از APIهای منعطف و راه حل های مبتنی بر برنامه برای برنامه نویسان و کاربران نهایی، اسناد و تصاویر دیجیتال را روی هر پلتفرمی امضا کنید."
words:
  for: "برای"

actions:
  main: "دانلود رایگان Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "صدور مجوز"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "برای شروع آماده اید؟"
  description: "ویژگی های GroupDocs.Signature را به صورت رایگان امتحان کنید یا درخواست مجوز کنید"

release:
  title: "نسخه {0} منتشر شد"
  notes: "ببینید چه چیز جدیدی است"
  downloads: "دانلودها"

code:
  title: "فایل های PDF را در جاوا امضا کنید"
  more: "نمونه های بیشتر"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // سند PDF را انتخاب کنید
    Signature signature = new Signature("sample.pdf");
    
    // متن ارائه دهید
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // سند را امضا کرده و در فایل ذخیره کنید
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "نمای کلی GroupDocs.Signature"
  description: "API برای انجام امضای سند و عملیات مرتبط در برنامه های جاوا"
  features:
    # feature loop
    - title: "اسناد تجاری بهبود یافته با امضای دیجیتال در جاوا"
      content: "امضای سریع و قابل تنظیم: GroupDocs.Signature برای جاوا طیف گسترده ای از گزینه های امضای دیجیتال را برای فایل های PDF، تصاویر و اسناد آفیس ارائه می دهد. می‌توانید از متن، بارکد، کدهای QR، گواهی‌های دیجیتال، تصاویر یا ابرداده‌های پنهان استفاده کنید. پردازش اسناد سریع و کارآمد است."

    # feature loop
    - title: "دستکاری اسناد امضا شده"
      content: "پردازش سند پیشرفته شامل عملیات قدرتمندی بر روی اسناد امضا شده با استفاده از GroupDocs.Signature برای جاوا است. می توانید امضاهایی را که به اسناد تجاری اضافه شده اند با استفاده از معیارهای مفید مختلف جستجو و تأیید کنید. علاوه بر این، می‌توانید به اطلاعات دقیق درباره سند دسترسی داشته باشید یا تصاویر پیش‌نمایش صفحات آن را دریافت کنید."

    # feature loop
    - title: "تنوع انتخاب های خروجی"
      content: "گزینه های امضای قوی به شما امکان می دهد خروجی را برای اسناد امضا شده با GroupDocs.Signature برای جاوا سفارشی کنید. شما می توانید دقیقاً هر امضا را در هر صفحه سند قرار دهید و ظاهر آن را به روش های مختلف پیکربندی کنید. Java API از ذخیره اسناد تجاری امضا شده در قالب های متعدد پشتیبانی شده پشتیبانی می کند و گزینه هایی را برای ایمن سازی آنها با رمزهای عبور ارائه می دهد."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال سکو"
  description: "GroupDocs.Signature برای جاوا از سیستم عامل ها، چارچوب ها و مدیران بسته های زیر پشتیبانی می کند"
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت های فایل پشتیبانی شده"
  description: |
    GroupDocs.Signature قالب‌های فایل [زیر پشتیبانی می‌کند](https://docs.groupdocs.com/signature/java/supported-document-formats/) برای جاوا از عملیات با.
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
  description: "امضای PDF، اسناد اداری و تصاویر با امضای دیجیتال"

  items:
    # feature loop
    - icon: "sign"
      title: "اضافه کردن امضاها"
      content: "با قرار دادن یک امضای دیجیتال دقیقاً در هر موقعیتی در هر صفحه، یک سند را با استفاده از انواع مختلف امضای پشتیبانی شده امضا کنید."

    # feature loop
    - icon: "custom"
      title: "سفارشی کردن نتایج"
      content: "برای دستیابی به نتیجه دلخواه، ظاهر امضا را با تنظیم رنگ، فونت، حاشیه، چرخش و سایر ویژگی‌ها سفارشی کنید."

    # feature loop
    - icon: "password"
      title: "ایمن سازی اسناد با رمز عبور"
      content: "برای بسیاری از انواع سند پشتیبانی شده، می توانید سند امضا شده را با رمز عبور محافظت کنید."

    # feature loop
    - icon: "protect"
      title: "جلوگیری از تغییرات غیرمجاز"
      content: "از اسناد تجاری مهم امضا شده با گواهی دیجیتال در برابر تغییرات غیرمجاز محافظت کنید."

    # feature loop
    - icon: "convert"
      title: "به دست آوردن نتایج در فرمت های دلخواه"
      content: "به راحتی فایل های نتیجه امضا شده را در هر قالب پشتیبانی شده به دست آورید. همچنین می توانید اسناد MS Word را بدون زحمت به PDF تبدیل کنید."

    # feature loop
    - icon: "preview"
      title: "پیش نمایش سند"
      content: "هر صفحه از یک سند را به عنوان تصویر برای پردازش بعدی ذخیره کنید."

    # feature loop
    - icon: "search"
      title: "جستجو برای امضا"
      content: "امکان دریافت اطلاعات در مورد امضاهای اضافه شده قبلی در اسناد خاص وجود دارد."

    # feature loop
    - icon: "validate"
      title: "تایید مدارک"
      content: "صحت امضاها را در هر سند امضا شده تأیید کنید."

    # feature loop
    - icon: "update"
      title: "مدیریت امضاها"
      content: "هنگامی که یک امضا در صفحه سند قرار می گیرد، می توان آن را در صورت نیاز حذف، منتقل یا به روز کرد."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه کد"
  description: "برخی از موارد معمولی GroupDocs.Signature برای عملیات جاوا استفاده می کنند"
  items:
    # code sample loop
    - title: "سند PDF را با کد QR بهبود بخشید"
      content: |
        بهبود فرآیندهای تجاری با افزودن [QR-codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) به صفحات خاصی از اسناد PDF می تواند ارزشمند باشد. مثالی از نحوه افزودن کد QR با استفاده از GroupDocs.Signature برای جاوا وجود دارد.
        {{< landing/code title="سند PDF را با کد QR بهبود بخشید">}}
        ```java {style=abap}
        // سند را برای امضا بارگیری کنید
        Signature signature = new Signature("file_to_sign.pdf");
        
        // گزینه های کد QR را با متن از پیش تعریف شده ایجاد کنید
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // نوع و موقعیت رمزگذاری کد QR را در صفحه پیکربندی کنید
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // سند را امضا کنید و آن را به عنوان فایل نتیجه ذخیره کنید
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "از امضای دیجیتال برای محافظت از DOCX استفاده کنید"
      content: |
        می‌توانید با استفاده از امضاهای شخصی یا شرکتی که به‌عنوان گواهی‌های دیجیتال ذخیره شده‌اند، [از یک سند محافظت کنید](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/). اسناد ایمن شده با گواهی را نمی توان بدون باطل کردن امضا تغییر داد.
        {{< landing/code title="از امضای دیجیتال برای محافظت از DOCX استفاده کنید">}}
        ```java {style=abap}   
        // سند را برای امضای دیجیتال بارگیری کنید
        Signature signature = new Signature("file_to_sign.pdf");
        
        // گزینه های امضای دیجیتال را مشخص کنید و مسیر فایل گواهی را ارائه دهید
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // رمز عبور گواهی را تنظیم کنید
        options.setPassword("1234567890");

        // سند را امضا کرده و در مسیر مورد نظر ذخیره کنید
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
