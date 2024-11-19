



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:07
draft: false
lang: fa
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "ایجاد و افزودن مهرها به JPEG از طریق JavaScript"
head_description: "از قدرت GroupDocs.Signature و JavaScript بهره ببرید تا مهرهای سفارشی را بر روی هر صفحه‌ای از مدارک JPEG خود ایجاد و قرار دهید."

############################# Header ############################
title: "ادغام مهرهای سفارشی در فایل‌های JPEG" 
description: "از GroupDocs.Signature for Node.js via Java برای ایجاد مهرهای اختصاصی و افزودن آن‌ها در هر مکان از مدارک خود بهره ببرید. پلتفرم ما گزینه‌های وسیعی را برای سفارشی‌سازی مهرها بر اساس نیازهای خاص کسب‌وکار شما فراهم می‌کند."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "آزمون رایگان"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java چیست؟"
    link: "/signature/nodejs-java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) یک راه‌حل قوی و چندمنظوره برای امضای مدارک فراهم می‌کند. این ابزار به کاربران امکان می‌دهد تا با استفاده از بیش از 60 فرمت مختلف، شامل PDF، Word، Excel، فایل‌های تصویری و فایل‌های ZIP، مهرها و سایر نوع‌های امضا را اضافه کنند. پلتفرم به شما اجازه می‌دهد تا متن، تصویر، بارکد، کد QR، متادیتا، گواهی‌های دیجیتال و امضاهای مهر را وارد کنید. علاوه بر امضا، می‌توانید هر امضای موجود در مدارک خود را جستجو، تأیید، ویرایش یا حذف کنید.

############################# Steps ############################
steps:
    enable: true
    title: "راهنمای افزودن مهرها به JPEG با استفاده از JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) ابزاری قدرتمند برای ایجاد و افزودن مهرها به مدارک فراهم می‌کند که می‌تواند برنامه‌های Node.js via Java را به طور قابل توجهی بهبود بخشد. از این ویژگی برای طراحی و اعمال مهرهای سفارشی بر روی صفحات مدارک خود استفاده کنید.
      
      1. مدرکی از نوع JPEG که نیاز به مهر دارد را وارد کنید.
      2. از StampSignOptions برای تعریف تمام پارامترهای ضروری استفاده کنید.
      3. به تعداد مورد نیاز خطوط مهر را وارد کنید.
      4. مهر را اعمال کرده و سند نهایی را ذخیره کنید.
   
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

        // مسیر سند را با نمونه Signature مرتبط کنید
        const signature = new signatureLib.Signature('input.jpeg');

        // ایجاد StampSignOptions با محتوای امضای ضروری
        const options = new signatureLib.StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // یک یا چند خط مهر را درج کنید
        const outerLine = new signatureLib.StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(signatureLib.Color.WHITE);
        outerLine.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine);

        // سند را با مهر اعمال شده ذخیره کنید
        const result = signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "تقویت امنیت مدارک با امضاها"
  description: "با کمک GroupDocs.Signature for Node.js via Java می‌توانید مهرها و سایر نوع‌های امضا را در تمام فرمت‌های مدارک محبوب اضافه، ویرایش، تأیید یا حذف کنید. API این پلتفرم فرآیند مدیریت امضاها را ساده‌سازی می‌کند تا یکپارچگی و سفارشی‌سازی مدارک بهبود یابد."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "ویژگی‌های GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضای سفارشی مدارک"
      content: "امضاهایی مانند متن، تصویر، بارکد، کد QR و مهر را به هر قسمت از مدارک خود اعمال کنید. این ابزار همچنین اجازه می‌دهد تا متادیتای پنهان و گواهی‌های دیجیتال برای محافظت بیشتر محتوای شما از تغییرات غیرمجاز اضافه شود."

    # feature loop
    - title: "جستجو و تأیید امضا"
      content: "بعد از امضای یک سند، از سیستم تأیید ما برای اطمینان از یکپارچگی امضاها استفاده کنید. علاوه بر این، پلتفرم ما این امکان را به شما می‌دهد تا با جستجو، اطلاعات دقیقی درباره تمام امضاهای اعمال شده بر روی یک سند را بازیابی کنید."

    # feature loop
    - title: "ویرایش امضاها به نیاز"
      content: "امضاهای قبلاً اعمال شده را بر اساس نیازتان تنظیم و به‌روزرسانی کنید. چه بخواهید محتوا، رنگ، اندازه یا موقعیت امضا را تغییر دهید، GroupDocs.Signature for Node.js via Java گزینه‌های کامل سفارشی‌سازی را ارائه می‌دهد."

    # feature loop
    - title: "حذف امضاهای غیرضروری"
      content: "به راحتی هر امضای غیرضروری را از مدارک خود حذف کنید. API ما از حذف طیف وسیعی از نوع‌های امضا، از جمله مهرها و گواهی‌های دیجیتال، پشتیبانی می‌کند و به شما انعطاف‌پذیری کامل برای مدیریت مدارکتان را می‌دهد."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ادغام مهرهای سفارشی در مدارک"
      content: |
        یاد بگیرید که چگونه مهرهای سفارشی با متن‌های ضروری را برای مدارک خود طراحی و اعمال کنید.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // مدرک را برای مهر زدن فراهم کنید
          const signature = new signatureLib.Signature('input.jpeg');

          // گزینه‌های مهر را با پیکربندی‌های مورد نظر تنظیم کنید
          const options = new signatureLib.StampSignOptions();

          // ابعاد و موقعیت مهر را بر روی صفحه مشخص کنید
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setAllPages(true);

          // خطوط دایره‌ای بیرونی با متن سفارشی اضافه کنید
          const outerLine1 = new signatureLib.StampLine();
          outerLine1.setText('* The best  choice *');
          outerLine1.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
          const signatureFont1 = new signatureLib.SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName('Arial');
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(signatureLib.Color.WHITE);
          outerLine1.setBackgroundColor(signatureLib.Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // خطوط داخلی مربع را در صورت نیاز اضافه کنید
          const innerLine1 = new signatureLib.StampLine();
          innerLine1.setText('Company #1');
          innerLine1.setTextColor(signatureLib.Color.RED);
          const signFont1 = new signatureLib.SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);
          
          // مدرک مهرخورده را ذخیره کنید
          const result = signature.sign('output.jpeg', options);
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "ویژگی‌های کلیدی را کاوش کنید"
    exclude: "stamp"
    description: "راه‌حل ما مجموعه‌ای از ابزارها را برای ایجاد، مدیریت، و حذف انواع مختلف امضاها ارائه می‌دهد و کنترل کامل بر روی گردش کار مدارک را به کاربران می‌دهد."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
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
    title: "اعمال امضای مهر بر روی انواع مختلف فایل"
    exclude: "JPEG"
    description: "API GroupDocs.Signature از امضای مهر در بیش از 60 فرمت فایل پشتیبانی می‌کند و به کاربران اجازه می‌دهد تا مهرهای سفارشی را بر روی هر صفحه یا منطقه‌ای قرار دهند و دسترسی و امنیت مدارک را بهبود ببخشند."
    items: 
          
        # format loop 1
        - name: "مهر زدن PDF"
          format: "PDF"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "مهر زدن DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "مهر زدن JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "مهر زدن PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "مهر زدن XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---