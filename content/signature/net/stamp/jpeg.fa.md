



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:06
draft: false
lang: fa
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "مهرهای گرد و مربع JPEG با استفاده از C#"
head_description: "از GroupDocs.Signature for .NET برای تولید و درج مهرهای شخصی‌سازی شده در فایل‌های JPEG استفاده کنید."

############################# Header ############################
title: "تولید مهر برای فایل‌های JPEG" 
description: "با استفاده از GroupDocs.Signature for .NET، مهرهای سفارشی را به طور یکپارچه در هر بخشی از اسناد خود ادغام کنید و انعطاف‌پذیری گسترده‌ای برای جایگذاری و پیکربندی مهرها مطابق با نیازهای کسب‌وکار خود ارائه دهید."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان خود را بگیرید"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "مروری بر GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) ابزاری چندمنظوره است که امکان درج انواع امضا به‌ویژه مهرهای قابل تنظیم را در اسناد فراهم می‌آورد. این ابزار از بیش از 60 فرمت فایل، از جمله PDF و اسناد Word تا تصاویر و فایل‌های ZIP پشتیبانی می‌کند. شما می‌توانید اسناد خود را با متن، تصویر، بارکد، متادیتا، گواهی‌های دیجیتال و مهرها غنی‌سازی کنید. علاوه بر این، شما کنترل کاملی برای جستجو، تأیید، تغییر یا حذف هر نوع امضایی که به فایل‌های خود اضافه کرده‌اید، دارید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه مهر را به JPEG با استفاده از C# درج کنیم"
    content: |
      [GroupDocs.Signature](/signature/net/) دارای قابلیت قوی ایجاد مهر است که برای بهبود برنامه‌های .NET ایده‌آل به حساب می‌آید. از این ابزار برای طراحی و پیاده‌سازی مهرهای بسیار سفارشی در صفحات سند خود استفاده کنید.
      
      1. سند JPEG که می‌خواهید مهر کنید را تهیه کنید.
      2. از StampSignOptions برای تنظیم دقیق تمام پارامترهای لازم استفاده کنید.
      3. چندین خط مهر را بر اساس نیازهای خود اضافه کنید.
      4. مهر پیکربندی شده را اعمال کرده و سند تغییر یافته را ذخیره کنید.
   
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
        // مسیر سند را با نمونه Signature ادغام کنید
        using (Signature signature = new Signature("input.jpeg"))
        {
            // StampSignOptions را با محتوای امضای مورد نیاز راه‌اندازی کنید
            StampSignOptions options = new StampSignOptions();
            options.Height = 180;
            options.Width = 180;

            // یک یا چند خط مهر را ادغام کنید
            options.OuterLines.Add(
                new StampLine()
                {
                    Text = "* The Best Company *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 22,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );

            // سند را با مهر اعمال شده حفظ کنید
            SignResult result = signature.Sign("output.jpeg", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "از امضاها برای تأمین و تقویت یکپارچگی اسناد استفاده کنید"
  description: "با کتابخانه GroupDocs.Signature for .NET، می‌توانید به‌طور یکپارچه قابلیت امضا را به اسناد خود اضافه کنید. به راحتی مهرهای سفارشی و سایر انواع امضا را اضافه، تغییر، تأیید یا حذف کنید و انعطاف‌پذیری و دقت را برای مدیریت ایمن اسناد ارائه دهید."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "امضاهای مهر با قدرت GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضای جامع اسناد"
      content: "با قرار دادن امضاها شامل متن، تصویر، بارکد، کد QR و مهرها در هر موقعیت یا صفحه از فایل، اسناد خود را متنوع‌تر کنید. علاوه بر این، متادیتای تعبیه شده را مدیریت کرده و گواهی‌های دیجیتال را برای جلوگیری از تغییرات غیرمجاز اعمال کنید."

    # feature loop
    - title: "جستجو و تأیید امضا به‌صورت کارآمد"
      content: "پس از امضا، صحت و یکپارچگی امضاهای اسناد را تأیید کنید. از عملکرد جستجوی پیشرفته برای بازیابی و مدیریت تمامی داده‌های امضا موجود در سند استفاده کنید."

    # feature loop
    - title: "تغییر و سفارشی‌سازی امضاها"
      content: "امضاهای قبلاً درج شده را به‌راحتی تغییر دهید. چه بخواهید محتوا، موقعیت، اندازه یا رنگ را تغییر دهید، راه‌حل ما انعطاف‌پذیری کاملی برای تغییر امضاها ارائه می‌دهد."

    # feature loop
    - title: "به‌راحتی امضاها را حذف کنید"
      content: "زمانی که نیاز به حذف امضاها دارید، GroupDocs.Signature for .NET مجموعه کاملی از ابزارها را برای حذف هر نوع امضا，包括 مهرها، گواهی‌های دیجیتال و غیره ارائه می‌دهد و اطمینان می‌دهد که اسناد شما به‌روز و مطابق قوانین باقی بمانند."
      
  code_samples_ext:
    # code sample ext loop
    - title: "پیاده‌سازی مهرهای سفارشی در اسناد"
      content: |
        بیاموزید چگونه مهرهای سفارشی با جزئیات متنی مهم را در اسناد خود ایجاد و ادغام کنید.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // سند را برای مهر کردن فراهم کنید
          using (Signature signature = new Signature("input.jpeg"))
          {
              // گزینه‌های مهر را با تنظیمات دلخواه راه‌اندازی کنید
              StampSignOptions options = new StampSignOptions()
              {
                    // ابعاد و موقعیت مهر را در صفحه تعریف کنید
                    Height = 200,
                    Width = 200,
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,
                    AllPages = true
              };

              // خطوط دایره‌ای خارجی را همراه با متن ادغام کنید
              options.OuterLines.Add(
                    new StampLine()
                    {
                        Text = "* The best  choice *",
                        TextRepeatType = StampTextRepeatType.FullTextRepeat,
                        Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                        Height = 22,
                        TextBottomIntent = 6,
                        TextColor = Color.WhiteSmoke,
                        BackgroundColor = Color.DarkSlateBlue
                    }
              );

              // در صورت نیاز خطوط مربع داخلی را ادغام کنید
              options.InnerLines.Add(
                    new StampLine()
                    { 
                        Text = "Company #1",
                        TextColor = Color.MediumVioletRed,
                        Font = new SignatureFont() { Size = 20, Bold = true },
                        Height = 40
                    }
              );

              // مستند را با مهر نهایی و ذخیره کنید
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "امکانات اصلی را کشف کنید"
    exclude: "stamp"
    description: "یک دامنه وسیع از گزینه‌ها را برای ایجاد، مدیریت و حذف انواع مختلف امضاها کشف کنید و کنترل جامع بر روی جریان‌های کاری اسناد خود داشته باشید."
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
    title: "استفاده از مهرها در قالب‌های مختلف اسناد"
    exclude: "JPEG"
    description: "API GroupDocs.Signature به شما این امکان را می‌دهد که مهرها را در بیش از 60 نوع فایل استاندارد صنعتی درج کنید. به‌راحتی مهرهای سفارشی را در هر مکانی از اسناد خود اعمال کنید و امکان ردیابی و شخصی‌سازی بهتر اسناد را فراهم آورید."
    items: 
          
        # format loop 1
        - name: "مهر زدن PDF"
          format: "PDF"
          link: "/signature/net/stamp/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "مهر زدن DOCX"
          format: "DOCX"
          link: "/signature/net/stamp/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "مهر زدن JPEG"
          format: "JPEG"
          link: "/signature/net/stamp/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "مهر زدن PPTX"
          format: "PPTX"
          link: "/signature/net/stamp/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "مهر زدن XLSX"
          format: "XLSX"
          link: "/signature/net/stamp/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---