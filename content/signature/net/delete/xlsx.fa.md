



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:19
draft: false
lang: fa
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "حذف امضاها از XLSX با استفاده از C#"
head_description: "حذف امضاهای دیجیتال، بارکد، متن، تصویر و متادیتا از اسناد امضا شده XLSX می‌تواند به سادگی با استفاده از GroupDocs.Signature for .NET انجام شود."

############################# Header ############################
title: "حذف امضاها از XLSX به صورت کارآمد" 
description: "فراتر از امضای اسناد تجاری، راه‌حل ما ابزارهای جامعی را برای شناسایی و حذف انواع مختلف امضاها با استفاده از GroupDocs.Signature for .NET ارائه می‌دهد."
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
    title: "مروری بر GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) یک ابزار امضای قدرتمند است که اضافه کردن انواع مختلف امضا از جمله متن و تصویر تا بارکد، گواهی‌های دیجیتال و مهرها را تسهیل می‌کند. این راه‌حل از بیش از 60 فرمت فایل—شامل PDF، MS Office، تصاویر، ZIP و دیگر فرمت‌های تجاری رایج—پشتیبانی می‌کند و انعطاف‌پذیری در مدیریت اسناد را فراهم می‌آورد. علاوه بر این، امضاهای اعمال‌شده به راحتی قابل شناسایی، تأیید، تغییر یا حذف هستند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه امضاهای الکترونیکی را از XLSX با استفاده از C# حذف کنیم"
    content: |
      [GroupDocs.Signature](/signature/net/) کار را برای توسعه‌دهندگان .NET در حذف امضاهای الکترونیکی از فایل‌های XLSX با پیاده‌سازی چند مرحله ساده تسهیل می‌کند.
      
      1. مسیر فایل XLSX را به نمونه‌ای از کلاس Signature ارائه دهید.
      2. متد جستجو را برای بازیابی تمام امضاها در سند فراخوانی کنید.
      3. یک یا چند مورد از امضاهای بازیابی شده را حذف کنید.
      4. نتایج پردازش سند را بررسی کنید.
   
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
        // سند حاوی امضاها را به نمونه Signature منتقل کنید
        using (Signature signature = new Signature("input.xlsx"))
        {
            // امضاهای دیجیتال موجود در سند را بازیابی کنید
            DigitalSearchOptions options = new DigitalSearchOptions();

            List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

            // اولین امضای دیجیتالی شناسایی شده را حذف کنید
            if(signatures.Count > 0)
            {
                DigitalSignature digitalSignature = signatures[0];
                bool result = signature.Delete(digitalSignature);

                // اولین امضای دیجیتالی شناسایی شده را حذف کنید
                if(result)
                {
                    Console.WriteLine($"Digital signature in XLSX was deleted successfully");
                }
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "بهینه‌سازی مدیریت اسناد با ابزارهای پیشرفته امضا"
  description: "GroupDocs.Signature for .NET به‌دقت طراحی شده است تا امضا کردن و پردازش فرمت‌های فایل تجاری را بهبود بخشد و افزودن، تغییر، تأیید یا حذف امضاها را امکان‌پذیر سازد."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "ویژگی‌های متنوع GroupDocs.Signature را کاوش کنید"
  features:
    # feature loop
    - title: "امضای اسناد"
      content: "به سادگی امضاهای متنی، تصویری، بارکدی، QR کدی یا علامت‌دار را در هر صفحه از اسناد پشتیبانی شده قرار دهید. همچنین، از متادیتای پنهان مانند EXIF در تصاویر استفاده کنید یا با گواهی‌های دیجیتال از یکپارچگی سند محافظت نمایید و از تغییرات غیرمجاز جلوگیری کنید."

    # feature loop
    - title: "جستجو و تأیید امضاها"
      content: "از ابزارهای ما برای اطمینان از اصالت امضاها در اسناد خود استفاده کنید. جستجوهای عمیق انجام دهید تا لیستی کامل از تمام امضاها را بازیابی کنید و مدیریت جامع اسناد را تضمین کنید."

    # feature loop
    - title: "تغییر امضاها"
      content: "امضاهای قبلاً اضافه شده را با تنظیم متن، repositioning یا تغییر رنگ‌ها به راحتی اصلاح کنید تا نیازهای خاص خود را برآورده سازید."

    # feature loop
    - title: "حذف امضاها"
      content: "راه‌حل ما قابلیت‌های کامل CRUD را برای امضاها ارائه می‌دهد و به شما امکان می‌دهد انواع مختلف امضاها را از اسناد خود به طور کارآمد حذف کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "یادآوری همه امضاهای بارکدی"
      content: |
        بیاموزید که چگونه می‌توان تمام امضاهای بارکدی موجود در یک سند را حذف کرد.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // یک سند حاوی امضاهای بارکدی ارائه دهید
          using (Signature signature = new Signature("input.xlsx"))
          {
              // تمام امضاهای بارکدی را حذف کنید
              DeleteResult result = signature.Delete(SignatureType.Barcode);

              // نتیجه فرآیند حذف را ارزیابی کنید
              if (result.Succeeded.Count > 0)
              {
                  Console.WriteLine("Following XLSX barcode signatures were deleted:");                        
                  int number = 1;
                  foreach (BarcodeSignature temp in result.Succeeded)
                  {
                      Console.WriteLine($"Signature #{number++}: Type: {temp.SignatureType} 
                            Id:{temp.SignatureId}, Text: {temp.Text}");
                  }
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
    title: "مشاهده ویژگی‌های برجسته ما"
    exclude: "delete"
    description: "مانند همیشه، تجربه گسترده‌ای از انواع امضاهای پشتیبانی شده و عملیات را به شما ارائه می‌دهیم."
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
    title: "حذف امضاها در چندین فرمت فایل"
    exclude: "XLSX"
    description: "GroupDocs.Signature for .NET برای تسهیل حذف امضاها از یک دامنه وسیع و بیش از 60 فرمت فایل طراحی شده است و سازگاری و کارآیی وسیعی را تضمین می‌کند."
    items: 
          
        # format loop 1
        - name: "حذف امضاهای PDF"
          format: "PDF"
          link: "/signature/net/delete/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "حذف امضاهای DOCX"
          format: "DOCX"
          link: "/signature/net/delete/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "حذف امضاهای PPTX"
          format: "PPTX"
          link: "/signature/net/delete/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "حذف امضاهای XLSX"
          format: "XLSX"
          link: "/signature/net/delete/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---