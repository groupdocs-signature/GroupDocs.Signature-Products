



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: fa
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "تولید کدهای QR در اسناد XLSX با JavaScript"
head_description: "از API GroupDocs.Signature برای ایجاد و ادغام بارکدهای دو بعدی در فایل‌های XLSX استفاده کنید. به راحتی کدهای QR را در هر صفحه از سند قرار دهید."

############################# Header ############################
title: "ساخت کدهای QR برای XLSX" 
description: "با استفاده از GroupDocs.Signature for Node.js via Java، بارکدهای دو بعدی با محتوای قابل سفارشی‌سازی، از جمله متن و داده‌های عددی، را در انواع مختلف اسناد مانند PDF، Word، Excel و تصاویر ایجاد و درج کنید."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "به صورت رایگان امتحان کنید"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "فرصت‌های GroupDocs.Signature for Node.js via Java را بررسی کنید"
    link: "/signature/nodejs-java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) ابزارهای پیشرفته بهبود اسناد را ارائه می‌دهد که امکان تولید و درج انواع مختلف امضا، از جمله کدهای QR، را در فرمت‌های رایج فایل‌ فراهم می‌کند. PDFها، مستندات Word، صفحات گسترده Excel، ارائه‌های PowerPoint و تصاویر را با امضاهای متنی، تصویری، بارکدی، کد QR، متاداده، دیجیتال و مهر امضا کنید و ایمن کنید.

############################# Steps ############################
steps:
    enable: true
    title: "راهنمای تولید و درج یک کد QR در هر نقطه از XLSX"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) امکان تولید کدهای QR در فرمت‌های رایج مختلف و ادغام آنها به صفحات XLSX را فراهم می‌کند. با پشتیبانی از بیش از 10 نوع مختلف کد QR، راه حل ما به‌راحتی می‌تواند در برنامه‌های Node.js via Java گنجانده شود و به آنها قابلیت‌های امضای کد QR را اضافه کند.
      
      1. فایل یا جریان XLSX را برای امضای کد QR ارائه دهید.
      2. متن دلخواه را به نمونه QrCodeSignOptions وارد کنید.
      3. تنظیمات بصری مانند رنگ، موقعیت، اندازه و غیره را تنظیم کنید.
      4. سند حاوی کد QR را ذخیره کنید.
   
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

        // یک نمونه Signature ایجاد کرده و مسیر سند را پاس دهید
        const signature = new signatureLib.Signature('input.xlsx');

        // از QrCodeSignOptions برای درج یک کد QR به سند استفاده کنید
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // نوع امضا و محل قرارگیری آن در صفحه را تعیین کنید
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // سند را با کد QR تازه اضافه شده ذخیره کنید
        signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "یکپارچه‌سازی جامع امضا و کد QR"
  description: "با API GroupDocs.Signature for Node.js via Java می‌توانید زنجیره کاملی از امضاها را مدیریت کنید. امضاها را به راحتی تولید، سفارشی‌سازی، تأیید، جستجو و حذف کنید و انعطاف‌پذیری بی‌نظیری به گردش کارهای خود ارائه دهید."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "ویژگی‌های امضا و کد QR"
  features:
    # feature loop
    - title: "امضای سند چندفرمت"
      content: "انواع مختلفی از امضاها، از جمله امضاهای متنی، تصویری، بارکدی، کد QR و مهر را به هر فرمت سند پشتیبانی شده اضافه کنید. آنها را در هر صفحه قرار دهید و متاداده سند را مدیریت کنید. امنیت سند را از طریق گواهی‌های دیجیتال برای جلوگیری از تغییرات غیرمجاز تأمین کنید."

    # feature loop
    - title: "تأیید امضاها به طور مؤثر"
      content: "تمام امضاها در یک سند را بررسی کنید تا مطمئن شوید که استانداردهای مورد نیاز را رعایت می‌کنند. به راحتی امضاها را از طریق قابلیت جستجوی داخلی بازیابی و مرور کنید."

    # feature loop
    - title: "ویرایش امضاهای انعطاف‌پذیر"
      content: "امضاهای موجود را به‌روزرسانی یا تغییر دهید و جنبه‌هایی از قبیل محتوا، مکان، اندازه و رنگ را تنظیم کنید تا با نیازهای سند شما پس از امضای اولیه مطابقت داشته باشد."

    # feature loop
    - title: "حذف امضا به راحتی"
      content: "هرگونه امضای ناخواسته یا غیرضروری، از جمله گواهی‌های دیجیتال را به سادگی حذف کنید. کنترل کامل بر مدیریت امضاها تضمین می‌کند که سندی پاک و مرتب داشته باشید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "سفارشی‌سازی یک کد QR تولید شده"
      content: |
        این نمونه جزئیات فرآیند افزودن یک کد QR سفارشی به یک صفحه XLSX را توضیح می‌دهد.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // سند برای امضا را به‌دست آورده و به Signature پاس دهید
          const signature = new signatureLib.Signature('input.xlsx');

          // تنظیمات کد QR را با متن مورد نیاز تنظیم کنید
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // محل کد QR را در صفحه تعیین کنید
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // فاصله امضا را مشخص کنید
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // رنگ کد QR را انتخاب کنید
          signOptions.setForeColor(signatureLib.Color.RED);

          // گزینه‌های فونت برای پیام همراه را تعریف کنید
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // رنگ پس‌زمینه و قلم برای کد QR را سفارشی‌سازی کنید
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // کد QR را به سند وارد کنید
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
            link: "/examples/signature/formats/signature_qrcode.xlsx"
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
    title: "درک قابلیت‌های اصلی ما"
    exclude: "qrcode"
    description: "ما انتخاب گسترده‌ای از فرمت‌های امضا و عملیات متناسب با نیازهای شما ارائه می‌دهیم."
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
    title: "ادغام کدهای QR با فرمت‌های مختلف فایل"
    exclude: "XLSX"
    description: "از API Node.js via Java برای تولید کدهای QR و قرارگیری آنها در فرمت‌های رایج استفاده کنید. داده‌های مهم را در این بارکدها محصور کنید تا یکپارچگی بدون درز و بازیابی آینده را تأمین کنید."
    items: 
          
        # format loop 1
        - name: "QR-Code برای PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "QR-Code برای DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "QR-Code برای JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "QR-Code برای PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "QR-Code برای XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---