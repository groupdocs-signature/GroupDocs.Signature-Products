



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:05
draft: false
lang: fa
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "اضافه کردن مهر به JPEG با استفاده از Java"
head_description: "از [[GroupDocs.Signature](/signature/java/)] و Java برای ایجاد مهرهای سفارشی و قرار دادن آنها در هر صفحه از اسناد JPEG استفاده کنید."

############################# Header ############################
title: "اضافه کردن مهرهای سفارشی به JPEG" 
description: "طراحی و اعمال مهرهای گرد یا چهارگوش به هر بخش از اسناد خود با استفاده از GroupDocs.Signature for Java. راه‌حل ما گزینه‌های سفارشی‌سازی زیادی را برای پاسخگویی به تمام نیازهای تجاری شما ارائه می‌دهد."
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
       [GroupDocs.Signature for Java](/signature/java/) ابزاری قوی است که به شما امکان می‌دهد امضای مهرهای مختلف را به اسناد اضافه کنید. این ابزار از بیش از 60 فرمت مختلف فایل، از جمله PDF، ورد، اکسل، تصاویر و فایل‌های ZIP پشتیبانی می‌کند. می‌توانید امضای متنی، تصویری، بارکد، متادیتا، گواهی دیجیتال و امضای مهر را اعمال کنید. علاوه بر اضافه کردن امضاها، می‌توانید آنها را جستجو، تأیید، ویرایش و حذف کنید.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل برای اضافه کردن مهر به JPEG با استفاده از Java"
    content: |
      [GroupDocs.Signature](/signature/java/) یک سازنده مهر فراهم می‌کند که می‌تواند برای برنامه‌های Java بسیار مفید باشد. از آن برای ایجاد مهرهای به خوبی سفارشی‌شده برای صفحات سند خود استفاده کنید.
      
      1. سند JPEG که قرار است مهر شود را ارائه دهید.
      2. از StampSignOptions برای پیکربندی تمام پارامترهای لازم استفاده کنید.
      3. به تعداد مورد نیاز خط اضافه کنید.
      4. مهر را اعمال کرده و سند را ذخیره کنید.
   
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
        // از مسیر سند با شی Signature استفاده کنید
        Signature signature = new Signature("input.jpeg");

        // شی StampSignOptions را با متن امضای مورد نظر ایجاد کنید
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // یک یا چند خط مهر اضافه کنید
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // سند مهر خورده را ذخیره کنید
        SignResult result = signature.sign("output.jpeg", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "محافظت از محتوای سند خود با امضاها"
  description: "کتابخانه GroupDocs.Signature for Java برای امضا و مدیریت امضاها در فرمت‌های فایل محبوب طراحی شده است. به‌راحتی مهرها و دیگر انواع امضاها را اضافه، ویرایش، تأیید یا حذف کنید."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "امضای مهر با GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضا کردن اسناد خود"
      content: "امضاهای سفارشی را به هر قسمت از سند خود اعمال کنید. از انواع مختلف امضا، از جمله متن، تصاویر، بارکدها، QR کدها و مهرها انتخاب کنید. علاوه بر این، متادیتای مخفی می‌تواند برای افزایش امنیت سند اضافه یا ویرایش شود."

    # feature loop
    - title: "جستجو و اعتبارسنجی امضاها"
      content: "هنگامی که یک سند امضا شده است، از ابزارهای تأیید ما استفاده کنید تا اطمینان حاصل کنید که محتوای امضا معتبر است. جستجو کرده و لیستی از تمام امضاها را برای پردازش‌های بعدی بازیابی کنید."

    # feature loop
    - title: "به‌روزرسانی امضاها در صورت نیاز"
      content: "به‌راحتی می‌توانید طیف گسترده‌ای از امضاهای اعمال‌شده روی یک سند را ویرایش کنید. خصوصیات مانند اندازه، رنگ، موقعیت، محتوا و موارد دیگر را به‌روز کنید."

    # feature loop
    - title: "حذف امضاها"
      content: "نیاز به حذف امضاها از یک سند دارید؟ API ما به‌طور کامل از حذف امضاها پشتیبانی می‌کند و مدیریت اسناد شما را آسان می‌کند."
      
  code_samples_ext:
    # code sample ext loop
    - title: "اضافه کردن مهرهای سفارشی به اسناد با استفاده از امضاهای ویژه"
      content: |
        بیاموزید که چگونه مهرهای سفارشی با اطلاعات متنی مهم را به اسناد خود تولید و اضافه کنید.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // سند مورد نظر برای مهر را ارائه دهید
          Signature signature = new Signature("input.jpeg");

          // شی گزینه‌های مهر را ایجاد کنید
          StampSignOptions options = new StampSignOptions();

          // اندازه و موقعیت بر روی صفحه را تنظیم کنید
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // یک یا چند خط گرد بیرونی با متن اضافه کنید
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // یک یا چند خط مربعی داخلی اضافه کنید
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // سند مهر خورده را ذخیره کنید
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "ویژگی‌های اصلی ما را کشف کنید"
    exclude: "stamp"
    description: "از طیف وسیعی از گزینه‌ها برای اضافه کردن، مدیریت و حذف امضاها استفاده کنید."
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
    title: "اضافه کردن مهر به چندین فرمت فایل"
    exclude: "JPEG"
    description: "API GroupDocs.Signature از قرار دادن مهر به اسناد در بیش از 60 فرمت پشتیبانی می‌کند. مهرها را در هر صفحه یا ناحیه قرار دهید تا مدیریت و سفارشی‌سازی سند را بهبود ببخشید."
    items: 
          
        # format loop 1
        - name: "مهر زدن PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "مهر زدن DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "مهر زدن JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "مهر زدن PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "مهر زدن XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---