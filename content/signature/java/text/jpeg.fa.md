



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:54
draft: false
lang: fa
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "ایجاد امضاهای متنی JPEG با Java"
head_description: "از API Java برای درج امضاهای متنی در فایل‌های JPEG استفاده کنید. به‌طور بی‌دردسر فرمت‌های محبوب اسناد از جمله PDF، Word، Excel، ارائه‌ها، تصاویر و ZIP را پردازش کنید."

############################# Header ############################
title: "ایجاد امضاهای متنی برای JPEG" 
description: "امضاهای متنی سفارشی را به اسناد تجاری خود با استفاده از GroupDocs.Signature for Java اضافه کنید. گردش کار سازمانی را با گزینه‌های سفارشی‌سازی امضا‌ها بهینه کنید."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دریافت رایگان"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "درباره راهکار GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) امضاهای متنی انعطاف‌پذیر و قابل سفارشی‌سازی را برای ساده‌سازی وظایف مدیریت اسناد شما ارائه می‌دهد. محتوای امضاهای متنی را پیکربندی کرده و آن‌ها را به هر صفحه‌ای اعمال کنید و گردش کار اسنادی سازمان خود را بهبود دهید.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل افزودن امضاهای متنی به JPEG با استفاده از Java"
    content: |
      [GroupDocs.Signature](/signature/java/) می‌تواند در برنامه‌های Java ادغام شود تا امضاهای متنی به اسناد JPEG اضافه کند. توسعه‌دهندگان می‌توانند به‌سرعت عملکرد محصولات خود را با استفاده از راهکارهای ما گسترش دهند.
      
      1. از سند JPEG به‌عنوان پارامتر برای سازنده کلاس Signature استفاده کنید.
      2. نمونه‌ای از TextSignOptions با متن مناسب ایجاد کنید.
      3. گزینه‌های ظاهری امضا را پیکربندی کنید.
      4. امضای متنی را به هر صفحه‌ای از سند اضافه کنید.
   
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
        // مسیر سند را به سازنده Signature پاس دهید
        Signature signature = new Signature("input.jpeg");

        // نمونه‌ای از TextSignOptions با متن امضا ایجاد کنید
        TextSignOptions options = new TextSignOptions("Approved");
        
        // رنگ و ویژگی‌های فونت متن را تنظیم کنید
        options.setForeColor(Color.RED);
        SignatureFont signatureFont = new SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName("Comic Sans MS");
        options.setFont(signatureFont);

        // امضای متنی را به سند اضافه کنید
        SignResult result = signature.sign("output.jpeg", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "مدیریت امضاهای متنی اسناد"
  description: "با GroupDocs.Signature for Java می‌توانید گردش کار اسناد شرکت خود را با افزودن امضاهای متنی به فرمت‌های محبوب فایل بهینه کنید. به‌راحتی ظاهر و محتوای امضاها را تنظیم کنید."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضاهای اسناد"
      content: "امضاهای متنی، تصویری، بارکد، کد QR یا مهر را به هر صفحه از اسناد پشتیبانی‌شده اعمال کنید. از متاداده‌ها برای درج محتوای پنهان و تأمین امنیت اسناد خود با گواهی‌های دیجیتال استفاده کنید."

    # feature loop
    - title: "جستجو و تأیید امضاها"
      content: "سلامت اسناد امضا شده خود را با ابزار تأیید امضا ما تضمین کنید. همچنین می‌توانید تمامی امضاهای درج شده در یک سند را استعلام و جستجو کنید."

    # feature loop
    - title: "تغییر یا حذف امضاها"
      content: "محتوا، موقعیت و ظاهر امضاهای قبلاً اضافه‌شده را تغییر دهید یا آن‌ها را به‌طور کامل از سند حذف کنید."

    # feature loop
    - title: "امضاهای متنی بومی"
      content: "امضاهای متنی خاص سند، مانند برچسب‌ها در PDF یا واترمارک‌ها در اسناد Word را برای سفارشی‌سازی بیشتر اضافه کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "علامت‌گذاری اسناد با امضاهای متنی"
      content: |
        یاد بگیرید چگونه اطلاعات متنی را به اسناد تجاری اضافه کنید تا فرآیندهای تجاری بهبود یابد.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // یک سند را برای امضا انتخاب کنید
          Signature signature = new Signature("input.jpeg");

          // گزینه‌های متنی را با متن دلخواه ایجاد کنید
          TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025");

          // اندازه و موقعیت امضا را در صفحه مشخص کنید
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // امضاها از گوشه‌های صفحه فضای خالی را پشتیبانی می‌کنند
          Padding padding = new Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // رنگ و سبک فونت متن می‌تواند سفارشی‌سازی شود
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);

          // امضاهای متنی می‌توانند شامل یک حاشیه باشند
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // سفارشی‌سازی پس‌زمینه نیز در دسترس است
          Background background = new Background();
          background.setColor(Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // متن می‌تواند به‌عنوان تصویر برای سازگاری ذخیره شود
          options.setSignatureImplementation(TextSignatureImplementation.Image);

          // سند را با اضافه‌شده متن ذخیره کنید
          SignResult result = signature.sign("output.jpeg", options);
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
            link: "/examples/signature/formats/signature_text.jpeg"
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
    title: "ویژگی‌ها و گزینه‌های کلیدی امضا"
    exclude: "text"
    description: "راهکار ما از عملیات کامل CRUD و بیشتر برای هفت نوع مختلف امضا پشتیبانی می‌کند."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/java/esign/jpeg/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/java/text/jpeg/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/java/image/jpeg/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/java/barcode/jpeg/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/java/qrcode/jpeg/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/java/stamp/jpeg/"
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
    title: "افزودن امضاهای متنی به فرمت‌های مختلف فایل"
    exclude: "JPEG"
    description: "از API Java برای درج امضاهای متنی در اسناد Office استفاده کنید و کنترل کامل بر محتوای سند در هر مرحله از چرخه حیات آن داشته باشید."
    items: 
          
        # format loop 1
        - name: "امضای متنی PDF"
          format: "PDF"
          link: "/signature/java/text/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "امضای متنی DOCX"
          format: "DOCX"
          link: "/signature/java/text/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "امضای متنی JPEG"
          format: "JPEG"
          link: "/signature/java/text/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "امضای متنی PPTX"
          format: "PPTX"
          link: "/signature/java/text/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "امضای متنی XLSX"
          format: "XLSX"
          link: "/signature/java/text/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---