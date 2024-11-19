



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:33
draft: false
lang: fa
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "جستجو برای امضاهای الکترونیکی در فایل‌های PPTX با JavaScript"
head_description: "قدرت API GroupDocs.Signature for Node.js via Java را برای شناسایی و جستجوی امضاهای الکترونیکی در فایل‌های PDF، مستندات ورد، صفحات اکسل، ارائه‌ها و تصاویر به کار بگیرید."

############################# Header ############################
title: "جستجو برای امضاهای الکترونیکی در PPTX" 
description: "اطلاعات دقیق درباره‌ی تمام امضاهای جاسازی‌شده در فایل‌های PDF، ورد، اکسل، ارائه‌ها و تصاویر را با استفاده از ابزارهای پیشرفتهی ارائه‌شده توسط GroupDocs.Signature for Node.js via Java کشف و بازیابی کنید."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "شروع به‌صورت رایگان"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "مروری بر GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) یک چارچوب قدرتمند برای مدیریت امضاهای دیجیتال در مجموعه‌ای وسیع از انواع فایل‌ها ارائه می‌دهد. با پشتیبانی از بیش از 60 فرمت از جمله PDF، مستندات Microsoft Office، تصاویر و فایل‌های ZIP، این API به کاربران این امکان را می‌دهد که انواع مختلف امضاها از جمله متن، تصویر، بارکد، گواهی‌های دیجیتال و غیره را اعمال، شناسایی، تأیید، به‌روزرسانی یا حذف کنند.

############################# Steps ############################
steps:
    enable: true
    title: "راهنمای جستجوی امضاها در PPTX با استفاده از JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) یک ابزار قدرتمند برای شناسایی امضاهای دیجیتالی در فایل‌های PPTX ارائه می‌دهد. توسعه‌دهندگان Node.js via Java می‌توانند به راحتی عملکرد برنامه خود را با راه‌حل ما گسترش دهند.
      
      1. مسیر فایل PPTX را برای جستجوی امضا مشخص کنید.
      2. از SearchOptions برای فیلتر کردن نتایج جستجو استفاده کنید.
      3. متد Search را برای پیدا کردن امضاها اجرا کنید.
      4. فهرست امضاهای کشف‌شده را بررسی کنید.
   
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

        // یک شیء Signature را با استفاده از مسیر مستند ایجاد کنید
        const signature = new signatureLib.Signature('input.pptx');

        // پیکربندی TextSearchOptions برای شامل کردن هر صفحه
        const options = new signatureLib.TextSearchOptions();
        options.setAllPages(true);

        // جستجو برای شناسایی تمام امضاهای متنی درون مستند را انجام دهید
        const signatures = signature.search(signatureLib.TextSignature.class, options).toArray();
        console.log(`\nSource document contains the following text signature(s).`);

        // امضاهای کشف‌شده را برای تحلیل جامع جمع‌آوری کنید
        for (const textSignature of signatures) {
            console.log(`Found Text signature at page ${textSignature.getPageNumber()} 
            with type [${textSignature.getSignatureImplementation()}] and text '${textSignature.getText()}'.`);
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "راه‌حل کامل مدیریت امضا"
  description: "GroupDocs.Signature for Node.js via Java یک راه‌حل کامل برای افزودن، ویرایش، جستجو و تأیید امضاهای الکترونیکی در فرمت‌های مستندات محبوب ارائه می‌دهد. با ویژگی‌های پیشرفته امضای مستندات، فرآیندهای کاری خود را تجهیز کنید."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "ویژگی‌های شناسایی امضا"
  features:
    # feature loop
    - title: "امضای دیجیتالی فایل‌های تجاری"
      content: "امضاهای الکترونیکی مانند متن، تصویر، بارکد و گواهی‌های دیجیتال را به هر مکانی در مستندات خود اضافه کنید. GroupDocs.Signature از امضای اسناد PDF، ورد، اکسل، تصاویر و غیره پشتیبانی می‌کند و مدیریت مستندات را منعطف می‌سازد."

    # feature loop
    - title: "مدیریت کارآمد امضاها"
      content: "پس از امضا کردن، به راحتی می‌توانید تمام امضاهای جاسازی‌شده در یک مستند را شناسایی کنید. این API امکان جستجو و بازیابی جامع امضاها و همچنین به‌روزرسانی یا حذف آن‌ها را فراهم می‌کند."

    # feature loop
    - title: "امنیت مستندات و مدیریت متا دیتا"
      content: "با جاسازی یا حذف متا دیتاهای پنهان، صحت مستندات خود را تأمین کنید. با استفاده از گواهی‌های دیجیتال، فایل‌های خود را از تغییرات غیرمجاز محافظت کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "شناسایی امضاهای تصویری"
      content: |
        این مثال توضیح می‌دهد که چگونه یک امضای تصویری را در یک مستند خاص شناسایی کنید.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // مستند منبع را به عنوان پارامتر به سازنده ارسال کنید
          const signature = new signatureLib.Signature('input.pptx');

          // برای پیدا کردن هر امضا، جستجو برای امضاهای از نوع متن انجام دهید
          const signatures = signature.search(signatureLib.ImageSignature.class, signatureLib.SignatureType.Image).toArray();
          console.log(`\nSource document contains the following image signature(s).`);

          // یافته‌ها را با خواص جامع امضاهای شناسایی شده نمایش دهید
          for (const imageSignature of signatures) {
              console.log(`Found Image signature at page ${imageSignature.getPageNumber()} 
              and size ${imageSignature.getSize()}.`);
          }
          ```
        platform: "nodejs-java"
        copy_title: "کپی"
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
    title: "عملکردهای کلیدی"
    exclude: "search"
    description: "API جامع ما مجموعه‌ای از عملیات را برای ساده‌سازی مدیریت امضاهای مستندات، از امضا کردن تا پردازش و تأیید پس از آن ارائه می‌دهد."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/nodejs-java/text/pptx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/nodejs-java/image/pptx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/nodejs-java/search/pptx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pptx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "شناسایی امضاها در انواع مختلف فایل‌ها"
    exclude: "PPTX"
    description: "با API GroupDocs.Signature for Node.js via Java، می‌توانید به طور مؤثر امضاهای الکترونیکی را از مجموعه‌ای گسترده از فرمت‌های فایل پشتیبانی شده جستجو و بازیابی کنید تا ادغام بی‌دردسری در فرآیندهای مستندات خود داشته باشید."
    items: 
          
        # format loop 1
        - name: "جستجوی امضاها در PDF"
          format: "PDF"
          link: "/signature/nodejs-java/search/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "یافتن امضاها در DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/search/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "یافتن امضاها در PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/search/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "جستجوی امضاها در XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---