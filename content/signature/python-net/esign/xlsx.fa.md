



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:30
draft: false
lang: fa
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "امضای الکترونیکی اسناد XLSX با برنامه‌های Python"
head_description: "قدرت API Python را برای امضای الکترونیکی و ایمن‌سازی اسناد XLSX مانند PDF، فایل‌های Word، صفحات Excel، ارائه‌ها و تصاویر به کار ببرید."

############################# Header ############################
title: "امضای الکترونیکی XLSX" 
description: "از GroupDocs.Signature for Python via .NET برای وارد کردن انواع امضاهای الکترونیکی به اسناد خود استفاده کنید و از انطباق و یکپارچگی داده‌ها در فرمت‌های مختلف مانند PDF، Word، Excel، ارائه‌ها و تصاویر اطمینان حاصل کنید."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "مروری بر API GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) مجموعه کاملی از ابزارها را برای افزودن امضاهای الکترونیکی به اسناد فراهم می‌کند. چه نیاز به امضا، جستجو، تأیید، به‌روزرسانی یا حذف امضاهای دیجیتال داشته باشید، GroupDocs.Signature for Python via .NET این کار را در فرمت‌های مختلف—PDF، مستندات Word، صفحات Excel، ارائه‌های PowerPoint و فرمت‌های تصویر متنوع—بدون نیاز به نرم‌افزارهای شخص ثالث آسان می‌سازد.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل امضای الکترونیکی XLSX با استفاده از Python"
    content: |
      با [GroupDocs.Signature](/signature/python-net/)، توسعه‌دهندگان Python via .NET می‌توانند به‌طور یکپارچه قابلیت امضا را به اسناد XLSX اضافه کنند. امضاهای سفارشی را به برنامه‌های خود اضافه کنید.
      
      1. فایل XLSX را به نمونه Signature بارگذاری کنید.
      2. از SignOptions برای پیکربندی تنظیمات امضا استفاده کنید.
      3. خصوصیات امضا مانند اندازه، رنگ و محتوا را سفارشی کنید.
      4. سند امضا شده را در محل دلخواه ذخیره کنید.
   
    code:
      platform: "python-net"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "نمونه امضاها"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شد"
      links:
        #  loop
        - title: "نمونه‌های بیشتر"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # سند را به یک نمونه Signature بارگذاری کنید
            with sg.Signature('input.xlsx') as signature:

                # یک شیء QrCodeSignOptions جدید ایجاد کنید
                options = sg.QrCodeSignOptions("QR code text")

                # تمام گزینه‌های لازم را تنظیم کنید
                options.Left = 100
                options.Top = 100
                options.ForeColor = sg.Color.Red

                # سند امضا شده را در سیستم خود ذخیره کنید
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ویژگی‌های پیشرفته امضای الکترونیکی برای اسناد"
  description: "API امضا کردن ما، فرآیندهای کسب و کار را با ارائه روش‌های کارآمد برای امضا، اعتبارسنجی، ویرایش و مدیریت امضاهای الکترونیکی با پشتیبانی کامل از اتوماسیون، تسهیل می‌کند."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "ویژگی‌های امضای الکترونیکی"
  features:
    # feature loop
    - title: "امضای اسناد اداری"
      content: "امضاهای الکترونیکی را به راحتی در هر نقطه‌ای از اسناد خود قرار دهید. محتوای خود را با گواهی‌نامه‌های دیجیتال، بارکدها، متاداده و عناصر بصری سفارشی کنید، در حالی که امنیت و اصالت سند را تضمین می‌نمایید."

    # feature loop
    - title: "مدیریت کامل امضا"
      content: "پس از امضای یک سند، می‌توانید همه امضاها را مشاهده و مدیریت کنید. می‌توانید به‌روزرسانی ایجاد کنید یا امضاها را در صورت نیاز حذف نمایید و کنترل کامل بر سند را داشته باشید."

    # feature loop
    - title: "افزایش امنیت سند"
      content: "اسناد خود را با گواهی‌نامه‌های دیجیتال محافظت کنید. متاداده را وارد یا بازیابی کنید تا ردیابی، حسابرسی و انطباق را بهبود بخشید و اصالت محتوای خود را تضمین نمایید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه یک امضای تصویر به سند اضافه کنید"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توانید یک امضای تصویر را به یک صفحه خاص از سند اعمال کنید.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg
        
          def run():

              # سندی را که می‌خواهید امضا کنید بارگذاری کنید
              with sg.Signature('input.xlsx') as signature:

                  # مسیر تصویر را در گزینه‌های امضا تنظیم کنید
                  options = sg.ImageSignOptions("image.jpg")

                  # اندازه و مکان امضا را در صفحات هدف تعریف کنید
                  options.VerticalAlignment = sg.VerticalAlignment.Bottom
                  options.HorizontalAlignment = sg.HorizontalAlignment.Right
                  options.Height = 150
                  options.Width = 200
                  options.Margin = sg.Padding(50)
                  options.AllPages = True

                  # امضا را اعمال کرده و سند امضا شده را ذخیره کنید
                  result = signature.Sign("output.xlsx", options)
          ```
        platform: "python-net"
        copy_title: "کپی"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "برای کپی کلیک کنید"
          copy_done: "کپی شد"
        top_links:
          #  loop
          - title: "دانلود نتیجه"
            icon: "download"
            link: "/examples/signature/formats/signature_esign.xlsx"
        links:
          #  loop
          - title: "نمونه‌های بیشتر"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "امکانات GroupDocs.Signature را به صورت رایگان امتحان کنید یا درخواست مجوز ارسال کنید"
  items:
    #  loop
    - title: "بارگیری PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "مجوزدهی"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "کشف مجموعه ویژگی‌های کامل ما"
    exclude: "esign"
    description: "ما مجموعه وسیعی از گزینه‌ها و عملیات امضا را برای تمامی نیازهای امضای الکترونیکی شما ارائه می‌دهیم."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "امضای دامنه وسیعی از فرمت‌های فایل"
    exclude: "XLSX"
    description: "با API Python via .NET، می‌توانید بیش از 60 فرمت استاندارد صنعتی را به‌طور الکترونیکی امضا کنید و انعطاف‌پذیری بی‌نظیری در ایمن‌سازی اسناد کسب و کار خود ارائه دهید."
    items: 
          
        # format loop 1
        - name: "امضای الکترونیکی PDF"
          format: "PDF"
          link: "/signature/python-net/esign/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "امضای الکترونیکی DOCX"
          format: "DOCX"
          link: "/signature/python-net/esign/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "امضای الکترونیکی JPEG"
          format: "JPEG"
          link: "/signature/python-net/esign/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "امضای الکترونیکی PPTX"
          format: "PPTX"
          link: "/signature/python-net/esign/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "امضای الکترونیکی XLSX"
          format: "XLSX"
          link: "/signature/python-net/esign/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---