---
############################# Static ############################
layout: "landing"
date: 2024-09-25T12:45:24
draft: false

lang: fa
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java" 
    # supported_platforms loop
    - title: "Python"
      tag: "python-net" 

############################# Head ############################
head_title: "Node.js Digital Signature API - GroupDocs.Signature"
head_description: "امضاهای الکترونیکی امن را در برنامه های Node.js با GroupDocs.Signature ادغام کنید. گردش کار امضای اسناد را آسان و کارآمد کنید."

############################# Header ############################
title: "اسناد را امضا کنید با Node.js API"
description: "با استفاده از APIهای منعطف و راه حل های مبتنی بر برنامه برای برنامه نویسان و کاربران نهایی، اسناد و تصاویر دیجیتال را روی هر پلتفرمی امضا کنید."
words:
  for: "برای"

actions:
  main: "دانلود از NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "صدور مجوز"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
  title: "برای شروع آماده اید؟"
  description: "ویژگی های GroupDocs.Signature را به صورت رایگان امتحان کنید یا درخواست مجوز کنید"

release:
  title: "نسخه {0} منتشر شد"
  notes: "ببینید چه چیز جدیدی است"
  downloads: "دانلودها"

code:
  title: "امضای PDF توسط Node.js"
  more: "نمونه های بیشتر"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // سند PDF را انتخاب کنید
    let signature = new Signature("sample.pdf");
    
    // متن ارائه دهید
    let options = new TextSignOptions("John Smith");
    
    // تنظیم رنگ
    options.ForeColor = Color.Red;
    
    // سند را امضا کرده و در فایل ذخیره کنید
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "نمای کلی GroupDocs.Signature"
  description: "کتابخانه امضای اسناد که آماده استفاده در برنامه های Node.js است"
  features:
    # feature loop
    - title: "راه حل امضای دیجیتال برای اسناد تجاری با Node.js"
      content: "GroupDocs.Signature for Node.js via Java مجموعه کاملی از گزینه‌های امضای دیجیتال را برای PDF، اسناد Office و تصاویر ارائه می‌دهد. متن، بارکد، تصاویر، گواهی‌های دیجیتال و ابرداده موجود است. پردازش ساده اسناد کارایی را تضمین می کند."

    # feature loop
    - title: "دستکاری پیشرفته اسناد امضا شده"
      content: "GroupDocs.Signature به شما امکان می‌دهد اسناد امضا شده را پردازش کنید. جستجو و اعتبارسنجی امضاها با استفاده از معیارهای مختلف. علاوه بر این، اطلاعات دقیق سند را استخراج کنید یا تصاویر پیش‌نمایش صفحات را ایجاد کنید."

    # feature loop
    - title: "فرمت های خروجی متنوع"
      content: "راه حل ما کنترل گسترده ای بر فرمت خروجی اسناد امضا شده فراهم می کند. امضاها را دقیقاً در هر صفحه قرار دهید و ظاهر آنها را سفارشی کنید. اسناد امضا شده را در قالب های متعدد پشتیبانی شده ذخیره کنید و به صورت اختیاری آنها را با رمز عبور ایمن کنید."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال سکو"
  description: "GroupDocs.Signature for Node.js via Java پردازش اسناد را با سیستم عامل های مختلف انجام می دهد"
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
    GroupDocs.Signature for Node.js via Java [قالبهای فایل محبوب عملیات](https://docs.groupdocs.com/signature/java/supported-document-formats/) را تسهیل می‌کند.
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
  description: "PDF، اسناد آفیس و تصاویر را با امضای دیجیتال امضا کنید"

  items:
    # feature loop
    - icon: "sign"
      title: "امضاهای تجاری"
      content: "از انواع مختلف امضا برای امضای اسناد استفاده کنید. امضاهای دیجیتال را دقیقاً در هر مکان صفحه قرار دهید."

    # feature loop
    - icon: "custom"
      title: "سفارشی کردن ظاهر امضا"
      content: "جنبه های بصری امضاها را با تنظیم رنگ، فونت، حاشیه، چرخش و موارد دیگر برای دستیابی به نتیجه دلخواه خود تنظیم کنید."

    # feature loop
    - icon: "password"
      title: "اسناد محافظت شده با رمز عبور"
      content: "برای بسیاری از قالب‌های سند پشتیبانی شده، برای امنیت بیشتر، از اسناد امضا شده با رمز عبور محافظت کنید."

    # feature loop
    - icon: "protect"
      title: "جلوگیری از تغییرات غیرمجاز"
      content: "از اسناد تجاری مهم امضا شده با گواهی های دیجیتال در برابر تغییرات غیرمجاز محافظت کنید."

    # feature loop
    - icon: "convert"
      title: "فرمت های خروجی مورد نظر"
      content: "اسناد امضا شده را در هر قالب پشتیبانی شده به راحتی دریافت کنید. اسناد MS Word را به آسانی به فرمت PDF تبدیل کنید."

    # feature loop
    - icon: "preview"
      title: "پیش نمایش اسناد"
      content: "صفحات سند جداگانه را به عنوان تصاویر برای نیازهای آینده ذخیره کنید."

    # feature loop
    - icon: "search"
      title: "جستجوی امضا"
      content: "اطلاعات مربوط به امضاهای اضافه شده قبلی در اسناد خود را بازیابی کنید."

    # feature loop
    - icon: "validate"
      title: "اعتبار سنجی سند"
      content: "صحت امضاهای ارائه شده در هر سند را تأیید کنید."

    # feature loop
    - icon: "update"
      title: "مدیریت امضا"
      content: "هر گونه امضایی که در هر صفحه سندی گذاشته شده است را حذف، تغییر مکان یا تغییر دهید."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه کد"
  description: "نمونه‌های گویا عملیات‌های معمولی GroupDocs.Signature for Node.js via Java را نشان می‌دهند"
  items:
    # code sample loop
    - title: "PDF را با کدهای QR علامت گذاری کنید"
      content: |
        [ترکیب بارکد](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) در صفحات سند PDF خاص می‌تواند فرآیندهای تجاری را ساده‌تر کند. این بخش نمونه ای از افزودن کد QR با استفاده از GroupDocs.Signature for Node.js via Java را ارائه می دهد.
        {{< landing/code title="نحوه قرار دادن کد QR در PDF.">}}
        ```javascript {style=abap}
        // سند را برای امضا بارگیری کنید
        let signature = new Signature("file_to_sign.pdf");
        
        // گزینه های کد QR را با متن از پیش تعریف شده ایجاد کنید
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // نوع و موقعیت رمزگذاری کد QR را در صفحه پیکربندی کنید
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // سند را امضا کنید و آن را به عنوان فایل نتیجه ذخیره کنید
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "محافظت از DOCX با امضای دیجیتال"
      content: |
        [محافظت از اسناد خود](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) با امضاهای مبتنی بر گواهی‌های دیجیتال. امضای دیجیتال از اسناد تجاری شما در برابر تغییر محتوا محافظت می کند.
        {{< landing/code title="در اینجا نحوه اطمینان از یکپارچگی سند آمده است.">}}
        ```javascript {style=abap}   
        // سند را برای امضای دیجیتال بارگیری کنید
        let signature = new Signature("file_to_sign.docx");
        
        // گزینه های امضای دیجیتال را مشخص کنید و مسیر فایل گواهی را ارائه دهید
        let options = new DigitalSignOptions("certificate.pfx");

        // رمز عبور گواهی را تنظیم کنید
        options.Password = "1234567890";

        // سند را امضا کرده و در مسیر مورد نظر ذخیره کنید
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
