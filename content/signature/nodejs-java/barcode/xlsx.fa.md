



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:07
draft: false
lang: fa
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "تولید بارکد برای XLSX با استفاده از برنامه‌های JavaScript"
head_description: "به‌سرعت یک امضای بارکد را در یک سند XLSX با استفاده از JavaScript و تنها با چند خط کد تولید و جاسازی کنید. GroupDocs.Signature از امضای چندین فرمت فایل پشتیبانی می‌کند."

############################# Header ############################
title: "به سادگی بارکدها را در XLSX تولید و اضافه کنید" 
description: "از GroupDocs.Signature for Node.js via Java برای ادغام بارکدها در سندهای تجاری خود استفاده کنید و آن‌ها را دقیقا در مکان‌های مورد نیاز قرار دهید. راه‌حل ما گزینه‌های سفارشی‌سازی گسترده‌ای را برای تطبیق امضای بارکد با نیازهای شما ارائه می‌دهد."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "هم‌اکنون دانلود کنید – رایگان است!"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "مقدمه‌ای بر GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) یک ابزار قدرتمند برای امضای اسناد است که از انواع مختلف امضا شامل متن، تصویر، بارکد، گواهی دیجیتال و مهر پشتیبانی می‌کند. این ابزار با قابلیت سازگاری با بیش از 60 فرمت فایل، از جمله PDF، فایل‌های MS Office، تصاویر و آرشیوهای ZIP، مدیریت کاملی بر اسناد فراهم می‌آورد. امضاها در داخل اسناد می‌توانند بر اساس نیاز جستجو، تأیید، تغییر یا حذف شوند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه می‌توان بارکدها را در فایل XLSX تولید و جاسازی کرد"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) امکان تولید و قرار دادن بارکدها را در فرمت‌های محبوب مختلف در صفحات XLSX فراهم می‌کند. با پشتیبانی از بیش از 60 نوع بارکد، برنامه‌های Node.js via Java به‌راحتی با ویژگی‌های امضای بارکد تقویت می‌شوند.
      
      1. فایل یا جریان XLSX را برای پردازش ارائه دهید.
      2. متن بارکد را به یک نمونه BarcodeSignOptions منتقل کنید.
      3. تنظیمات بارکد مانند موقعیت، اندازه و غیره را تنظیم کنید.
      4. سند را با بارکد تازه اضافه‌شده ذخیره کنید.
   
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

        // ایجاد یک شیء Signature با مسیر سند
        const signature = new signatureLib.Signature('input.xlsx');

        // استفاده از BarcodeSignOptions برای ادغام یک بارکد در سند
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // تنظیم نوع بارکد و پارامترهای اضافی
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // ذخیره سند امضا شده
        signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "اسناد خود را با گزینه‌های پیشرفته امضا تقویت و ایمن کنید"
  description: "کتابخانه GroupDocs.Signature for Node.js via Java برای تسهیل امضا و مدیریت بعدی فرمت‌های محبوب اسناد طراحی شده است. به‌سرعت و به سادگی می‌توانید امضاهای مختلف را اضافه، ویرایش، تأیید یا حذف کنید."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "عملکردهای کلیدی GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضای پویا اسناد"
      content: "يمكنك إمضاء أي صفحة من مستنداتك باستخدام أطياف مختلطة من الأنواع المختلفة من التوقيع مثل النصوص والصور والباركودات وQR كودات والأختام. بالإضافة إلى ذلك، يمكنك إدراج بيانات تعريف خفية، مثل بيانات EXIF في الصور، أو تأمين المستند ضد التعديلات غير المصرح بها باستخدام الشهادات الرقمية."

    # feature loop
    - title: "تأکید و جستجوی امضاهای قوی"
      content: "راه‌حل ما ابزارهای گسترده‌ای برای مدیریت اسناد امضا شده فراهم می‌آورد. صحت امضاها را برای اطمینان از سلامت سند تأیید کنید و از ویژگی جستجو برای لیست‌کردن تمامی امضاهای جاسازی‌شده در یک سند استفاده کنید."

    # feature loop
    - title: "امضاها را به راحتی ویرایش کنید"
      content: "بیشتر امضاهای قبلاً اضافه‌شده می‌توانند به سادگی ویرایش شوند. متن را به‌روزرسانی کنید، مکان را تغییر دهید یا ظاهر امضا را متناسب با نیازهای خود تغییر دهید."

    # feature loop
    - title: "حذف امضا به‌صورت ساده"
      content: "با پشتیبانی جامع از عملیات CRUD، ابزار ما امکان حذف مؤثر امضاها از اسناد شما را فراهم می‌آورد و اطمینان حاصل می‌کند که تنها امضاهای مرتبط باقی بمانند."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه یک امضای بارکد اعمال کنیم"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان یک بارکد سفارشی را در صفحات سند XLSX جاسازی کرد.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // سند مورد نظر برای امضای آن را ارائه دهید
          const signature = new signatureLib.Signature('input.xlsx');

          // استفاده از BarcodeSignOptions برای ادغام یک بارکد در سند
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // تنظیم نوع بارکد و پارامترهای اضافی
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // حاشیه بارکد از لبه صفحه را تعریف کنید
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // رنگ بار را انتخاب کنید
          signOptions.setForeColor(signatureLib.Color.RED);

          // سبک فونت برای پیام را مشخص کنید
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // موقعیت پیام را تعیین کنید
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // سند را امضا کرده و ذخیره کنید
          signature.sign('output.xlsx', signOptions);

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
            link: "/examples/signature/formats/signature_barcode.xlsx"
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
    title: "به ویژگی‌های اصلی ما نگاهی بیندازید"
    exclude: "barcode"
    description: "از طیف وسیعی از انواع و ابزارهای امضا که ما ارائه می‌دهیم، استفاده کنید."
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
    title: "امضا در چندین فرمت سند"
    exclude: "XLSX"
    description: "API Node.js via Java به شما امکان می‌دهد بیش از 60 فرمت مختلف را امضا کنید. چه بخواهید امضاها را به صفحات خاص اضافه کنید یا آن‌ها را در مکان‌های دقیق قرار دهید، ابزار ما این کار را آسان می‌کند."
    items: 
          
        # format loop 1
        - name: "اضافه کردن بارکد به PDF"
          format: "PDF"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "اضافه کردن بارکد به DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "اضافه کردن بارکد به JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "اضافه کردن بارکد به PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "اضافه کردن بارکد به XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---