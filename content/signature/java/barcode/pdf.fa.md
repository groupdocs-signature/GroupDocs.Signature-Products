



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:24
draft: false
lang: fa
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "به راحتی بارکدها را به فایل‌های PDF با Java اضافه کنید"
head_description: "بارکدهای امضائی را به اسناد PDF در Java ایجاد و درج کنید. GroupDocs.Signature ادغام امضا را برای فرمت‌های مختلف امکان‌پذیر می‌سازد."

############################# Header ############################
title: "تولید بارکد برای PDF" 
description: "بارکدهای فرمت‌های محبوب را به هر نقطه‌ای در اسناد تجاری خود با GroupDocs.Signature for Java اضافه کنید. راه‌حل ما گزینه‌های گسترده‌ای برای سفارشی‌سازی امضاهای بارکد ارائه می‌دهد."
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
       [GroupDocs.Signature for Java](/signature/java/) یک راه‌حل پیشرفته امضا است که از انواع مختلف امضا پشتیبانی می‌کند. می‌توانید اسناد را با متن، تصاویر، بارکدها، گواهینامه‌های دیجیتال، مهر و ... در بیش از 60 فرمت فایل، از جمله PDF، MS Office، تصاویر، فایل‌های ZIP و دیگر فرمت‌های محبوب تجاری امضا کنید. علاوه بر این، امضاها در اسناد امضا شده می‌توانند هر زمان جستجو، تأیید، ویرایش یا حذف شوند.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل برای تولید و اضافه کردن بارکد به فایل PDF"
    content: |
      [GroupDocs.Signature](/signature/java/) می‌تواند بارکدها را در فرمت‌های مختلف محبوب تولید و آنها را در صفحات PDF قرار دهد. با پشتیبانی از بیش از 60 نوع بارکد، برنامه‌های Java می‌توانند به راحتی با قابلیت‌های امضای بارکد با ادغام کتابخانه ما بهبود یابند.
      
      1. فایل یا جریانی از PDF را برای پردازش ارائه دهید.
      2. متن بارکد را به نمونه BarcodeSignOptions منتقل کنید.
      3. گزینه‌های بارکد مانند موقعیت، اندازه و غیره را سفارشی کنید.
      4. فایل را با بارکد جدید اضافه شده ذخیره کنید.
   
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
        // ایجاد یک نمونه جدید از Signature با مسیر سند
        Signature signature = new Signature("input.pdf");

        // استفاده از BarcodeSignOptions برای اضافه کردن بارکد به سند
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // تنظیم نوع بارکد و سایر خصوصیات
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // ذخیره فایل امضا شده
        signature.sign("output.pdf", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "محتوای اسناد را با امضاها تقویت یا محافظت کنید"
  description: "کتابخانه GroupDocs.Signature for Java برای امضا و پردازش بیشتر فرمت‌های محبوب طراحی شده است. به سرعت و به سادگی انواع مختلف امضاها را اضافه، ویرایش، تأیید یا حذف کنید."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "ویژگی‌های GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضای سند"
      content: "هر صفحه از اسناد پشتیبانی شده را با متن، تصاویر، بارکدها، کدهای QR یا مهر امضا کنید. متاداده‌های پنهانی مانند EXIF در تصاویر اضافه کنید یا محتوای سند را از تغییرات غیرمجاز با استفاده از گواهینامه‌های دیجیتال محافظت کنید."

    # feature loop
    - title: "جستجو و تأیید امضا"
      content: "کارهای بیشتری می‌توان با یک سند امضا شده انجام داد. ما تأیید امضاها را برای اطمینان از درستی همه چیز ارائه می‌دهیم. همچنین می‌توانید فهرستی از تمامی امضاهای سند را از طریق جستجو بازیابی کنید."

    # feature loop
    - title: "ویرایش امضاها"
      content: "بیشتر امضاهای اضافه شده قبلی قابل ویرایش هستند. به راحتی متن را اصلاح کرده، موقعیت را تنظیم کنید یا رنگ را تغییر دهید."

    # feature loop
    - title: "حذف امضاها"
      content: "راه‌حل ما از عملیات CRUD کامل برای امضاها پشتیبانی می‌کند. انواع مختلفی از امضاها می‌توانند در صورت لزوم از یک سند حذف شوند."
      
  code_samples_ext:
    # code sample ext loop
    - title: "نحوه ایجاد امضای بارکد"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان بارکد سفارشی شده را در صفحات سند PDF قرار داد.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // سندی که باید امضا شود را فراهم کنید
          Signature signature = new Signature("input.pdf");

          // گزینه‌های امضا را با متن دلخواه ایجاد کنید
          BarcodeSignOptions signOptions = new BarcodeSignOptions("Accepted");
          signOptions.setEncodeType(BarcodeTypes.Code39FullASCII);

          // موقعیت نسبی بارکد را در صفحه تنظیم کنید
          signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Left);

          // فاصله بارکد را از لبه صفحه تنظیم کنید
          Padding padding = new Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // رنگ میله‌ها را تنظیم کنید
          signOptions.setForeColor(Color.RED);

          // نوع خط پیام را تعریف کنید
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Arial");
          signOptions.setFont(font);

          // موقعیت پیام را مشخص کنید
          signOptions.setCodeTextAlignment(CodeTextAlignment.Above);

          // سند را امضا کرده و ذخیره کنید
          SignResult signResult = signature.sign("output.pdf", signOptions);

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
            link: "/examples/signature/formats/signature_barcode.pdf"
        links:
          #  loop
          - title: "نمونه‌های بیشتر"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

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
    title: "قابلیت‌های اصلی ما را کشف کنید"
    exclude: "barcode"
    description: "ما با افتخار واریته وسیعی از امضاها و عملکردهای پشتیبانی شده را ارائه می‌دهیم"
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
    description: "بیش از 60 فرمت می‌توانند با استفاده از API Java ما امضا شوند. امضاهای مختلف را به هر صفحه یا موقعیتی در داخل سند اعمال کنید."
    items: 
          
        # format loop 1
        - name: "اضافه کردن بارکد به PDF"
          format: "PDF"
          link: "/signature/java/barcode/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "اضافه کردن بارکد به DOCX"
          format: "DOCX"
          link: "/signature/java/barcode/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "اضافه کردن بارکد به JPEG"
          format: "JPEG"
          link: "/signature/java/barcode/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "اضافه کردن بارکد به PPTX"
          format: "PPTX"
          link: "/signature/java/barcode/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "اضافه کردن بارکد به XLSX"
          format: "XLSX"
          link: "/signature/java/barcode/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---