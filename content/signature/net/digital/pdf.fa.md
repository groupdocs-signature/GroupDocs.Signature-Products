



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:58
draft: false
lang: fa
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "اضافه کردن امضاهای الکترونیکی دیجیتال به فایل PDF با C#"
head_description: "روی یک فایل PDF امضای دیجیتال قرار دهید با استفاده از C# تنها با چند خط کد. از GroupDocs.Signature for .NET برای امضای فرمت‌های مختلف فایل استفاده کنید."

############################# Header ############################
title: "امضای دیجیتال PDF با امضاهای دیجیتال" 
description: "سلامت اسناد تجاری خود را با استفاده از گواهی‌های دیجیتال و ویژگی‌های قوی GroupDocs.Signature for .NET محکم کنید. ما راهکارهای متنوعی برای نشانه‌گذاری و ایمن‌سازی اسناد شما ارائه می‌دهیم."
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
    title: "درباره GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) یک راه‌حل پیشرفته امضا است که طیف وسیعی از وظایف پردازش سند را تسهیل می‌کند. این نرم‌افزار به شما اجازه می‌دهد تا متن، تصاویر، گواهی‌های دیجیتال و مهرها را به فایل‌ها در بیش از 60 فرمت، از جمله PDF، MS Office، تصاویر، فایل‌های ZIP و سایر فرمت‌های ضروری تجاری وارد کنید. علاوه بر این، اسناد امضا شده می‌توانند به راحتی جستجو، تأیید، ویرایش یا حذف شوند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه PDF را با گواهی‌های دیجیتال در C# ایمن کنید"
    content: |
      [GroupDocs.Signature](/signature/net/) به توسعه‌دهندگان .NET اجازه می‌دهد سندهای PDF را در مقابل تغییرات با استفاده از امضاهای دیجیتال ایمن کنند. برنامه‌های تجاری خود را با قابلیت‌های قوی حفاظت از داده‌ها تقویت کنید.
      
      1. فایل PDF را به سازنده کلاس Signature پاس دهید.
      2. برای ایمن‌سازی سند از یک گواهی دیجیتال و رمز عبور آن استفاده کنید.
      3. اختیاری، نمای تصویری امضای دیجیتال را در صفحات سند اضافه کنید.
      4. سند را امضا کنید تا مطمئن شوید که دست نخورده باقی مانده است.
   
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
        // از Signature برای امضای دیجیتال سند استفاده کنید
        using (Signature signature = new Signature("input.pdf"))
        {
            // گواهی دیجیتال و رمز عبور مرتبط را ارائه دهید
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // اگر نیاز است، نمای تصویری را تنظیم کنید
                PageNumber = 1,
                Left = 50,
                Top = 50
            };

            // سند را با گواهی دیجیتال ایمن کنید
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "محتوای سند را با امضاها افزایش یا ایمن کنید"
  description: "کتابخانه GroupDocs.Signature for .NET برای امضای تمام فرمت‌های فایل رایج طراحی شده است. فرآیندهای تجاری خود را با افزودن، ویرایش، تأیید یا حذف انواع مختلف امضاها ساده کنید."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Signature"
  features:
    # feature loop
    - title: "گنجاندن امضاها در اسناد"
      content: "امضاهای متنی، تصویری، بارکد، QR-Code یا مهر را با دقت در هر صفحه از هر سند پشتیبانی شده وارد کنید. همچنین می‌توانید متادیتای پنهان، مانند EXIF، در تصاویر و بیشتر انواع فایل‌ها را اضافه یا ویرایش کنید. با استفاده از امضاهای دیجیتال اطمینان حاصل کنید که محتوای سند شما دست نخورده باقی مانده است."

    # feature loop
    - title: "جستجو و تأیید امضاها"
      content: "پردازش پس از امضا امکانات زیادی را ارائه می‌دهد. بررسی کنید که آیا اسناد امضا شده شما به درستی پردازش شده‌اند یا خیر. برای کنترل بیشتر، می‌توانید فهرست کاملی از تمام امضاها را از طریق تابع جستجو استخراج کنید."

    # feature loop
    - title: "ویرایش امضاها"
      content: "اکثر انواع امضاها به طور کامل قابل ویرایش هستند. شما می‌توانید متن را تنظیم کنید، عناصر را جابجا کنید، رنگ‌ها را تغییر دهید، اندازه را تغییر دهید و موارد دیگر."

    # feature loop
    - title: "حذف امضاهای زائد"
      content: "راه‌حل ما عملیات کامل CRUD را برای امضاها فراهم می‌کند. در صورت لزوم، می‌توانید انواع مختلف امضاها، از جمله گواهی‌های دیجیتال را از سند خود حذف کنید."
      
  code_samples:
    # code sample loop
    - title: "ایمن‌سازی اسناد با امضاهای دیجیتال"
      content: |
        یاد بگیرید چگونه با استفاده از امضاهای دیجیتال از تغییرات در اسناد جلوگیری کنید.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // فایل را برای امضا کردن ارائه دهید
        using (Signature signature = new Signature("input.pdf"))
        {
            // از یک گواهی دیجیتال معتبر با رمز عبور مربوطه استفاده کنید
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // هر اطلاعات متنی اضافی را مشخص کنید
                Reason = "Security issue",
                Contact = "John Smith",
                Location = "Office D.W.",

                // یک تصویر و گزینه‌های دیگر برای نمای تصویری وارد کنید
                ImageFilePath = "image.png",
                AllPages = true,
                VerticalAlignment = VerticalAlignment.Center,
                HorizontalAlignment = HorizontalAlignment.Left,
                Width = 60,
                Height = 80,

                Margin = new Padding() {  Bottom = 10, Right = 10 }
            };

            // سند ایمن شده را در یک مکان مشخص ذخیره کنید
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```
        {{< /landing/code >}}


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
    title: "به ویژگی‌های برجسته ما نگاهی بیندازید"
    exclude: "digital"
    description: "ما تنوع بالایی از فرمت‌های امضا و عملیات قدرتمند را ارائه می‌دهیم"
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "امضای اسناد در فرمت‌های مختلف"
    exclude: "PDF"
    description: "API .NET به شما این امکان را می‌دهد که بیش از 60 فرمت مختلف را پردازش کنید. شما می‌توانید به‌طور یکپارچه امضاهای متنوعی را در هر صفحه ایجاد و گنجانده، گواهی‌های دیجیتال را برای امنیت محتوا اعمال کرده و به‌طور کارآمد امضاهای موجود را مدیریت کنید."
    items: 
          
        # format loop 1
        - name: "محافظت از PDF"
          format: "PDF"
          link: "/signature/net/digital/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "محافظت از DOCX"
          format: "DOCX"
          link: "/signature/net/digital/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "محافظت از PPTX"
          format: "PPTX"
          link: "/signature/net/digital/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "محافظت از XLSX"
          format: "XLSX"
          link: "/signature/net/digital/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---