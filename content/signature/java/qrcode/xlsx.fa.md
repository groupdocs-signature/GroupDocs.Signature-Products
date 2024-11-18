



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:01
draft: false
lang: fa
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "ایجاد کد QR برای XLSX با Java"
head_description: "API GroupDocs.Signature قابلیت تولید کدهای QR برای فایل‌های XLSX را فراهم می‌کند. کدهای QR را از محتوای خود ایجاد کنید و آنها را در هر صفحه‌ای قرار دهید."

############################# Header ############################
title: "ایجاد کدهای QR برای XLSX" 
description: "کدهای بارکد ۲ بعدی با داده‌های متنی و عددی را ایجاد کنید و آنها را در هر صفحه از اسناد مختلف با استفاده از GroupDocs.Signature for Java قرار دهید."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "آزمایش رایگان"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "بیشتر درباره GroupDocs.Signature for Java بیاموزید"
    link: "/signature/java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) مجموعه وسیعی از ویژگی‌ها را برای تولید و جاسازی انواع مختلف امضاها در تمام فرمت‌های اصلی سند ارائه می‌دهد. این API از فایل‌های PDF، اسناد Word، جداول Excel، ارائه‌های PowerPoint و تصاویر پشتیبانی می‌کند. اسناد خود را با امضاهای متنی، تصویری، بارکدی، QR کد، متا دیتا، دیجیتال و مهر ارتقا دهید.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل تولید و قرار دادن کد QR در هر مکان در XLSX"
    content: |
      [GroupDocs.Signature](/signature/java/) می‌تواند کدهای QR را در بسیاری از فرمت‌های محبوب تولید کند و آنها را در صفحات XLSX قرار دهد. بیش از ۱۰ نوع کد QR پشتیبانی می‌شود و می‌توان به سرعت در برنامه‌های Java یکپارچه سازی کرد. از محصول ما برای امضای اسناد با کدهای QR تولید شده استفاده کنید.
      
      1. فایل یا جریان XLSX که قرار است با کد QR امضا شود را دریافت کنید.
      2. متن مورد نظر برای QrCodeSignOptions را فراهم کنید.
      3. گزینه‌های بصری مانند رنگ، موقعیت، اندازه و غیره را سفارشی کنید.
      4. فایل را با کد QR ذخیره کنید.
   
    code:
      platform: "java"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "نمونه امضاها"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شد"
      links:
        #  loop
        - title: "نمونه‌های بیشتر"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // سند را به یک نمونه جدید از Signature منتقل کنید
        Signature signature = new Signature("input.xlsx");

        // از QrCodeSignOptions برای افزودن کد QR به سند استفاده کنید
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // نوع امضا و موقعیت آن در صفحه را مشخص کنید
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // فایل را با کد QR اضافه شده ذخیره کنید
        signature.sign("output.xlsx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "به اسناد خود امضا اضافه کنید"
  description: "API GroupDocs.Signature for Java از امضا کردن تمام فرمت‌های فایل رایج پشتیبانی می‌کند. تولید، ویرایش، جستجو، تأیید و حذف انواع مختلف امضاها را انجام دهید."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضای اسناد"
      content: "GroupDocs.Signature از امضای متنی، تصویری، بارکدی، QR کد و مهر پشتیبانی می‌کند. آنها را در هر صفحه‌ای از هر فرمت سند پشتیبانی شده قرار دهید. با استفاده از امضاهای متا دیتا، متا داده‌های سند را مدیریت کرده و محتوای آن را با استفاده از گواهی‌های دیجیتال در برابر تغییرات غیر مجاز محافظت کنید."

    # feature loop
    - title: "جستجو و تأیید"
      content: "اطمینان حاصل کنید که تمام امضاهای یک سند معتبر هستند با استفاده از رویه تأیید. با استفاده از ویژگی جستجوی داخلی، فهرست کاملی از امضاهای موجود در یک سند را بازیابی کنید."

    # feature loop
    - title: "ویرایش امضاها"
      content: "خصوصیات امضا را پس از امضا کردن به سادگی ویرایش کنید. محتوای آن را، موقعیت، رنگ، اندازه و سایر ویژگی‌ها را طبق نیاز تنظیم کنید."

    # feature loop
    - title: "حذف امضاها"
      content: "امضاهای ناخواسته را به سادگی حذف کنید. انواع مختلف امضاها، از جمله گواهی‌های دیجیتال، می‌توانند به صورت برنامه‌نویسی از اسناد حذف شوند."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه یک کد QR تولید شده را سفارشی کنید"
      content: |
        از این مثال برای یادگیری نحوه قرار دادن یک کد QR جدید بر روی صفحه XLSX استفاده کنید.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // سندی که نیاز به امضا دارد را بگیرید و به Signature منتقل کنید
          Signature signature = new Signature("input.xlsx");

          // از گزینه‌های کد QR برای ارائه متنی با اطلاعات لازم استفاده کنید
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // موقعیت نسبی کد QR را در صفحه تنظیم کنید
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // حاشیه امضا را تنظیم کنید
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // رنگ کد QR را مشخص کنید
          signOptions.setForeColor(Color.RED);

          // گزینه‌های فونت برای پیام را تعریف کنید
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // رنگ و قلم رنگ پس‌زمینه کد QR را سفارشی کنید
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // کد QR را به سند اضافه کنید
          SignResult signResult = signature.sign("output.xlsx", signOptions);
          ```
        platform: "java"
        copy_title: "کپی"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
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
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "امکانات GroupDocs.Signature را به صورت رایگان امتحان کنید یا درخواست مجوز ارسال کنید"
  items:
    #  loop
    - title: "بارگیری Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "مجوزدهی"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "این موارد کلیدی را بررسی کنید"
    exclude: "qrcode"
    description: "ما یک انتخاب متنوع از ویژگی‌های امضا و عملیات پیشرفته داریم."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "تولید کدهای QR برای فرمت‌های اضافی فایل"
    exclude: "XLSX"
    description: "تمام فرمت‌های فایل محبوب را با استفاده از API Java با کدهای QR تولید شده ارتقا دهید. داده‌های بارکد ۲ بعدی را برای سهولت در اسکن و پردازش اضافه کنید."
    items: 
          
        # format loop 1
        - name: "QR-Code برای PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "QR-Code برای DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "QR-Code برای JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "QR-Code برای PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "QR-Code برای XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---