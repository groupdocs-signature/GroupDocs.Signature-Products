---
############################# Static ############################
layout: "family"
date:  2024-07-25T14:25:12
draft: false

product: "Signature"
product_tag: "signature"

lang: fa

############################# Head ############################
head_title: "C#.NET، Java، برنامه های امضای دیجیتال Node.js"
head_description: "امضاهای الکترونیکی را در برنامه‌های NET، جاوا یا Node.js با GroupDocs.Signature ادغام کنید. فرمت های رایج اسناد تجاری را امضا کنید."

############################# Header ############################
title: "راه حل امضای الکترونیکی سند"
description:  |
  با استفاده از APIهای انعطاف پذیر و راه حل های مبتنی بر برنامه برای برنامه نویسان و کاربران نهایی، اسناد و تصاویر دیجیتال را در هر پلتفرمی امضا کنید.

  امضاهای اضافه شده قبلی را با استفاده از روش های پیشرفته جستجو و اصلاح کنید.

  از اسناد در برابر تغییرات با گواهی های دیجیتال محافظت کنید و ابرداده های پنهان را کنترل کنید.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "پلتفرم خود را انتخاب کنید"
  title: "استقلال سکو"
  description: "کتابخانه GroupDocs.Signature سیستم عامل ها و چارچوب های زیر را پشتیبانی می کند:"
  details_link_title: "بیشتر بدانید"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> هر ویرایشگر متن دیگری
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "ویژگی های کلیدی GroupDocs.Signature"
  description: "راه حل ما برای افزودن انواع مختلف امضا به فرمت های رایج اسناد و فایل طراحی شده است. فرآیندهای کسب و کار خود را به راحتی غنی کنید."

  items:
    # items loop
    - icon: "additional"
      title: "داده های خود را با امضا غنی کنید"
      content: "متن، تصاویر، واترمارک و غیره را به اسناد تجاری خود اضافه کنید."

    # items loop
    - icon: "protect"
      title: "از محتوای اسناد محافظت کنید"
      content: "با مهر و موم کردن با گواهی دیجیتال، تغییر سند را ممنوع کنید."

    # items loop
    - icon: "search"
      title: "داده ها و بارکدهای پنهان را اضافه کنید"
      content: "از ابرداده برای ذخیره اطلاعات نامرئی یا قرار دادن بارکدهای سفارشی در صفحات استفاده کنید."

    # items loop
    - icon: "manipulate"
      title: "دستکاری امضاها"
      content: "جستجو، به روز رسانی، یا حذف همه امضاهایی که قبلا اضافه شده اند."

############################# Code samples ############################
code_samples:
  enable: true
  title: "با استفاده از امضا از فایل های خود محافظت کنید"
  description: "نمونه کد GroupDocs.Signature"
  items:
    # code sample loop
    - title: "کد QR را ایجاد و اضافه کنید"
      content: |
       GroupDocs.Signature به ما امکان می‌دهد کدهای QR را تولید و به اسناد با قالب‌های پشتیبانی شده اضافه کنیم. مسیر سندی را که باید امضا شود ارائه دهید و گزینه های متنی و تصویری کد QR مورد نظر را تنظیم کنید. می توانید تصویر کد QR تولید شده را در هر ناحیه از هر صفحه سند قرار دهید.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // سند را برای امضا مشخص کنید
            using (Signature signature = new Signature("source.docx"))
            {
                // گزینه های علامت QR-code را ایجاد کنید
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // گزینه های کد QR را تنظیم کنید
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // فایل پردازش شده را امضا و ذخیره کنید
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // سند را برای امضا مشخص کنید
            Signature signature = new Signature("source.docx");

            // گزینه های علامت QR-code را ایجاد کنید
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // گزینه های کد QR را تنظیم کنید
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // فایل پردازش شده را امضا و ذخیره کنید
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // سند را برای امضا مشخص کنید
            const signature = new signatureLib.Signature('source.docx');

            // گزینه های علامت QR-code را ایجاد کنید
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // گزینه های کد QR را تنظیم کنید
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // فایل پردازش شده را امضا و ذخیره کنید
            signature.sign('result.docx', options);
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "بیش از 60 فرمت فایل پشتیبانی می شود"
  description: "GroupDocs.Signature تقریباً از همه فرمت‌های فایل محبوب پشتیبانی می‌کند"

############################# Metrics ###############################
metrics:
  enable: true
  title: "داده های آماری کتابخانه ما"
  description: "معیارهای کلیدی محصول را بررسی کنید و بینش هایی را در مورد دستاوردها، تأثیر و رشد ما آشکار کنید"

  items:
    # items loop
    - number: "50+"
      title: "فرمت های پشتیبانی شده"
      content: "امضای بیش از 60 مورد از محبوب ترین فرمت های فایل تجاری."

    # items loop
    - number: "500k"
      title: "دانلودهای NuGet"
      content: "GroupDocs.Signature برای دات نت یک کتابخانه محبوب با بیش از 550000 بارگیری در NuGet است."

    # items loop
    - number: "15k"
      title: "Maven دانلود می کند"
      content: "توسعه دهندگان جاوا GroupDocs.Signature را بیش از 15 هزار بار در Maven دانلود کرده اند."

    # items loop
    - number: "140+"
      title: "مشتریان خوشحال"
      content: "توسعه دهندگان فردی و شرکت های برتر در سراسر جهان از محصولات ما برای ایجاد راه حل های نوآورانه استفاده می کنند."


############################# Customers ###############################
customers:
  enable: true
  title: "مشتریان خوشحال ما"
  description: "کتابخانه های GroupDocs توسط برندهای مشهور و برجسته جهانی در سراسر جهان به کار گرفته می شوند"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "برای شروع آماده اید؟"
  description: "ویژگی های GroupDocs.Signature را به صورت رایگان در پلتفرم خود امتحان کنید"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "سوالات متداول"
  description: "سوالات متداول ما را کاوش کنید"

  items:
    # items loop
    - question: "آیا GroupDocs.Signature برای امضای اسناد به کتابخانه خارجی نیاز دارد؟"
      answer: "نه، GroupDocs.Signature مستقل کار می کند. هیچ وابستگی شخص ثالثی مانند Adobe Acrobat، Microsoft Office و غیره وجود ندارد."

    # items loop
    - question: "آیا امکان تست ویژگی های GroupDocs.Signature قبل از خرید وجود دارد؟"
      answer: "کاملا! GroupDocs.Signature یک آزمایش رایگان ارائه می‌دهد. آن را نصب کنید و ویژگی های آن را بررسی کنید. توجه داشته باشید که نسخه‌های آزمایشی «نشان‌های آزمایشی» را به اسناد شما اضافه می‌کنند و فقط 3 صفحه اول را پردازش می‌کنند. برای تجربه کامل، یک مجوز موقت 30 روزه رایگان برای دسترسی به همه عملکردها دریافت کنید. جزئیات را در [مجوز موقت](https://purchase.groupdocs.com/temporary-license/) ببینید."

    # items loop
    - question: "چه انواع مجوز ارائه شده است؟"
      answer: "به دنبال مجوز GroupDocs.Signature هستید؟ ما گزینه های مختلفی را متناسب با نیاز شما ارائه می دهیم. بر اساس اندازه تیم، مکان‌های استقرار (دفتر منفرد یا محل کار راه دور)، و اینکه آیا توزیع مشتری نهایی نیاز به اشتراک‌گذاری SDK/API با مشتریان دارد یا خیر، انتخاب کنید. از طرف دیگر، مجوز استفاده ماهانه با برنامه های اندازه گیری شده را انتخاب کنید - فقط برای آنچه استفاده می کنید پرداخت کنید. بهترین مناسب برای خود را در [قیمت گذاری](https://purchase.groupdocs.com/pricing/signature/net/) کشف کنید."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "APIهای کم کد GroupDocs.Signature"
  description: "فایل ها را با استفاده از برنامه خود از طریق REST API مبتنی بر ابر ما امضا کنید."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "از CURL RESTful API برای قرار دادن امضا روی PDF، Word، Excel، PowerPoint، JPEG و بسیاری از فرمت‌های فایل دیگر استفاده کنید."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "برنامه های NET خود را با امضای اسناد از طریق Cloud SDK غنی کنید. از اسناد تجاری به روش خود محافظت کنید."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "GroupDocs.Signature SDK به برنامه‌های جاوای شما برای امضای فایل‌ها به امکانات مختلفی دسترسی می‌دهد."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "برنامه های وب GroupDocs.Signature"
  description: "GroupDocs.Signature یک برنامه وب رایگان را ارائه می دهد که می توانید اسناد را امضا کنید. بیش از 60 فرمت فایل محبوب را می توان از طریق مرورگر مورد علاقه شما به صورت رایگان امضا کرد."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "ابزار آنلاین برای قرار دادن امضا بر روی اسناد از هر دستگاه."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "MS Word DOCX را به صورت آنلاین امضا کنید."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "از اسناد PDF به صورت آنلاین محافظت کنید."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---