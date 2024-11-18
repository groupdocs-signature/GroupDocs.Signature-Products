



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:11
draft: false
lang: fa
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "امضای فایل XLSX با امضاهای الکترونیکی در JavaScript"
head_description: "از قابلیت‌های API JavaScript برای امضای دیجیتال و حفاظت از فایل‌های XLSX، از جمله PDF، مستندات ورد، صفحه‌های اکسل، ارائه‌ها و فرمت‌های تصویری بهره ببرید."

############################# Header ############################
title: "امضای الکترونیکی فایل‌های XLSX" 
description: "از GroupDocs.Signature for Node.js via Java برای درج امضاهای دیجیتال متنوع در اسناد خود استفاده کنید تا یکپارچگی داده‌ها و انطباق برای فایل‌هایی مانند PDF، ورد، اکسل، ارائه‌ها و فرمت‌های تصویری را تضمین کنید."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "حالاً دانلود کنید"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "بررسی اجمالی API GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) مجموعه‌ای قوی از ابزارها را برای افزودن امضاهای الکترونیکی ارائه می‌دهد. با API شهودی آن، می‌توانید به راحتی امضا کنید، جستجو کنید، تأیید کنید، تغییر دهید و امضاها را از انواع فایل‌های مختلف بدون نیاز به نرم‌افزار خارجی حذف کنید. این API امکان امضای آسان PDFها، مستندات ورد، صفحه‌های اکسل، اسلایدهای پاورپوینت و بسیاری از فرمت‌های تصویری را فراهم می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل امضای XLSX با استفاده از JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) روند افزودن امضاهای سفارشی به فایل‌های XLSX را تسهیل می‌کند. توسعه‌دهندگان Node.js via Java می‌توانند به راحتی قابلیت امضا را به برنامه‌های خود اضافه کنند.
      
      1. سند XLSX را به نمونه Signature بارگذاری کنید.
      2. تنظیمات SignOptions را برای تعریف ویژگی‌های امضا پیکربندی کنید.
      3. خواص مانند اندازه، رنگ و محتوا را به دلخواه تنظیم کنید.
      4. سند امضا شده را در مکان مشخص شده ذخیره کنید.
   
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

        // سند را به یک نمونه Signature وارد کنید.
        const signature = new signatureLib.Signature('input.xlsx');

        // یک شی QrCodeSignOptions را ایجاد کنید.
        const options = new signatureLib.QrCodeSignOptions('QR code text');
        
        // همه گزینه‌های مورد نیاز را تعیین کنید.
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(new Color(255, 0, 0));

        // سند امضا شده را در دیسک محلی ذخیره کنید.
        signature.sign('output.xlsx', options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "قابلیت‌های پیشرفته امضای دیجیتال"
  description: "API پیشرفته ما عملیات تجاری را با تسهیل امضا، تأیید، تغییر و مدیریت امضاهای الکترونیکی برای طیف وسیعی از اسناد ساده‌تر می‌کند."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "ویژگی‌های امضای دیجیتال"
  features:
    # feature loop
    - title: "امضای دیجیتال برای فایل‌های اداری"
      content: "امضاهای دیجیتال را به راحتی به هر صفحه یا موقعیتی در یک سند اضافه کنید. امضاهای خود را با گزینه‌هایی مانند گواهینامه‌های دیجیتال، متاداده، بارکدها یا عناصر بصری سفارشی کنید تا امنیت و یکپارچگی سند را تقویت کنید."

    # feature loop
    - title: "کنترل جامع امضا"
      content: "پس از امضای یک سند، می‌توانید امضاهای آن را به راحتی مدیریت کنید. فهرست کاملی از تمام امضاها را بازیابی کنید، تا به‌روزرسانی‌ها یا حذف‌های لازم را انجام دهید."

    # feature loop
    - title: "تقویت امنیت سند"
      content: "از گواهینامه‌های دیجیتال برای محافظت از اسناد خود در برابر تغییرات ناخواسته استفاده کنید. می‌توانید متاداده را جاسازی یا استخراج کنید تا قابلیت ردیابی و ممیزی را افزایش دهید و اطمینان حاصل کنید که اسناد تطابق و اعتبار دارند."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه یک امضای تصویری به یک سند اضافه کنیم"
      content: |
        این راهنما روند افزودن یک امضای تصویری به صفحه مشخصی در یک سند را تشریح می‌کند.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
        
          // مدرک منبع را به عنوان یک پارامتر ورودی ارائه دهید.
          const signature = new signatureLib.Signature('input.xlsx');

          // مسیر فایل تصویر را در گزینه‌های پیکربندی امضا مشخص کنید.
          const options = new signatureLib.ImageSignOptions('image.jpg');

          // ابعاد را پیکربندی کرده و صفحات هدف برای امضا را مشخص کنید.
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          options.setMargin(new signatureLib.Padding(50));
          options.setAllPages(true);

          // عملیات اعمال امضا را به سند پیاده‌سازی کنید.
          signature.sign('output.xlsx', options);

          ```
        platform: "nodejs-java"
        copy_title: "کپی"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "برای کپی کلیک کنید"
          copy_done: "کپی شد"
        top_links:
          #  loop
          - title: "دانلود نتیجه"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.xlsx"
        links:
          #  loop
          - title: "نمونه‌های بیشتر"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


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
    title: "نگاهی به قابلیت‌های گسترده ما"
    exclude: "esign"
    description: "ما مجموعه وسیعی از انواع امضا و عملیات با ویژگی‌های غنی ارائه می‌دهیم."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "امضا زدن به انواع فایل‌ها به صورت دیجیتال"
    exclude: "XLSX"
    description: "API Node.js via Java به شما این امکان را می‌دهد که امضاهای دیجیتال را به بیش از 60 نوع فایل اعمال کنید و به شما انعطاف‌پذیری گسترده‌ای در ایمن‌سازی اسناد حیاتی کسب و کارتان ارائه می‌دهد."
    items: 
          
        # format loop 1
        - name: "امضای الکترونیکی PDF"
          format: "PDF"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "امضای الکترونیکی DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/esign/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "امضای الکترونیکی JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "امضای الکترونیکی PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "امضای الکترونیکی XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---