



---
############################# Static ############################
layout: "format"
date:  2024-11-20T08:57:22
draft: false
lang: fa
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "اضافه کردن امضای دیجیتال الکترونیکی به فایل PDF با Java"
head_description: "با استفاده از Java یک امضای دیجیتال به فایل PDF اضافه کنید و تنها با چند خط کد. از GroupDocs.Signature for Java برای امضای چندین فرمت فایل استفاده کنید."

############################# Header ############################
title: "امضای PDF با امضاهای دیجیتال" 
description: "محتوای اسناد تجاری خود را با مهرهای دیجیتال با استفاده از ویژگی‌های GroupDocs.Signature for Java امن کنید. ما چندین روش برای علامت‌گذاری و تأمین امنیت اسناد شما ارائه می‌دهیم."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "درباره GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) یک راه‌حل جامع امضا است که از انواع مختلف پردازش اسناد پشتیبانی می‌کند. شما می‌توانید متن، تصاویری، گواهی‌های دیجیتال و مهرها را به فایل‌ها در 60+ فرمت، از جمله PDF، MS Office، تصاویر، فایل‌های ZIP و سایر فرمت‌های محبوب تجاری اضافه کنید. همچنین، اسناد امضا شده می‌توانند به دستگاه‌های جستجو، تأیید، ویرایش یا به‌طور خودکار حذف شوند.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل حفاظت از PDF با گواهی‌های دیجیتال در Java"
    content: |
      [GroupDocs.Signature](/signature/java/) به توسعه‌دهندگان Java اجازه می‌دهد تا تغییرات را در اسناد PDF با استفاده از امضاهای دیجیتال مسدود کنند. برنامه‌های تجاری خود را با قابلیت تأمین امنیت داده‌های مهم مجهز کنید.
      
      1. سند PDF را به سازنده کلاس Signature منتقل کنید.
      2. از یک گواهی دیجیتال و رمز عبور آن برای محافظت از سند استفاده کنید.
      3. اختیاری: نمای بصری امضای دیجیتال را بر روی صفحات سند اضافه کنید.
      4. سند را امضا کنید تا از هرگونه تغییرات آینده جلوگیری شود.
   
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
        // از Signature با سند برای امضای دیجیتال استفاده کنید
        Signature signature = new Signature("input.pdf");

        // یک گواهی دیجیتال و رمز عبور را فراهم کنید
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        options.setPassword("1234567890");

        // در صورت لزوم، نمای بصری را تنظیم کنید
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);

        // سند را با یک گواهی دیجیتال محافظت کنید
        SignResult result = signature.sign("output.pdf", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "تقویت یا حفاظت از محتوای سند با امضاها"
  description: "کتابخانه GroupDocs.Signature for Java قادر به امضای تمامی فرمت‌های فایل محبوب است. امضاهای مختلف را به‌طور خودکار اضافه، ویرایش، تأیید یا حذف کنید تا پروسه‌های تجاری خود را تسهیل کنید."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "ویژگی‌های GroupDocs.Signature"
  features:
    # feature loop
    - title: "اضافه کردن امضاها به اسناد"
      content: "امضاهای متنی، تصویری، بارکدی، کد QR یا مهرها به‌دقت می‌توانند به هر صفحه از هر سند پشتیبانی‌شده اضافه شوند. داده‌های متا پنهان مانند EXIF می‌توانند در تصاویر و بیشتر انواع فایل‌ها اضافه یا ویرایش شوند. محتواهای سند را از تغییرات غیرمجاز با استفاده از امضاهای دیجیتال محافظت کنید."

    # feature loop
    - title: "جستجو و تأیید امضا"
      content: "پس از امضا، اسناد می‌توانند به شیوه‌های مختلف پردازش شوند. اسناد امضا شده را تأیید کنید تا از پردازش صحیح آن‌ها اطمینان حاصل کنید. اگر به کنترل بیشتری نیاز دارید، فهرستی از تمام امضاها را از طریق جستجو بدست آورید."

    # feature loop
    - title: "ویرایش امضاها"
      content: "اکثر انواع امضاها از ویرایش بیشتر پشتیبانی می‌کنند. شما آزاد هستید تا متن را اصلاح کرده، موقعیت، رنگ، اندازه و غیره را تغییر دهید."

    # feature loop
    - title: "حذف امضاهای غیر ضروری"
      content: "راه‌حل ما از عملیات CRUD کامل برای امضاها پشتیبانی می‌کند. بسیاری از انواع امضاها، از جمله گواهی‌های دیجیتال، می‌توانند در صورت نیاز از یک سند حذف شوند."
      
  code_samples_ext:
    # code sample ext loop
    - title: "محافظت از اسناد با امضاهای دیجیتال"
      content: |
        یاد بگیرید چگونه یک سند را از تغییرات با استفاده از امضاهای دیجیتال تأمین امنیت کنید.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // یک سند برای امضا کردن ارائه دهید
          Signature signature = new Signature("input.pdf");

          // از یک گواهی دیجیتال معتبر با رمز عبور استفاده کنید
          DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
          options.setPassword("1234567890");

          // داده‌های متنی اضافی را مشخص کنید
          options.setReason("Security issue");
          options.setContact("John Smith");
          options.setLocation("Office D.W.");

          // از یک تصویر و سایر گزینه‌ها برای نمای بصری استفاده کنید
          options.setImageFilePath("image.png");

          options.setAllPages(true);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setWidth(80);
          options.setHeight(60);

          Padding padding = new Padding();
          padding.setBottom(10);
          padding.setRight(10);
          options.setMargin(padding);

          // سند محافظت‌شده را در مکان دیگری ذخیره کنید
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
            link: "/examples/signature/formats/signature_digital.pdf"
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
    title: "ویژگی‌های جامع ما را بررسی کنید"
    exclude: "digital"
    description: "ما به عملکرد گسترده و حمایت از امضاهایی که پلتفورم ما ارائه می‌دهد، افتخار می‌کنیم."
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
    title: "امضای اسناد در فرمت‌های دیگر"
    exclude: "PDF"
    description: "API Java به شما امکان می‌دهد تا بیش از 60 فرمت را پردازش کنید. امضاهای مختلفی بسازید و به هر صفحه اضافه کنید، محتوا را با گواهی‌های دیجیتال مهر کنید و امضاهای موجود در سند را مدیریت و ویرایش کنید."
    items: 
          
        # format loop 1
        - name: "محافظت از PDF"
          format: "PDF"
          link: "/signature/java/digital/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "محافظت از DOCX"
          format: "DOCX"
          link: "/signature/java/digital/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "محافظت از PPTX"
          format: "PPTX"
          link: "/signature/java/digital/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "محافظت از XLSX"
          format: "XLSX"
          link: "/signature/java/digital/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---