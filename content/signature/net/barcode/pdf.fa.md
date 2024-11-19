



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:25
draft: false
lang: fa
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "تولید بارکد برای PDF با استفاده از API C#"
head_description: "امضای بارکد و امن‌سازی اسناد PDF با استفاده از C# تنها با چند خط کد. از GroupDocs.Signature برای امضای طیف وسیعی از فرمت‌های فایل استفاده کنید."

############################# Header ############################
title: "تولید بارکد برای اسناد PDF" 
description: "از GroupDocs.Signature for .NET برای قرار دادن بارکد در هر قسمتی از اسناد تجاری خود استفاده کنید. API ما گزینه‌های سفارشی‌سازی گسترده‌ای برای امضاهای بارکدی ارائه می‌دهد."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "رایگان دانلود کنید"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "مروری بر GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) یک راه‌حل پیچیده برای امضای اسناد است که از طیف وسیعی از انواع امضاها حمایت می‌کند، از جمله متن، تصاویر، بارکدها، گواهینامه‌های دیجیتال و مهرها. این ابزار سازگار با بیش از 60 فرمت فایل—مانند PDF، MS Office، تصاویر، فایل‌های ZIP و غیره—این امکان را به شما می‌دهد که نه تنها امضاها را اعمال کنید بلکه آنها را جستجو، تأیید، ویرایش یا در صورت نیاز حذف کنید.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل تولید و جاسازی بارکد در فایل PDF"
    content: |
      [GroupDocs.Signature](/signature/net/) تولید بارکدها در فرمت‌های محبوب و قرار دادن آنها در صفحات PDF را تسهیل می‌کند. با پشتیبانی از بیش از 60 نوع بارکد، برنامه‌های .NET می‌توانند به راحتی با قابلیت‌های امضای بارکد با ادغام کتابخانه ما تقویت شوند.
      
      1. فایل یا جریان PDF را برای پردازش تأمین کنید.
      2. متن بارکد را به شی BarcodeSignOptions منتقل کنید.
      3. گزینه‌های بارکد مانند موقعیت، اندازه و غیره را تنظیم کنید.
      4. فایل را با بارکد جدید ذخیره کنید.
   
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
        // یک شی Signature جدید با مسیر سند ایجاد کنید
        using (Signature signature = new Signature("input.pdf"))
        {
            // از BarcodeSignOptions برای افزودن بارکد به سند استفاده کنید
            BarcodeSignOptions options = new BarcodeSignOptions("Business data")
            {
                // نوع بارکد و ویژگی‌های اضافی را پیکربندی کنید
                EncodeType = BarcodeTypes.Code128,
                Left = 50,
                Top = 150
            };

            // فایل امضا شده را ذخیره کنید
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "اسناد خود را با قابلیت‌های امضای پیشرفته تقویت و محافظت کنید"
  description: "کتابخانه GroupDocs.Signature for .NET برای تسهیل امضای جامع اسناد و پردازش در فرمت‌های پرکاربرد طراحی شده است. به راحتی می‌توانید انواع مختلف امضاها را اضافه، ویرایش، تأیید یا حذف کنید."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضای همه‌جانبه اسناد"
      content: "به طور کارآمد هر صفحه‌ای را در اسناد پشتیبانی شده با استفاده از متن، تصاویر، بارکدها، کدهای QR یا مهرها امضا کنید. همچنین، می‌توانید متاداده‌های پنهان مانند داده‌های EXIF در تصاویر را جاسازی کنید، یا محتوای سند خود را در برابر تغییرات غیرمجاز با استفاده از گواهی‌های دیجیتال محافظت کنید."

    # feature loop
    - title: "جستجو و تأیید امضا به طور جامع"
      content: "ابزار ما عملکرد قدرتمند برای کار با اسناد امضا شده ارائه می‌دهد. با تأیید امضاها، از یکپارچگی اسناد خود اطمینان حاصل کرده و به راحتی لیست جامعی از تمام امضاها در یک سند را با استفاده از ویژگی جستجو بازیابی کنید."

    # feature loop
    - title: "ویرایش امضاها به آسانی"
      content: "تقریباً تمام امضاهای قبلاً اعمال شده قابلیت ویرایش دارند. به راحتی متن را به‌روزرسانی کنید، موقعیت را تغییر دهید یا رنگ‌ها را برای پاسخگویی به نیازهای خود تنظیم کنید."

    # feature loop
    - title: "حذف امضا به طور کارآمد"
      content: "رویکرد ما به طور کامل از عملیات CRUD برای امضاها پشتیبانی می‌کند و به شما امکان می‌دهد هر امضای ناخواسته یا قدیمی را به سرعت از اسناد خود حذف کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه یک امضای بارکد تولید کنیم"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توانید یک بارکد سفارشی را در صفحات سند PDF جاسازی کنید.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.pdf"))
          {
              // گزینه‌های امضا را با متن دلخواه فرمول‌بندی کنید
              BarcodeSignOptions options = new BarcodeSignOptions("Accepted")
              {
                  EncodeType = BarcodeTypes.Code39FullASCII,

                  // موقعیت نسبی بارکد را در صفحه تعیین کنید
                  VerticalAlignment = Domain.VerticalAlignment.Top,
                  HorizontalAlignment = Domain.HorizontalAlignment.Left,

                  // فاصله بارکد را از لبه صفحه مشخص کنید
                  Margin = new Padding() { Top = 180, Right = 20 },

                  // رنگ میله‌ها را مشخص کنید
                  ForeColor = Color.Red,

                  // سبک فونت پیام را انتخاب کنید
                  Font = new SignatureFont { Size = 12, FamilyName = "Arial" },

                  // موقعیت پیام را مشخص کنید
                  CodeTextAlignment = CodeTextAlignment.Above
              };

              // سند را امضا کرده و ذخیره کنید
              SignResult result = signature.Sign("output.pdf", options);
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
            link: "/examples/signature/formats/signature_barcode.pdf"
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
    title: "ویژگی‌های اصلی ما را کشف کنید"
    exclude: "barcode"
    description: "ما انتخاب گسترده‌ای از گزینه‌های امضا و عملیات را ارائه می‌دهیم."
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
    title: "امضا دادن بر روی انواع فرمت‌ها"
    exclude: "PDF"
    description: "API .NET ما از امضای بیش از 60 فرمت مختلف پشتیبانی می‌کند. به راحتی می‌توانید انواع مختلف امضاها را در هر صفحه یا در هر موقعیت دلخواه در اسناد خود قرار دهید."
    items: 
          
        # format loop 1
        - name: "اضافه کردن بارکد به PDF"
          format: "PDF"
          link: "/signature/net/barcode/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "اضافه کردن بارکد به DOCX"
          format: "DOCX"
          link: "/signature/net/barcode/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "اضافه کردن بارکد به JPEG"
          format: "JPEG"
          link: "/signature/net/barcode/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "اضافه کردن بارکد به PPTX"
          format: "PPTX"
          link: "/signature/net/barcode/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "اضافه کردن بارکد به XLSX"
          format: "XLSX"
          link: "/signature/net/barcode/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---