



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:10
draft: false
lang: fa
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "اضافه کردن امضاهای تصویری به فایل DOCX با JavaScript"
head_description: "با استفاده از چند خط کد، امضای تصویری را به فایل DOCX برای Node.js اضافه کنید. از API GroupDocs.Signature for Node.js via Java برای اضافه کردن تصاویر استفاده کنید."

############################# Header ############################
title: "امضای فایل‌های DOCX با استفاده از امضاهای تصویری" 
description: "از قابلیت‌های GroupDocs.Signature for Node.js via Java برای جاسازی بی‌دردسر تصاویر در انواع مختلف فرمت‌های اسنادی مانند PDF، Word، Excel و انواع فایل‌های تصویری استفاده کنید. اضافه کردن یک تصویر امضای اجرایی می‌تواند به طور قابل توجهی حرفه‌ای بودن و اعتبار مدارک شما را افزایش دهد و ارائه‌ای ظریف و شیک ایجاد کند."
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
    title: "معرفی GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) به کاربران این امکان را می‌دهد که امضاهای تصویری را در هر نقطه‌ای از اسناد خود گنجانده و کارهای خود را با افزودن تصاویر به PDF، Word، Excel، PowerPoint و فرمت‌های تصویری رایج، تسهیل کنند و کارآمدی مدیریت اسناد را بهبود بخشند.

############################# Steps ############################
steps:
    enable: true
    title: "راهنمای افزودن تصاویر در DOCX با استفاده از JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) به برنامه‌های Node.js via Java این امکان را می‌دهد که امضاهای تصویری را به‌طور بی‌دردسر در اسناد DOCX یکپارچه کنند. قابلیت‌های برنامه شما را با کتابخانه جامع ما افزایش دهید.
      
      1. نخستین Signature را با سند DOCX ایجاد کنید
      2. از ImageSignOptions برای مشخص کردن تصویر امضا استفاده کنید
      3. تصویر را به دقت در هر صفحه قرار دهید
      4. سند امضا شده را در محل دلخواه ذخیره کنید
   
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

        // نخستین Signature را با مسیر سند تنظیم کنید
        const signature = new signatureLib.Signature('input.docx');

        // ImageSignOptions را برای شامل کردن امضای تصویری دلخواه پیکربندی کنید
        const options = new signatureLib.ImageSignOptions('company_logo.jpg');

        // تصویر را در گوشه بالا سمت چپ در تمامی صفحات قرار دهید
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);
        
        // سند را با امضای تصویری اعمال شده ذخیره کنید
        const result = signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "امکانات پیشرفته امضای اسناد"
  description: "API ما مجموعه‌ای از ویژگی‌ها را فراهم می‌کند که امضای الکترونیکی را ساده می‌کند. شما می‌توانید به راحتی امضاهای تصویری و انواع مختلف امضاها را اضافه، ویرایش، حذف، جستجو و تأیید کنید."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "امضاهای تصویری"
  features:
    # feature loop
    - title: "گنجاندن تصاویر در اسناد اداری"
      content: "امضاهای تصویری را به راحتی در هر نقطه‌ای از اسناد خود، چه در فایل‌های PDF، Word یا Excel، قرار دهید. با افزودن تصاویر، بارکدها، متا داده‌ها یا گواهی‌های دیجیتال به مدارک خود، آنها را بهبود ببخشید."

    # feature loop
    - title: "جستجو و تأیید امضاها"
      content: "با تأیید امضاها، از اعتبار اسناد امضاشده خود اطمینان حاصل کنید. از قابلیت جستجو برای بازیابی و بررسی تمامی امضاهای گنجانده شده در سند خود استفاده کنید."

    # feature loop
    - title: "ویرایش امضاهای موجود"
      content: "API ما به کاربران این امکان را می‌دهد که امضاها را بر اساس نیاز خود به‌روزرسانی و تنظیم کنند. اندازه، موقعیت یا ویژگی‌های دیگر هر امضا را برای انعطاف‌پذیری در مدیریت اسناد ویرایش کنید."

    # feature loop
    - title: "حذف امضاهای غیرضروری"
      content: "با حذف امضاهایی که دیگر نیازی به آنها ندارید، مدارک خود را به طور مؤثر مدیریت کنید. API ما از تمام عملیات CRUD برای تقریباً تمامی نوع امضاها پشتیبانی می‌کند."
      
  code_samples_ext:
    # code sample ext loop
    - title: "بهبود اسناد با امضاهای تصویری"
      content: |
        یاد بگیرید چگونه تصاویری را به اسناد تجاری اضافه کنید تا اطلاعات بیشتری را ارائه دهید.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // سندی را که باید امضا شود، انتخاب کنید
          const signature = new signatureLib.Signature('input.docx');

          // گزینه‌های تصویری را با مسیر تصویر پیکربندی کنید
          const options = new signatureLib.ImageSignOptions('manager_signature.jpg');

          // اندازه امضای تصویری را تنظیم کنید
          options.setWidth(100);
          options.setHeight(100);

          // تصویر را در گوشه پایین سمت راست قرار دهید
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // در صورت نیاز، از گوشه‌های صفحه فاصله‌گذاری کنید
          const padding = new signatureLib.Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // در صورت تمایل، مرز سفارشی را به تصویر اضافه کنید
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // امضای تصویری را برای ظاهر بهتر بچرخانید
          options.setRotationAngle(45);

          // سند به‌روز شده را در محل دلخواه ذخیره کنید
          const result = signature.sign('output.docx', options);
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
            link: "/examples/signature/formats/signature_image.docx"
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
    title: "عملکردهایی که ما ارائه می‌دهیم را کشف کنید"
    exclude: "image"
    description: "ما افتخار می‌کنیم که مجموعه وسیعی از روش‌ها و عملیات امضا را به نمایش بگذاریم."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "افزودن تصاویر به انواع فایل‌ها"
    exclude: "DOCX"
    description: "API Node.js via Java به شما این امکان را می‌دهد که تصاویر را به طیف وسیعی از فرمت‌های سندی اضافه کنید. اندازه، موقعیت و جایگاه صفحه را برای بهبود روند امضای اسناد خود سفارشی‌سازی کنید."
    items: 
          
        # format loop 1
        - name: "امضای PDF با تصویر"
          format: "PDF"
          link: "/signature/nodejs-java/image/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "امضای DOCX با تصویر"
          format: "DOCX"
          link: "/signature/nodejs-java/image/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "امضای JPEG با تصویر"
          format: "JPEG"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "امضای PPTX با تصویر"
          format: "PPTX"
          link: "/signature/nodejs-java/image/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "امضای XLSX با تصویر"
          format: "XLSX"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---