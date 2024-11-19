



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:31
draft: false
lang: fa
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "جستجوی امضا دیجیتال در PPTX با Java"
head_description: "از API GroupDocs.Signature for Java برای جستجوی امضاها در فایل‌های PPTX استفاده کنید. امضاها را در PDF، Word، Excel، ارائه‌ها و تصاویر پیدا کنید."

############################# Header ############################
title: "جستجوی امضاهای دیجیتال در PPTX" 
description: "لیست کاملی از امضاهای الکترونیکی که در فایل‌های PDF، Word، Excel، ارائه‌ها یا تصاویر جاسازی شده‌اند را با استفاده از GroupDocs.Signature for Java استخراج کنید."
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
       [GroupDocs.Signature for Java](/signature/java/) ویژگی‌های قدرتمندی برای امضای مدارک ارائه می‌دهد. این نرم‌افزار از افزودن متن، تصاویر، بارکدها، گواهی‌های دیجیتال و مهرها به فایل‌ها در بیش از 60 فرمت از جمله PDF، اسناد MS Office، تصاویر، فایل‌های ZIP و فرمت‌های تجاری رایج پشتیبانی می‌کند. علاوه بر این، می‌توانید در هر زمان امضاها را جستجو، تأیید، ویرایش یا حذف کنید.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل جستجوی امضاهای PPTX با استفاده از Java"
    content: |
      [GroupDocs.Signature](/signature/java/) یک موتور قدرتمند برای جستجوی هر نوع امضای دیجیتال در فایل‌های PPTX ارائه می‌دهد. توسعه‌دهندگان Java می‌توانند برنامه‌های خود را با راه‌حل ما تقویت کنند.
      
      1. مسیر فایل PPTX را برای جستجوی امضا فراهم کنید.
      2. از SearchOptions برای بهینه‌سازی نتایج جستجو استفاده کنید.
      3. متد جستجو را اجرا کنید تا نتایج را به دست آورید.
      4. لیست امضاهای پیدا شده را تحلیل کنید.
   
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

        // ایجاد یک نمونه از Signature با مسیر سند
        final Signature signature = new Signature("input.pptx");

        // ایجاد نمونه‌ای از TextSearchOptions برای پوشش تمام صفحات
        TextSearchOptions options = new TextSearchOptions();
        options.setAllPages(true);

        // جستجوی امضاهای متنی در سند
        List<TextSignature> signatures = signature.search(TextSignature.class, options);
        System.out.print("\nSource document contains following text signature(s).");

        // لیست امضاهای پیدا شده برای تحلیل بیشتر
        for (TextSignature textSignature : signatures) {
            System.out.print("Found Text signature at page " + textSignature.getPageNumber() 
                + " with type [" + textSignature.getSignatureImplementation() + "] and 
                text '" + textSignature.getText() + "'.");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "راه‌حل جامع امضای مدارک"
  description: "ما مفتخریم که راه‌حل امضای مدارک خود را معرفی کنیم که با تمام فرمت‌های اصلی مدارک سازگار است. یک دامنه وسیع از امضاها را برای بهبود مدارک خود اضافه کنید یا محتوای آن‌ها را ایمن سازید."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "جستجوی امضا"
  features:
    # feature loop
    - title: "امضای مدارک تجاری"
      content: "امضاهای دیجیتال را در هر مکان از هر صفحه یک سند وارد کنید. از انواع مختلف امضاها مانند متن، تصاویر، بارکدها، متادیتا، مهرها یا گواهی‌های دیجیتال استفاده کنید."

    # feature loop
    - title: "مدیریت امضاها"
      content: "پس از امضا کردن، ممکن است مدارک نیاز به پردازش بیشتری داشته باشند. همه امضاهای موجود را جستجو کنید و هر زمان که لازم بود، آن‌ها را به‌روزرسانی یا حذف کنید."

    # feature loop
    - title: "حفاظت از محتوای سند"
      content: "متادیتای پنهانی که در سند جاسازی شده است را مدیریت کنید. متادیتای جدید اضافه کنید یا ورودی‌های موجود را حذف کنید. از گواهی‌های دیجیتال شرکتی برای محافظت از محتوای سند در برابر تغییرات غیرمجاز استفاده کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "جستجوی امضاهای تصویری"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان یک امضای تصویری را در یک سند خاص پیدا کرد.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // مدرک منبع را به عنوان پارامتر سازنده منتقل کنید
          final Signature signature = new Signature("input.pptx");

          // با نوع متن هر امضایی را جستجو کنید
          List<ImageSignature> signatures = signature.search(ImageSignature.class, SignatureType.Image);
          System.out.print("\nSource document contains following image signature(s).");

          // نتایج را با خواص امضاهای پیدا شده نمایش دهید
          for (ImageSignature imageSignature : signatures)
          {
              System.out.print("Image signature found at page "+imageSignature.getPageNumber()+
                    " with size "+imageSignature.getSize()+". Created "+imageSignature.getCreatedOn()+
                    ", modified "+imageSignature.getModifiedOn());
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
    title: "عملیات پشتیبانی شده"
    exclude: "search"
    description: "محصول ما API انعطاف‌پذیری برای امضای مدارک و مدیریت امضاها پس از امضا کردن ارائه می‌دهد."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/java/esign/pptx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/java/text/pptx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/java/image/pptx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/java/barcode/pptx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/java/qrcode/pptx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/java/digital/pptx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/java/stamp/pptx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/java/search/pptx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/java/verify/pptx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/java/modify/pptx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/java/delete/pptx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "جستجوی امضاها در فرمت‌های مختلف فایل"
    exclude: "PPTX"
    description: "API GroupDocs.Signature for Java به شما امکان می‌دهد تا فهرستی از امضاها را از هر فایل امضاشده استخراج کنید. امضاها را از فرمت‌های محبوب فایل برای پردازش بیشتر استخراج کنید."
    items: 
          
        # format loop 1
        - name: "جستجوی امضاها در PDF"
          format: "PDF"
          link: "/signature/java/search/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "یافتن امضاها در DOCX"
          format: "DOCX"
          link: "/signature/java/search/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "یافتن امضاها در PPTX"
          format: "PPTX"
          link: "/signature/java/search/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "جستجوی امضاها در XLSX"
          format: "XLSX"
          link: "/signature/java/search/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---