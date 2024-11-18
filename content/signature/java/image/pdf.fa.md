



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:49
draft: false
lang: fa
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "اضافه کردن امضای تصویری به فایل PDF با استفاده از Java"
head_description: "امضای تصویری را به فایل PDF برای Java با چند خط کد اضافه کنید. از API GroupDocs.Signature for Java برای افزودن تصاویر استفاده کنید."

############################# Header ############################
title: "امضای فایل‌های PDF با امضای تصویری" 
description: "از GroupDocs.Signature for Java برای درج تصاویر در قالب‌های مختلف اسناد اداری، از جمله PDF، Word، Excel و فرمت‌های تصویری استفاده کنید. یک تصویر با امضای مدیر می‌تواند تأثیر شگرفی داشته باشد!"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "رایگان دانلود کنید"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "آشنایی با GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) این امکان را فراهم می‌کند تا امضای تصویری را به هر صفحه و مکانی در اسناد تجاری اضافه کنید. با افزودن تصاویر به PDFها، اسناد Word، صفحات Excel، ارائه‌های PowerPoint و فرمت‌های تصویری محبوب، جریان‌های کاری خود را بهینه کنید.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل افزودن یک تصویر به هر مکانی از یک PDF با استفاده از Java"
    content: |
      [GroupDocs.Signature](/signature/java/) قابلیت افزودن امضاها به هر صفحه از اسناد PDF را دقیقاً ارتقا می‌دهد. با ادغام کتابخانه ما، عملکرد محصول خود را افزایش دهید.
      
      1. یک نمونه از Signature با سند PDF ایجاد کنید.
      2. از ImageSignOptions برای مشخص کردن تصویر امضا استفاده کنید.
      3. تصویر را در هر موقعیتی از هر صفحه قرار دهید.
      4. سند امضا شده را در یک مکان جدید ذخیره کنید.
   
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
        // ایجاد نمونه‌ای از Signature با مسیر سند
        Signature signature = new Signature("input.pdf");

        // ایجاد ImageSignOptions با استفاده از یک تصویر برای امضا
        ImageSignOptions options = new ImageSignOptions("company_logo.jpg");

        // قرار دادن تصویر در بالای گوشه چپ تمام صفحات
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);

        // ذخیره سند امضا شده
        SignResult result = signature.sign("output.pdf", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "راه حل جامع امضای سند"
  description: "API ما از طیف وسیعی از ویژگی‌های امضا پشتیبانی می‌کند و به شما این امکان را می‌دهد که انواع مختلف امضاها، از جمله امضاهای تصویری، را اضافه، ویرایش، حذف، جستجو و تأیید کنید."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "امضای تصویری"
  features:
    # feature loop
    - title: "درج تصاویر در اسناد اداری"
      content: "به سادگی امضاهای تصویری را در هر موقعیتی از هر صفحه یک سند قرار دهید. محتوای خود را با متن، تصاویر، بارکدها، متاداده و گواهی‌نامه‌های دیجیتال غنی کنید."

    # feature loop
    - title: "جستجو و تأیید امضا"
      content: "به راحتی اعتبار امضاها را در اسناد امضا شده تأیید کنید. فهرستی از تمام امضاها درون یک سند را بازیابی کرده و اطلاعات دقیق در مورد هر یک را بررسی کنید."

    # feature loop
    - title: "ویرایش امضا"
      content: "محتوا، ظاهر، اندازه یا موقعیت هر امضای قبلاً اضافه شده به یک سند را به روز کنید. API ما ویرایش امضاها را ساده و مؤثر می‌کند."

    # feature loop
    - title: "حذف امضاهای غیرضروری"
      content: "API ما از عملیات کامل CRUD برای اکثر انواع امضا پشتیبانی می‌کند. شما می‌توانید به راحتی امضاها را از تقریباً همه انواع اسناد پشتیبانی شده در صورت نیاز حذف کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "بهبود محتوای سند با امضاهای تصویری"
      content: |
        یاد بگیرید چگونه تصاویر را به اسناد تجاری اضافه کنید تا اطلاعات اضافی ارائه دهید.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // یک سند برای امضا انتخاب کنید
          Signature signature = new Signature("input.pdf");

          // گزینه‌های تصویری را با مسیر تصویر ایجاد کنید
          ImageSignOptions options = new ImageSignOptions("manager_signature.jpg");

          // اندازه امضای تصویری را تنظیم کنید
          options.setWidth(100);
          options.setHeight(100);

          // تصویر را در گوشه پایین سمت راست قرار دهید
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);

          // اگر لازم است حاشیه‌ای از گوشه‌های صفحه اعمال کنید
          Padding padding = new Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // در صورت تمایل یک کادر سفارشی به تصویر اضافه کنید
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // امضا را برای هماهنگی بهتر بچرخانید
          options.setRotationAngle(45);

          // سند به روز شده را در هر مکانی ذخیره کنید
          SignResult result = signature.sign("output.pdf", options);

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
            link: "/examples/signature/formats/signature_image.pdf"
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
    title: "به قابلیت‌های پیشرفته ما نگاهی بیندازید"
    exclude: "image"
    description: "خوشحالیم که مجموعه‌ای از ابزارها و عملیات‌های امضا را معرفی کنیم."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "اضافه کردن تصاویر به سایر فرمت‌های فایل"
    exclude: "PDF"
    description: "با استفاده از API Java، شما می‌توانید فرمت‌های تصویری پشتیبانی شده را به اسناد مختلف وارد کنید. به سادگی اندازه را تغییر دهید، موقعیت را انتخاب کنید و امضاهای تصویری را به اسناد خود اضافه کنید."
    items: 
          
        # format loop 1
        - name: "امضای PDF با تصویر"
          format: "PDF"
          link: "/signature/java/image/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "امضای DOCX با تصویر"
          format: "DOCX"
          link: "/signature/java/image/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "امضای JPEG با تصویر"
          format: "JPEG"
          link: "/signature/java/image/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "امضای PPTX با تصویر"
          format: "PPTX"
          link: "/signature/java/image/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "امضای XLSX با تصویر"
          format: "XLSX"
          link: "/signature/java/image/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---