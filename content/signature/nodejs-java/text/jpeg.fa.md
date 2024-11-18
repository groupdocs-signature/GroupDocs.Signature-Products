



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:56
draft: false
lang: fa
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "افزودن امضای متنی به JPEG از طریق JavaScript"
head_description: "با استفاده از API JavaScript، امضاهای متنی را به طور یکپارچه به اسناد JPEG اضافه کنید. API ما از طیف گسترده‌ای از فرمت‌ها، از جمله PDF، Word، Excel، ارائه‌ها، تصاویر و فایل‌های ZIP حمایت می‌کند."

############################# Header ############################
title: "افزودن امضای متنی به JPEG" 
description: "امضاهای متنی شخصی‌سازی‌شده را به فایل‌های تجاری خود با GroupDocs.Signature for Node.js via Java اضافه کنید. با تقویت گردش کار اسناد خود، کنترل بیشتری بر روی فرآیندهای کار خود داشته باشید."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "شروع آزمایش رایگان"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "معرفی GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) راه‌حل نوآورانه‌ای است که به اضافه کردن امضاهای متنی به اسناد کمک می‌کند. امضاها را در هر صفحه سفارشی و قرار دهید و کارایی در مدیریت اسناد را بهبود ببخشید. با ادغام نشانه‌های متنی شخصی‌سازی‌شده، فرآیندهای کسب‌وکار خود را بهینه کنید و هم عملکرد و هم حرفه‌ای‌گری را ارتقا دهید.

############################# Steps ############################
steps:
    enable: true
    title: "راهنمایی برای ایجاد امضاهای متنی برای JPEG با استفاده از JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) امکان افزودن امضاهای متنی به اسناد JPEG را در برنامه‌های Node.js via Java فراهم می‌آورد. به سرعت قابلیت‌های محصول خود را با راه‌حل‌های قوی ما تقویت کنید.
      
      1. سند JPEG را به عنوان آرگومان به کلاس Signature ارائه دهید.
      2. با متن مورد نیاز TextSignOptions را نمونه‌سازی کنید.
      3. خصوصیات بصری امضای متنی را تنظیم کنید.
      4. امضای متنی را به صفحه(های) مورد نظر سند اضافه کنید.
   
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

        // کلاس Signature را با مسیر سند اولیه‌سازی کنید
        const signature = new signatureLib.Signature('input.jpeg');

        // با متن مورد نیاز، TextSignOptions ایجاد کنید
        const options = new signatureLib.TextSignOptions('Approved');

        // خصوصیات رنگ و فونت متن را پیکربندی کنید
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // امضای متنی را به سند اضافه کنید
        const result = signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "کنترل بهبود یافته امضای متنی"
  description: "با GroupDocs.Signature for Node.js via Java، می‌توانید مدیریت امضاهای متنی در فرمت‌های کلیدی اسناد را به طرز چشمگیری بهبود بخشید. این ابزار به شما امکان می‌دهد تا سبک، مکان و محتوای امضاها را به راحتی پیکربندی کرده و از این طریق فرآیندهای اسنادی خود را سفارشی‌سازی کنید."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "ویژگی‌های اصلی GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضاهای متنی دینامیک"
      content: "امضاهای مختلفی مانند متن، تصاویر، بارکد، کدهای QR یا مهر را در هر صفحه از اسناد پشتیبانی شده وارد کنید. متادیتا را به منظور حمل اطلاعات پنهان وارد کنید یا گواهینامه‌های دیجیتال را برای اقدامات امنیتی پیشرفته اعمال کنید."

    # feature loop
    - title: "جستجو و اعتبارسنجی امضا"
      content: "اصالت امضاهای واردشده در اسناد خود را تأیید کنید. به جستجوی کارآمد برای یافتن تمام موارد امضا بپردازید تا اطمینان حاصل شود که مدیریت و پیگیری اسناد به طور کامل انجام می‌شود."

    # feature loop
    - title: "ویرایش یا حذف امضاها"
      content: "امضاهای قبلاً اضافه‌شده را برحسب نیاز تغییر یا حذف کنید. می‌توانید ظاهر، موقعیت یا محتوای هر امضا را برای برآورده کردن الزامات در حال تغییر تنظیم کنید و از این طریق انعطاف‌پذیری در مدیریت اسناد را تضمین کنید."

    # feature loop
    - title: "سفارشی‌سازی بومی امضا"
      content: "برای نوع‌های خاص فایل، مکان‌یابی امضا را با ویژگی‌های داخلی سند، مانند افزودن واترمارک به فایل‌های Word یا مهرهای سفارشی به PDF‌ها، سفارشی کنید و به این ترتیب منحصربفرد بودن اسناد خود را افزایش دهید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "پیاده‌سازی امضاهای متنی در اسناد"
      content: |
        یاد بگیرید که چگونه امضاهای متنی را به اسناد تجاری برای بهینه‌سازی فرآیندها پیوست کنید.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // سندی را که باید امضا شود انتخاب کنید
          const signature = new signatureLib.Signature('input.jpeg');

          // گزینه‌های متنی را با محتوای مشخص تعریف کنید
          const options = new signatureLib.TextSignOptions('Rescheduled to 03/04/2025');

          // اندازه و موقعیت امضا را در صفحه تعیین کنید
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // حاشیه‌ای برای امضا از لبه‌های صفحه اعمال کنید
          const padding = new signatureLib.Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // رنگ متن و سبک فونت را سفارشی کنید
          options.setForeColor(signatureLib.Color.RED);
          const signatureFont = new signatureLib.SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName('Comic Sans MS');
          options.setFont(signatureFont);

          // در صورت تمایل، دوری برای امضای متنی اضافه کنید
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // پس‌زمینه امضا را پیکربندی کنید
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // در صورت نیاز، متن را به عنوان تصویر برای سازگاری ذخیره کنید
          options.setSignatureImplementation(signatureLib.TextSignatureImplementation.Image);
          
          // سند را با امضای متنی اضافه‌شده ذخیره کنید
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
            link: "/examples/signature/formats/signature_text.jpeg"
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
    title: "ویژگی‌های جامع مدیریت امضا"
    exclude: "text"
    description: "پلتفرم ما عملیات کامل CRUD و ویژگی‌های پیشرفته‌ای را برای مدیریت هفت نوع مختلف امضا ارائه می‌دهد که به شما امکان می‌دهد امضاهای اسناد خود را با دقت و راحتی مدیریت کنید."
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
    title: "اعمال امضاهای متنی در فرمت‌های مختلف"
    exclude: "JPEG"
    description: "از قابلیت‌های API Node.js via Java برای ادغام امضاهای متنی در طیف وسیعی از فرمت‌های Office بهره‌برداری کنید. با افزودن نشانه‌های متنی بسیار قابل سفارشی‌سازی، جریان اطلاعات را در هر مرحله از چرخه زندگی سند خود کنترل کنید."
    items: 
          
        # format loop 1
        - name: "امضای متنی PDF"
          format: "PDF"
          link: "/signature/nodejs-java/text/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "امضای متنی DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/text/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "امضای متنی JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "امضای متنی PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/text/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "امضای متنی XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---