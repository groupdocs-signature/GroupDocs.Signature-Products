



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:14
draft: false
lang: fa
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "تأیید امضای الکترونیکی DOCX با استفاده از Java"
head_description: "GroupDocs.Signature for Java امکان تأیید امضاهای موجود در پرونده‌های DOCX را فراهم می‌کند. امضاها را در پی‌دی‌اف‌ها، اسناد ورد، ورق‌های اکسل، ارائه‌ها، تصاویر یا آرشیوهای زیپ تأیید کنید."

############################# Header ############################
title: "تأیید امضای الکترونیکی برای DOCX" 
description: "تمام امضاهای الکترونیکی پشتیبانی شده در PDF، Word، Excel، ارائه‌ها، تصاویر یا فایل‌های ZIP را با GroupDocs.Signature for Java تأیید کنید."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "نسخه رایگان را دانلود کنید"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "کاربردهای GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) از عملیات کامل CRUD برای امضای اسناد و بیشتر پشتیبانی می‌کند. بیش از 60 فرمت سند از جمله PDF، فایل‌های MS Office، تصاویر و آرشیوهای ZIP را با متن، تصویر، کد بار، گواهینامه‌های دیجیتال، متاداده و مهر تأیید کنید. عملیات اضافی مانند جستجو، تأیید، تغییر یا حذف امضاها نیز در دسترس است.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل تأیید امضاها در DOCX با استفاده از Java"
    content: |
      [GroupDocs.Signature](/signature/java/) می‌تواند وجود امضاهای خاص را در یک سند DOCX تأیید کند. توسعه‌دهندگان Java می‌توانند برنامه‌های خود را با افزودن ویژگی‌های ارائه‌شده توسط راه‌حل ما تقویت کنند.
      
      1. فایل DOCX را به نمونه Signature بارگذاری کنید.
      2. یک نمونه و گزینه‌های VerifyOptions را تنظیم کنید تا نتیجه دلخواه را به دست آورید.
      3. فرآیند تأیید را آغاز کنید.
      4. نتایج تأیید را بررسی کنید.
   
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
        // یک Signature را با سند ایجاد کنید
        Signature signature = new Signature("input.docx");

        // ایجاد TextVerifyOptions برای تأیید امضاهایی که شامل متن خاص هستند
        TextVerifyOptions options = new TextVerifyOptions();
        options.setText("signature");
        options.setMatchType(TextMatchType.Contains);

        // امضاهای موجود در سند را تأیید کنید
        VerificationResult result = signature.verify(options);

        // نتایج تأیید را پردازش کنید
        if (result.isValid())
        {
            System.out.print("\nDocument was verified successfully!");
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "راه‌حل جامع امضای اسناد"
  description: "GroupDocs.Signature فرمت‌های مستندات اداری محبوب را با 7 نوع امضا و عملیات کامل CRUD تقویت می‌کند و حفاظت قوی برای محتوای سند شما فراهم می‌کند."
  image: "/img/signature/features_verify.webp" # 500x500 px
  image_description: "تأیید امضا"
  features:
    # feature loop
    - title: "امضای اسناد شرکتی"
      content: "امضای دیجیتال حرفه‌ای را به هر سندی اضافه کنید. راه‌حل ما از انواع مختلف امضاها از جمله متن، تصاویر، کدهای بار، متاداده، مهرها و گواهینامه‌های دیجیتال پشتیبانی می‌کند."

    # feature loop
    - title: "عملیات CRUD امضا"
      content: "در بسیاری از موارد، اسناد امضا شده نیاز به پردازش بیشتری دارند. فهرستی از تمام امضاها در یک سند را بازیابی کنید، آنها را تأیید کنید، ویژگی‌های آنها را تغییر دهید یا در صورت نیاز حذف کنید."

    # feature loop
    - title: "حفاظت از محتوای سند"
      content: "به اسناد شرکتی خود با گواهینامه‌های دیجیتال برای جلوگیری از تغییرات غیرمجاز حفاظت کنید. متاداده‌های پنهان را برای محافظت بیشتر از محتوای سند جاساز کنید."

    # feature loop
    - title: "امضاهای بومی"
      content: "از امضاهای متنی خاص سند، مانند مهرهای PDF یا نقطه‌های آبی Word، برای ایجاد اسناد حرفه‌ای و سفارشی برای استفاده شرکتی بهره‌برداری کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "تأیید امضاهای کد بار"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان امضاهای کد بار را در یک سند تأیید کرد.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // سندی را که شامل امضاهای کد بار است ارائه دهید
          final Signature signature = new Signature("input.docx");

          // گزینه‌ها را برای تأیید کد بارها بر اساس متن خاص تنظیم کنید
          BarcodeVerifyOptions options = new BarcodeVerifyOptions();
          options.setText("12345");
          options.setMatchType(TextMatchType.StartsWith);

          // امضاهای اعمال شده بر روی سند را تأیید کنید
          VerificationResult result = signature.verify(options);

          // نتایج تأیید را نمایش دهید
          if (result.isValid())
          {
              System.out.print("\nDocument was verified successfully!");
          }
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
    title: "عملیات و انواع امضاهای پشتیبانی شده"
    exclude: "verify"
    description: "مجموعه کاملی از ویژگی‌ها و عملیات امضایی که توسط GroupDocs.Signature پشتیبانی می‌شوند را کشف کنید."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats #####################
more_formats:
    enable: true
    title: "تأیید امضا در فرمت‌های فایل مختلف"
    exclude: "DOCX"
    description: "GroupDocs.Signature for Java فرآیند تأیید تمام امضاها در یک سند را ساده می‌کند. پارامترهای تأیید سفارشی را تعیین کنید تا از یکپارچگی اسناد امضا شده اطمینان حاصل کنید."
    items: 
          
        # format loop 1
        - name: "بررسی امضاهای PDF"
          format: "PDF"
          link: "/signature/java/verify/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "بررسی امضاهای DOCX"
          format: "DOCX"
          link: "/signature/java/verify/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "بررسی امضاهای PPTX"
          format: "PPTX"
          link: "/signature/java/verify/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "اعتبارسنجی امضاهای XLSX"
          format: "XLSX"
          link: "/signature/java/verify/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---