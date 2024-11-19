



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:09
draft: false
lang: fa
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "اضافه کردن امضای تصویر به فایل XLSX با C#"
head_description: "امضای تصویری را روی فایل XLSX برای .NET با استفاده از چند خط کد قرار دهید. از API GroupDocs.Signature for .NET برای اضافه کردن تصاویر استفاده کنید."

############################# Header ############################
title: "اضافه کردن امضای تصویر به فایل‌های XLSX" 
description: "از GroupDocs.Signature for .NET برای یکپارچه‌سازی بی‌نقص تصاویر در مجموعه وسیعی از فرمت‌های اسناد اداری، از جمله PDF، Word، Excel و فایل‌های تصویری استفاده کنید. افزودن تصویری از امضای رئیس شما می‌تواند تأثیر حرفه‌ای چشمگیری ایجاد کند و جذابیت بصری و اعتبار اسناد شما را افزایش دهد."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "کشف GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) امکانات جامع برای جاسازی امضای تصویر در هر مکان از هر صفحه در اسناد تجاری شما را ارائه می‌دهد. با یکپارچه‌سازی تصاویر در PDF‌ها، اسناد Word، صفحات Excel، ارائه‌های PowerPoint و مجموعه‌ای از فرمت‌های تصویری محبوب از طریق کتابخانه قوی ما، جریان‌های کاری خود را بهبود بخشید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه یک تصویر در هر مکانی از XLSX با استفاده از C# اضافه کنیم"
    content: |
      از [GroupDocs.Signature](/signature/net/) برای تقویت برنامه‌های .NET با قابلیت جاسازی دقیق امضاها در هر صفحه از اسناد XLSX استفاده کنید. به آسانی قابلیت‌های محصول خود را با یکپارچه‌سازی راه‌حل ما تقویت کنید.
      
      1. کلاس Signature را با سند XLSX ایجاد کنید.
      2. از ImageSignOptions برای مشخص کردن تصویر امضا استفاده کنید.
      3. تصویر را به دقت در هر مکان دلخواه صفحه قرار دهید.
      4. سند امضا شده جدید را در مکان مشخص‌شده ذخیره کنید.
   
    code:
      platform: "net"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "نمونه امضاها"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شد"
      links:
        #  loop
        - title: "نمونه‌های بیشتر"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // مقداردهی اولیه Signature با مسیر سند
        using (Signature signature = new Signature("input.xlsx"))
        {
            // تنظیم ImageSignOptions با استفاده از یک تصویر برای امضا
            ImageSignOptions options = new ImageSignOptions("company_logo.jpg")
            {
                // موقعیت تصویر در گوشه بالا سمت چپ تمام صفحات
                AllPages = true,
                Left = 100,
                Top = 200
            };

            // ذخیره سند امضا شده
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "راهکارهای جامع امضای سند"
  description: "خوشحالیم که مجموعه وسیعی از قابلیت‌های امضای پشتیبانی شده توسط API ما را ارائه می‌دهیم. به آسانی انواع مختلف امضا، از جمله امضاهای مبتنی بر تصویر را اضافه، ویرایش، حذف، جستجو و تأیید کنید."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "امضای تصویر"
  features:
    # feature loop
    - title: "جاسازی تصاویر در اسناد اداری"
      content: "به آسانی امضاهای الکترونیکی و تصاویر را در هر موقعیت مشخص در هر صفحه از یک سند وارد کنید. محتوای سند خود را با متن، تصاویر، بارکدها، متاداده یا گواهی‌های دیجیتال به منظور افزایش کارایی و امنیت تقویت کنید."

    # feature loop
    - title: "جستجو و تأیید امضاها"
      content: "اسناد امضا شده را با تأیید صحت و یکپارچگی امضاها مدیریت کنید. فهرستی جامع از تمام امضاها در یک سند را بازیابی کرده و ویژگی‌های خاص آن‌ها را بررسی کنید."

    # feature loop
    - title: "ویرایش امضاها"
      content: "گاهی امضاها در اسناد نیاز به به‌روزرسانی دارند. به راحتی محتوای، ظاهر، اندازه یا موقعیت امضاهای موجود را برای تطابق با نیازهای در حال تغییر تنظیم کنید."

    # feature loop
    - title: "حذف امضاهای زاید"
      content: "API ما عملیات CRUD کاملی را برای اکثر انواع امضاها تسهیل می‌کند. می‌توانید به طور مؤثری امضاها را از تقریباً تمام فرمت‌های مستندات پشتیبانی شده حذف کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "تأمین امنیت محتوای سند با امضاهای تصویری"
      content: |
        یاد بگیرید که چگونه اسناد تجاری را با جاسازی تصاویر غنی کنید و اطلاعات تکمیلی ارائه دهید.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // سند مورد نظر برای امضا را انتخاب کنید
          using (Signature signature = new Signature("input.xlsx"))
          {
              // گزینه‌های تصویر را با مسیر تصویر مشخص‌شده ایجاد کنید
              ImageSignOptions options = new ImageSignOptions("manager_signature.jpg")
              {
                    // ابعاد امضای تصویر را تعریف کنید
                    Width = 100,
                    Height = 100,

                    // تصویر را در گوشه پایین سمت راست قرار دهید
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,

                    // فضای لازم را از لبه‌های صفحه اعمال کنید
                    Margin = new Padding() { Bottom = 120, Right = 120 },

                    // به صورت اختیاری، یک حاشیه دلخواه به تصویر اضافه کنید
                    Border = new Border()
                    {
                        Visible = true,
                        Color = Color.Red,
                        DashStyle = DashStyle.DashDotDot,
                        Weight = 5
                    },

                    // امضا را برای هم‌ترازی بهینه بچرخانید
                    RotationAngle = 45
              };

              // سند به‌روز شده را در مکان مورد نظر ذخیره کنید
              SignResult result = signature.Sign("output.xlsx", options);
          }
          ```
        platform: "net"
        copy_title: "کپی"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "برای کپی کلیک کنید"
          copy_done: "کپی شد"
        top_links:
          #  loop
          - title: "دانلود نتیجه"
            icon: "download"
            link: "/examples/signature/formats/signature_image.xlsx"
        links:
          #  loop
          - title: "نمونه‌های بیشتر"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "امکانات GroupDocs.Signature را به صورت رایگان امتحان کنید یا درخواست مجوز ارسال کنید"
  items:
    #  loop
    - title: "بارگیری Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "مجوزدهی"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "درک پیشنهادات ویژگی ما"
    exclude: "image"
    description: "مجموعه متنوعی از انواع امضا و عملیات قوی ارائه شده توسط پلتفرم ما را کاوش کنید."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "یکپارچه‌سازی تصاویر در فرمت‌های مختلف فایل"
    exclude: "XLSX"
    description: "از API .NET برای الحاق فرمت‌های تصویری پشتیبانی شده به مجموعه‌ای گسترده از اسناد استفاده کنید. به راحتی اندازه، موقعیت، انتخاب صفحات خاص و اعمال امضاهای مبتنی بر تصویر را به اسناد خود اضافه کنید."
    items: 
          
        # format loop 1
        - name: "امضای PDF با تصویر"
          format: "PDF"
          link: "/signature/net/image/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "امضای DOCX با تصویر"
          format: "DOCX"
          link: "/signature/net/image/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "امضای JPEG با تصویر"
          format: "JPEG"
          link: "/signature/net/image/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "امضای PPTX با تصویر"
          format: "PPTX"
          link: "/signature/net/image/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "امضای XLSX با تصویر"
          format: "XLSX"
          link: "/signature/net/image/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---