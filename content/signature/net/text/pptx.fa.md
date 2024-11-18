



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:55
draft: false
lang: fa
format: Pptx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ایجاد امضاهای متنی برای PPTX با استفاده از برنامه‌های C#"
head_description: "قدرت API C# را برای وارد کردن امضاهای متنی در پرونده‌های PPTX به کار بگیرید و از انواع فرمت‌ها مانند PDF، Word، Excel، ارائه‌ها، تصاویر و ZIP پشتیبانی کنید."

############################# Header ############################
title: "ادغام روان امضاهای متنی در PPTX" 
description: "با استفاده از GroupDocs.Signature for .NET، امضاهای متنی سفارشی را به راحتی به مدارک تجاری خود اضافه کنید. با قابلیت‌های متنوع سفارشی‌سازی امضا، فرآیندهای سازمانی را بهینه کنید."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "همین امروز رایگان امتحان کنید"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "حل‌وفصل GroupDocs.Signature for .NET را کشف کنید"
    link: "/signature/net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) یک پلتفرم پیشرفته برای وارد کردن امضاهای متنی به شدت قابل سفارشی‌سازی ارائه می‌دهد و جریان‌های کاری اسناد شما را ساده می‌سازد. محتوای امضاهای متنی و ویژگی‌های بصری آن‌ها را مطابق نیاز خود سفارشی کنید و آن‌ها را به‌صورت یکسان در صفحات مختلف به کار ببرید تا مدیریت اسناد را ارتقا بخشید و کارآیی عملیاتی را افزایش دهید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه امضاهای متنی را به PPTX با استفاده از C# ایجاد و اضافه کنیم"
    content: |
      [GroupDocs.Signature](/signature/net/) ادغام امضاهای متنی را در پرونده‌های PPTX در برنامه‌های .NET تسهیل می‌کند. قابلیت‌های محصول خود را به سرعت با راه‌حل‌های جامع ما افزایش دهید.
      
      1. پرونده PPTX را به‌عنوان پارامتر به سازنده کلاس Signature منتقل کنید.
      2. TextSignOptions را با متن امضای مورد نیاز ایجاد کنید.
      3. ویژگی‌های بصری برای امضا را تعریف کنید.
      4. امضای متنی را به هر صفحه مشخص از سند ادغام کنید.
   
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
        // ابتدا Signature را با مسیر سند راه‌اندازی کنید
        using (Signature signature = new Signature("input.pptx"))
        {
            // یک نمونه از TextSignOptions با متن امضای مورد نظر ایجاد کنید
            TextSignOptions options = new TextSignOptions("Approved")
            {
                // رنگ متن و ویژگی‌های فونت را پیکربندی کنید
                ForeColor = Color.Red,
                Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" }
            };

            // امضای متنی را در سند ادغام کنید
            SignResult result = signature.Sign("output.pptx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "مدیریت کامل امضاهای متنی"
  description: "GroupDocs.Signature for .NET با افزودن امضاهای متنی سفارشی در فرمت‌های فایل محبوب، جریان‌های کاری اسناد را تقویت می‌کند. به راحتی ظاهر، موقعیت و محتوای این امضاها را برای مطابق‌سازی با نیازهای خاص خود مدیریت کنید."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "ویژگی‌های GroupDocs.Signature را کاوش کنید"
  features:
    # feature loop
    - title: "امضاهای مستند متنوع"
      content: "امضاهای مختلفی از جمله متن، تصاویر، بارکدها، کدهای QR و تمبرها را به هر صفحه‌ای از اسناد پشتیبانی شده اضافه کنید. از متاداده برای گنجاندن محتوای مخفی استفاده کنید و در عین حال اطلاعات حساس را با استفاده از گواهی‌های دیجیتال محافظت کنید."

    # feature loop
    - title: "جستجو و تأیید امضا"
      content: "با استفاده از ابزارهای قوی تأیید امضا، از اعتبار و یکپارچگی اسناد امضا شده خود اطمینان حاصل کنید. جستجوهایی انجام دهید تا فهرستی جامع از تمامی امضاها در یک مدرک برای تحلیل بیشتر استخراج کنید."

    # feature loop
    - title: "به‌روزرسانی یا حذف امضاها"
      content: "محتوا، ویژگی‌های بصری یا موقعیت امضاهای قبلاً وارد شده را به راحتی تغییر دهید. در صورت لزوم، امضاهای نامناسب را حذف کنید تا محتویات اسناد دقیق و مرتبط باقی بماند."

    # feature loop
    - title: "امضاهای متنی تخصصی"
      content: "امضاهای متنی خاص مانند واترمارک‌ها برای اسناد Word یا برچسب‌ها برای PDFها را پیاده‌سازی کنید تا لایه‌ای اضافی از سفارشی‌سازی و کنترل را فراهم آورید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "وارد کردن امضاهای متنی در اسناد"
      content: |
        یاد بگیرید چگونه امضاهای متنی را به اسناد تجاری اضافه کنید تا فرآیندها را تسهیل کنید.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // مدرکی که قرار است امضا شود را انتخاب کنید
          using (Signature signature = new Signature("input.pptx"))
          {
              // گزینه‌های متنی را با محتوای مشخص کنید
              TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025")
              {
                    // ابعاد و موقعیت امضا را در صفحه تعیین کنید
                    Left = 100,
                    Top = 180,
                    Width = 230,
                    Height = 30,

                    // برای امضاها از لایه‌های حاشیه‌ای از لبه‌های صفحه استفاده کنید
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // رنگ متن و سبک فونت را سفارشی کنید
                    ForeColor = Color.OrangeRed,
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // برای امضای متنی یک حاشیه اضافه کنید
                    Border = new Border()
                    {
                        Color = Color.OrangeRed,
                        DashStyle = DashStyle.Dash,
                        Transparency = 0.5,
                        Visible = true,
                        Weight = 2
                    },

                    // در صورت لزوم، گزینه سفارشی‌سازی پس‌زمینه را اعمال کنید
                    Background = new Background()
                    {
                        Color = Color.LightYellow,
                        Transparency = 0.8
                    },

                    // به‌اختیار، متن را به‌عنوان تصویری ذخیره کنید تا از سازگاری اطمینان حاصل کنید
                    SignatureImplementation = TextSignatureImplementation.Image
              };

              // مدرک را با امضای متنی ادغام شده ذخیره کنید
              SignResult result = signature.Sign("output.pptx", options);
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
            link: "/examples/signature/formats/signature_text.pptx"
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
    title: "امکانات پیشرفته و گزینه‌های امضا"
    exclude: "text"
    description: "API ما از مدیریت کامل چرخه زندگی هفت نوع امضا پشتیبانی می‌کند و امکانات جامعی برای مدیریت، تأیید و سفارشی‌سازی امضاهای شما ارائه می‌دهد."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/net/esign/pptx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/net/text/pptx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/net/image/pptx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/net/barcode/pptx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/net/qrcode/pptx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/net/digital/pptx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/net/stamp/pptx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/net/search/pptx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/net/verify/pptx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/net/modify/pptx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/net/delete/pptx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ورود امضاهای متنی در فرمت‌های فایل متنوع"
    exclude: "PPTX"
    description: "با API .NET، می‌توانید امضاهای متنی را به انواع مختلفی از اسناد Office اضافه کنید. با افزودن امضاهای متنی که هم عملکرد و هم امنیت را افزایش می‌دهند، کنترل کامل بر چرخه زندگی اسناد خود داشته باشید."
    items: 
          
        # format loop 1
        - name: "امضای متنی PDF"
          format: "PDF"
          link: "/signature/net/text/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "امضای متنی DOCX"
          format: "DOCX"
          link: "/signature/net/text/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "امضای متنی JPEG"
          format: "JPEG"
          link: "/signature/net/text/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "امضای متنی PPTX"
          format: "PPTX"
          link: "/signature/net/text/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "امضای متنی XLSX"
          format: "XLSX"
          link: "/signature/net/text/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---