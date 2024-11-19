



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:32
draft: false
lang: fa
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "جستجوی امضای الکترونیکی در DOCX با C#"
head_description: "از امکانات API GroupDocs.Signature for .NET برای جستجوی امضای تعبیه شده در PDFها، Word، Excel، ارائه‌ها و تصاویر استفاده کنید."

############################# Header ############################
title: "جستجوی امضای دیجیتال در DOCX" 
description: "لیستی جامع از امضاهای الکترونیکی تعبیه شده در قالب‌های مختلف مانند PDFها، Word، Excel، ارائه‌ها و تصاویر را به صورت یکپارچه استخراج کنید که همه توسط GroupDocs.Signature for .NET پشتیبانی می‌شوند."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان خود را آغاز کنید"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "امکانات GroupDocs.Signature for .NET را بررسی کنید"
    link: "/signature/net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) قابلیت‌های پیشرفته‌ای برای امضای اسناد دیجیتال ارائه می‌دهد. با پشتیبانی از بیش از 60 فرمت فایل، از جمله PDFها، اسناد MS Office، تصاویر و فایل‌های ZIP، به شما امکان می‌دهد امضاهای مختلف مانند متن، تصاویر، بارکدها، کدهای QR، گواهی‌های دیجیتال و مهرها را اضافه، جستجو، تأیید، تغییر یا حذف کنید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه امضاهای DOCX را با استفاده از C# جستجو کنیم"
    content: |
      [GroupDocs.Signature](/signature/net/) یک موتور قدرتمند برای یافتن امضاهای دیجیتال در فایل‌های DOCX ارائه می‌دهد. توسعه‌دهندگان .NET می‌توانند به راحتی برنامه‌های خود را با راه‌حل ما تقویت کنند.
      
      1. مسیر فایل DOCX را برای جستجوی امضا تأمین کنید.
      2. از SearchOptions برای بهبود معیارهای جستجو استفاده کنید.
      3. متد جستجو را فراخوانی کنید تا نتایج را بازیابی کنید.
      4. لیست امضاهای شناسایی شده را ارزیابی کنید.
   
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
        // یک شی Signature را با مسیر سند مشخص شده مقداردهی اولیه کنید
        using (Signature signature = new Signature("input.docx"))
        {
            // یک نمونه از TextSearchOptions را ایجاد کنید تا تمام صفحات را در بر بگیرد
            TextSearchOptions options = new TextSearchOptions()
            {
                AllPages = true
            };

            // یک جستجو را برای شناسایی هر امضای مبتنی بر متن در سند انجام دهید
            List<TextSignature> signatures = signature.Search<TextSignature>(options);
            Console.WriteLine($"\nSource document contains following text signature(s).");

            // یک لیست از امضاهای شناسایی شده برای بررسی دقیق جمع آوری کنید               
            foreach (TextSignature textSignature in signatures)
            {
                Console.WriteLine($"Found Text signature at page {textSignature.PageNumber} with type
                    [{textSignature.SignatureImplementation}] and text '{textSignature.Text}'.");
            }
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "اکوسیستم کامل امضای سند"
  description: "یک راه حل پیشرفته و دارای امکانات زیاد برای امضای اسناد را کشف کنید که به طور خاص برای بهبود و تأمین امنیت اسناد شما با انواع مختلف امضا در قالب‌های گوناگون طراحی شده است."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "جستجو و مدیریت امضا"
  features:
    # feature loop
    - title: "امضا و تأمین امنیت اسناد تجاری"
      content: "امضاهای دیجیتال را به هر نقطه‌ای از سند اضافه کنید. GroupDocs.Signature از مجموعه‌ای از انواع امضاها، از جمله متن، تصاویر، بارکدها، متادیتا، مهرها و گواهی‌های دیجیتال پشتیبانی می‌کند و اصالت و انطباق سند را تضمین می‌کند."

    # feature loop
    - title: "مدیریت جامع امضاها"
      content: "پس از امضا، از ویژگی جستجو برای بازیابی تمام امضاهای تعبیه شده استفاده کنید. امضاها را در صورت نیاز تغییر یا حذف کنید و کنترل کاملی بر یکپارچگی سند داشته باشید."

    # feature loop
    - title: "حفاظت از یکپارچگی سند شما"
      content: "از ابزارهای پیشرفته برای مدیریت متادیتای پنهان تعبیه‌شده در اسناد استفاده کنید. ورودهای متادیتا را اضافه یا حذف کنید و گواهی‌های دیجیتال شرکتی را برای جلوگیری از ویرایش‌های غیرمجاز و اطمینان از اصالت سند اعمال کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "جستجوی امضاهای تصویری"
      content: |
        این مثال فرآیند شناسایی یک امضای تصویری در یک سند مشخص را نشان می‌دهد.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // سند منبع را به عنوان یک آرگومان به سازنده ارائه دهید
          using (Signature signature = new Signature("input.docx"))
          {
              // برای هر امضای از نوع متن جستجو کنید
              List<ImageSignature> signatures = signature.Search<ImageSignature>(SignatureType.Image);
              Console.WriteLine($"\nSource document contains following image signature(s).");

              // نتایج را با ویژگی‌های دقیق امضاهای شناسایی شده ارائه دهید
              foreach (ImageSignature imageSignature in signatures)
              {
                    Console.WriteLine($"Found Image signature at page {imageSignature.PageNumber} 
                    and size {imageSignature.Size}.");
              }
          }
          ```
        platform: "net"
        copy_title: "کپی"
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
    title: "عملکردهای اصلی"
    exclude: "search"
    description: "API ما انعطاف‌پذیری وسیعی را ارائه می‌دهد و به کاربران این امکان را می‌دهد که اسناد را امضا کرده و عملیات جامع پس از امضا، مانند جستجو، تأیید و تغییر امضاها را انجام دهند."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "بازیابی امضاها از انواع فرمت‌های فایل"
    exclude: "DOCX"
    description: "API GroupDocs.Signature for .NET به شما امکان می‌دهد امضاها را از مجموعه وسیعی از انواع اسناد استخراج و مدیریت کنید. به راحتی امضاهای تعبیه شده از تمام فرمت‌های اصلی فایل را برای تجزیه و تحلیل یا پردازش بیشتر بازیابی کنید."
    items: 
          
        # format loop 1
        - name: "جستجوی امضاها در PDF"
          format: "PDF"
          link: "/signature/net/search/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "یافتن امضاها در DOCX"
          format: "DOCX"
          link: "/signature/net/search/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "یافتن امضاها در PPTX"
          format: "PPTX"
          link: "/signature/net/search/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "جستجوی امضاها در XLSX"
          format: "XLSX"
          link: "/signature/net/search/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---