



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:02
draft: false
lang: fa
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "تولید کد QR برای فایل‌های JPEG با استفاده از C#"
head_description: "از API GroupDocs.Signature برای تولید کد QR برای فایل‌های JPEG استفاده کنید. کدهای QR را به‌طور یکپارچه در هر صفحه برای بهبود کارایی قرار دهید."

############################# Header ############################
title: "تولید کد QR برای JPEG" 
description: "کدهای بارکد 2 بعدی را با استفاده از داده‌های متنی یا عددی به‌راحتی تولید کنید و آنها را در صفحات و فرمت‌های مختلف از جمله PDF، Word، Excel و غیره با استفاده از GroupDocs.Signature for .NET اعمال کنید."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "آزمون رایگان خود را شروع کنید"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "توانمندی‌های GroupDocs.Signature for .NET را کشف کنید"
    link: "/signature/net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) مجموعه‌ای گسترده از ویژگی‌ها را ارائه می‌دهد که به کاربران قدرت می‌دهد تا انواع امضا را در فرمت‌های پیشرو مستندات تولید و قرار دهند. چه این مستندات PDF، اسناد Word، صفحات Excel، ارائه‌های PowerPoint یا فایل‌های تصویری باشند، می‌توانید مدارک خود را با امضاهای متنی، تصویری، بارکد، QR Code، متادیتا، دیجیتال و مهر تقویت کنید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه در هر جایی از JPEG کد QR تولید و وارد کنیم"
    content: |
      [GroupDocs.Signature](/signature/net/) تولید کد QR در فرمت‌های مختلف محبوب و قرار دادن آنها در صفحات JPEG را تسهیل می‌کند. کتابخانه ما که از بیش از 10 نوع کد QR پشتیبانی می‌کند، می‌تواند به‌صورت یکپارچه در برنامه‌های .NET ادغام شود. مدارک خود را با امضاهای کد QR با استفاده از محصول ما تقویت کنید.
      
      1. فایل JPEG یا جریانی که باید با یک کد QR امضا شود را دریافت کنید.
      2. متن لازم را به QrCodeSignOptions ارائه دهید.
      3. پارامترهای بصری مانند رنگ، موقعیت، اندازه و غیره را سفارشی کنید.
      4. مستند را با کد QR جاسازی شده حفظ کنید.
   
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
        // یک نمونه جدید Signature را با مستند مربوطه ایجاد کنید
        using (Signature signature = new Signature("input.jpeg"))
        {
            // از QrCodeSignOptions برای قرار دادن یک کد QR در مستند استفاده کنید
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // نوع امضا را مشخص کنید و موقعیت آن را در صفحه تعیین کنید
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // مستند را با کد QR یکپارچه شده ذخیره کنید
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "یکپارچگی جامع امضا برای مستندات"
  description: "با استفاده از API GroupDocs.Signature for .NET، کاربران می‌توانند به‌راحتی انواع مختلف امضا را تولید، تغییر دهند، جستجو کنند، اعتبارسنجی کنند و حذف کنند، و جریان‌های کاری مستندات را با دقت بی‌نظیری تسهیل کنند."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضای مستند با انواع امضاهای متعدد"
      content: "GroupDocs.Signature امکان اعمال امضاهای متنی، تصویری، بارکد، QR Code و مهر را در هر فرمت مستند فراهم می‌کند. امضاها می‌توانند دقیقاً در هر صفحه قرار گیرند و متادیتا می‌تواند به‌راحتی از طریق امضاهای متادیتا مدیریت شود. با استفاده از گواهینامه‌های دیجیتال که از ایجاد تغییرات غیرمجاز جلوگیری می‌کنند، از سلامت مدارک خود محافظت کنید."

    # feature loop
    - title: "جستجو و اعتبارسنجی امضا"
      content: "اصالت و دقت امضاهای مستند را از طریق یک فرایند اعتبارسنجی پیشرفته تأیید کنید. به‌راحتی فهرستی دقیق از تمامی امضاهای موجود در یک مستند را برای نظارت جامع بازیابی کنید."

    # feature loop
    - title: "تغییر امضاهای قابل تنظیم"
      content: "امضاهای قبلی را به‌روزرسانی و اصلاح کنید و محتوای، محل، رنگ، اندازه و سایر ویژگی‌ها را مطابق با نیازهای خاص خود تنظیم کنید."

    # feature loop
    - title: "حذف کارآمد امضا"
      content: "مدیریت مستندات خود را با حذف برنامه‌نویسی امضاهای ناخواسته تسهیل کنید. چه در حال کار با گواهینامه‌های دیجیتال باشید یا سایر انواع امضا، حذف به‌سرعت و به‌صورت مؤثر انجام می‌شود."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه کد QR با گزینه‌های مختلف ایجاد کنیم؟"
      content: |
        این مثال نشان می‌دهد که چگونه یک کد QR سفارشی را در یک صفحه JPEG قرار دهیم.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // مستند را که باید امضا شود دریافت کرده و به Signature پاس دهید.
          using (Signature signature = new Signature("input.jpeg"))
          {
              // گزینه‌های کد QR را با متن لازم پیکربندی کنید.
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // موقعیت نسبی کد QR را در صفحه تعیین کنید.
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // فضای خالی امضا را تنظیم کنید.
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // رنگ کد QR را مشخص کنید.
                    ForeColor = Color.Red,

                    // گزینه‌های فونت برای پیام را تعریف کنید.
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // رنگ و براش پس‌زمینه کد QR را سفارشی کنید.
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // کد QR را به مستند جاسازی کنید.
              SignResult result = signature.Sign("output.jpeg", options);
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
            link: "/examples/signature/formats/signature_qrcode.jpeg"
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
    title: "درباره راه‌حل‌های امضا ما بیاموزید"
    exclude: "qrcode"
    description: "بسیاری از انواع امضا و ویژگی‌های عملیاتی را با افتخار ارائه می‌دهیم."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/net/esign/jpeg/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/net/text/jpeg/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/net/image/jpeg/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/net/barcode/jpeg/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/net/qrcode/jpeg/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/net/stamp/jpeg/"
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
    title: "تولید کد QR برای فرمت‌های دیگر مستندات"
    exclude: "JPEG"
    description: "تمام فرمت‌های استاندارد صنعتی را با قابلیت قرار دادن کد QR از طریق API .NET تقویت کنید. اطلاعات حیاتی را به کدهای بارکد 2 بعدی ذخیره و کدگذاری کنید تا به‌راحتی اسکن و از آن بازیابی شود."
    items: 
          
        # format loop 1
        - name: "QR-Code برای PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "QR-Code برای DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "QR-Code برای JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "QR-Code برای PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "QR-Code برای XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---