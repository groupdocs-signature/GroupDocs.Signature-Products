



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:59
draft: false
lang: fa
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "افزودن امضاهای الکترونیکی دیجیتال به فایل PDF با JavaScript"
head_description: "با استفاده از JavaScript بر روی یک فایل PDF امضای دیجیتال قرار دهید و تنها با چند خط کد. از GroupDocs.Signature for Node.js via Java برای امضای فرمت‌های مختلف فایل استفاده کنید."

############################# Header ############################
title: "محافظت از PDF با گواهی‌های دیجیتال" 
description: "امنیت اسناد تجاری خود را با گنجاندن گواهی‌های دیجیتال با استفاده از قابلیت‌های پیشرفته GroupDocs.Signature for Node.js via Java تضمین کنید. ما گزینه‌های انعطاف‌پذیری برای محافظت و تأیید صحت اسناد شما ارائه می‌دهیم."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "رایگان دانلود کنید"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "درباره GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) یک راه‌حل جامع برای امضا است که برای مدیریت نیازهای مختلف پردازش اسناد طراحی شده است. این ابزار به شما امکان می‌دهد متن، تصاویر، گواهی‌های دیجیتال و مهر را به بیش از ۶۰ فرمت مختلف فایل، از جمله PDF، مایکروسافت آفیس، تصاویر و فایل‌های ZIP اضافه کنید. علاوه بر این، اسناد امضا شده را می‌توان به راحتی جستجو، تأیید، ویرایش یا حذف کرد.

############################# Steps ############################
steps:
    enable: true
    title: "راهنما برای ایمن‌سازی PDF با گواهی‌های دیجیتال در JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) این امکان را برای توسعه‌دهندگان Node.js via Java فراهم می‌کند تا اسناد PDF را از تغییرات با استفاده از امضاهای دیجیتال محافظت کنند. برنامه‌های تجاری خود را با قابلیت‌های امنیت داده‌های جامع تقویت کنید.
      
      1. سند PDF را به سازنده کلاس Signature منتقل کنید.
      2. یک گواهی دیجیتال و رمز عبور مربوطه را برای ایمن‌سازی سند اعمال کنید.
      3. در صورت تمایل، نمای بصری از امضای دیجیتال را بر روی صفحات سند اضافه کنید.
      4. سند را امضا کنید تا از هرگونه تغییر در آینده جلوگیری شود.
   
    code:
      platform: "nodejs-java"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "نمونه امضاها"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شد"
      links:
        #  loop
        - title: "نمونه‌های بیشتر"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // از Signature برای اعمال یک امضای دیجیتال بر روی سند استفاده کنید
        const signature = new signatureLib.Signature('input.pdf');

        // گواهی دیجیتال و رمز عبور مورد نیاز را ارائه دهید
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // در صورت لزوم، تنظیمات امضای بصری را پیکربندی کنید
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // سند را با استفاده از گواهی دیجیتال رمزگذاری کنید
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "بهینه‌سازی یا محافظت از محتوای سند با امضاها"
  description: "GroupDocs.Signature for Node.js via Java برای امضای تمامی فرمت‌های اصلی فایل ساخته شده است و به شما این امکان را می‌دهد تا انواع مختلف امضاها را اضافه، تنظیم، تأیید یا حذف کنید."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضاها را به اسناد خود اضافه کنید"
      content: "به راحتی امضاهای متنی، تصویری، بارکد، QR-Code یا مهر را روی هر صفحه از اسناد پشتیبانی شده قرار دهید. همچنین می‌توانید metadata پنهانی مانند EXIF در تصاویر را وارد یا ویرایش کنید. محتوای سند خود را از تغییرات غیرمجاز با گواهی‌های دیجیتال محافظت کنید."

    # feature loop
    - title: "امضاها را پیدا و تأیید کنید"
      content: "پس از امضا، سند شما می‌تواند چندین بار تأیید شود. صحت محتوای امضا شده را تأیید کنید یا جستجوی دقیقی انجام دهید تا لیستی از تمامی امضاهای موجود استخراج کنید."

    # feature loop
    - title: "امضاهای موجود را ویرایش کنید"
      content: "بیشتر انواع امضاها اجازه ویرایش پس از ایجاد را می‌دهند. می‌توانید متن را تغییر دهید، عناصر را جابه‌جا کنید، رنگ‌ها را تنظیم کنید، اندازه‌ها را تغییر دهید و تغییرات دیگر لازم را اعمال کنید."

    # feature loop
    - title: "امضاهای غیرضروری را حذف کنید"
      content: "راه‌حل ما امکان انجام کامل عملیات CRUD برای امضاها را فراهم می‌کند. در صورت نیاز، می‌توانید انواع مختلف امضاها، از جمله گواهی‌های دیجیتال، را از سند خود حذف کنید."
      
  code_samples:
    # code sample loop
    - title: "محافظت از اسناد با امضاهای دیجیتال"
      content: |
        یاد بگیرید چگونه یک سند را با استفاده از امضاهای دیجیتال در برابر تغییرات قفل کنید.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // سندی که نیاز به امضا دارد را ارائه دهید
        const signature = new signatureLib.Signature('input.pdf');

        // از یک گواهی دیجیتال مناسب و رمز عبور آن استفاده کنید
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // هر گونه اطلاعات متنی اضافی را اضافه کنید
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // عناصر بصری مانند تصاویر را برای نمایش امضا اضافه کنید
        options.setImageFilePath('image.png');
        options.setAllPages(true);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        const padding = new signatureLib.Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        
        // سند دیجیتال قفل شده را به محل مشخصی ذخیره کنید
        const result = signature.sign('output.pdf', options);
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "امکانات GroupDocs.Signature را به صورت رایگان امتحان کنید یا درخواست مجوز ارسال کنید"
  items:
    #  loop
    - title: "بارگیری NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "مجوزدهی"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "با عملکردهای اصلی ما آشنا شوید"
    exclude: "digital"
    description: "ما به طور افتخارآمیزی از مجموعه کاملی از گزینه‌های امضا و قابلیت‌ها پشتیبانی می‌کنیم."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "امضا کردن اسناد در فرمت‌های مختلف"
    exclude: "PDF"
    description: "API Node.js via Java از بیش از ۶۰ فرمت پشتیبانی می‌کند و به شما امکان می‌دهد تنوعی از امضاها را در هر صفحه اعمال کرده، امنیت محتوا را با گواهی‌های دیجیتال تأمین کرده و امضاها را به‌طور مؤثر در داخل سند مدیریت کنید."
    items: 
          
        # format loop 1
        - name: "محافظت از PDF"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "محافظت از DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "محافظت از PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "محافظت از XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---