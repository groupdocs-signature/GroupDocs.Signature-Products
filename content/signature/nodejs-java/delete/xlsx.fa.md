



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:42
draft: false
lang: fa
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "حذف امضاها از XLSX با استفاده از JavaScript"
head_description: "حذف امضای دیجیتال، بارکد، متن، تصویر و متاداده از اسناد امضا شده XLSX می‌تواند به راحتی با استفاده از GroupDocs.Signature for Node.js via Java انجام شود."

############################# Header ############################
title: "حذف امضاهای موجود در XLSX بدون زحمت" 
description: "راه‌حل جامع ما فراتر از امضای ساده اسناد است و ویژگی‌های قدرتمندی را در GroupDocs.Signature for Node.js via Java برای شناسایی و حذف انواع مختلف امضاها ارائه می‌دهد."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان خود را دریافت کنید"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "با GroupDocs.Signature for Node.js via Java آشنا شوید"
    link: "/signature/nodejs-java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) یک کتابخانه امضای دیجیتال پیشرفته و درجه یک است که برای پشتیبانی از طیف وسیعی از انواع امضاها طراحی شده است، از جمله متن، تصاویر، بارکدها، گواهی‌های دیجیتال و مهرها. با سازگاری با بیش از 60 فرمت سند، از جمله PDF، فایل‌های MS Office، تصاویر، آرشیوهای ZIP و دیگر فرمت‌های کلیدی کسب و کار، این ابزار قابلیت‌های بی‌نظیری را در جریان‌های کاری اسناد الکترونیکی ارائه می‌دهد. این پلتفرم نه‌تنها امکان افزودن امضا را فراهم می‌کند بلکه قابلیت‌های قابل توجهی برای جستجو، اعتبارسنجی، به‌روزرسانی و حذف امضاها را ارائه می‌دهد و مدیریت کامل چرخه‌های زندگی فرآیندهای امضای دیجیتال را در محیط‌های سازمانی تضمین می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "راهنمایی برای حذف امضاهای دیجیتال از XLSX با استفاده از JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) به توسعه‌دهندگان Node.js via Java اجازه می‌دهد تا به‌طور مؤثر امضاهای الکترونیکی را در فایل‌های XLSX با دنبال کردن مجموعه‌ای از مراحل ساده حذف کنند.
      
      1. مسیر فایل XLSX را به یک نمونه از کلاس Signature ارائه دهید.
      2. از روش Search برای شناسایی تمام امضاها در سند استفاده کنید.
      3. یک یا چند مورد از امضاهای شناسایی شده را حذف کنید.
      4. نتایج پردازش سند را مرور کنید.
   
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

        // مدرکی که دارای امضاها است را به نمونه Signature ارائه دهید
        const signature = new signatureLib.Signature('input.xlsx');

        // همه امضاهای بارکد را پاک کنید
        const options = new signatureLib.DigitalSearchOptions();
        const signatures = signature.search(signatureLib.DigitalSignature.class, options);

        // اولین امضای دیجیتال شناسایی شده را حذف کنید
        if(signatures.size() > 0)
        {
            const digitalSignature = signatures[0];
            const result = signature.delete('output.xlsx', digitalSignature);

            // نتیجه حذف را مدیریت کنید
            if(result)
            {
                console.log(`\n XLSX digital signature deleted successfully`);
            }
        }

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "امنیت اسناد را با ابزارهای امضا افزایش دهید"
  description: "GroupDocs.Signature for Node.js via Java به‌طور خاص برای ساده‌سازی امضا و مدیریت فرمت‌های فایل تجاری طراحی شده است و به شما این امکان را می‌دهد تا به دقت امضاها را اضافه، ویرایش، تأیید یا حذف کنید."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "از قابلیت‌های جامع GroupDocs.Signature مطلع شوید"
  features:
    # feature loop
    - title: "امضای اسناد"
      content: "امضاهای متن، تصویر، بارکد، QR Code یا مهر را به هر صفحه از اسناد پشتیبانی شده اضافه کنید. از متاداده پنهانی مانند EXIF در تصاویر استفاده کنید یا یکپارچگی سند را با گواهی‌های دیجیتال برای جلوگیری از تغییرات غیرمجاز تضمین کنید."

    # feature loop
    - title: "جستجو و اعتبارسنجی امضا"
      content: "ابزارهای ما امکان تأیید دقیق امضای اسناد را فراهم می‌کنند و اصالت آن‌ها را تضمین می‌کنند. جستجوهای جامع برای استرداد همه امضاها در اسناد خود انجام دهید و کنترل بیشتری بر روی آن‌ها داشته باشید."

    # feature loop
    - title: "ویرایش امضاهای موجود"
      content: "امضاهای قبلاً اضافه شده را با تنظیم متن، تغییر موقعیت یا تغییر رنگ‌ها به شکلی که مورد نیاز شماست، به راحتی اصلاح کنید."

    # feature loop
    - title: "حذف امضاهای ناخواسته"
      content: "با قابلیت‌های کامل CRUD، راه‌حل ما حذف مؤثر طیف وسیعی از انواع امضاها از اسناد شما را امکان‌پذیر می‌کند و انعطاف‌پذیری و کنترل را تضمین می‌کند."
      
  code_samples_ext:
    # code sample ext loop
    - title: "حذف همه امضاهای بارکد"
      content: |
        روش حذف همه امضاهای بارکد موجود در یک سند را یاد بگیرید.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // سندی را که شامل امضاهای بارکد است ارائه دهید
          const signature = new signatureLib.Signature('input.xlsx');

          // همه امضاهای بارکد را پاک کنید
          const result = await signature.delete('output.xlsx', signatureLib.SignatureType.Barcode);
          if (result.getSucceeded().size() > 0) {

              // نتیجه حذف را مرور کنید
              console.log('Following XLSX barcode signatures were deleted:');
              let number = 1;
              result.getSucceeded().toArray().forEach((o) => {
                    const temp = o;
                    console.log(`Signature #${number++}: Type: ${temp.getSignatureType()}, 
                    Id: ${temp.getSignatureId()}, Text: ${temp.getText()}`);
              });
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
    title: "ویژگی‌های ما را کشف کنید"
    exclude: "delete"
    description: "مجموعه‌ای کامل از راه‌حل‌ها و عملیات‌های امضا در سیستم ما را بیابید."
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
    title: "حذف امضاها از فرمت‌های مختلف فایل"
    exclude: "XLSX"
    description: "راه‌حل GroupDocs.Signature for Node.js via Java ما در حذف امضاها در یک طیف متنوع از بیش از 60 فرمت فایل ماهر است و سازگاری و عملکرد وسیعی را تضمین می‌کند."
    items: 
          
        # format loop 1
        - name: "حذف امضاهای PDF"
          format: "PDF"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "حذف امضاهای DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/delete/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "حذف امضاهای PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "حذف امضاهای XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---