



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:14
draft: false
lang: fa
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "جستجوی امضاهای الکترونیکی برای PDF با استفاده از Python"
head_description: "از API GroupDocs.Signature for Python via .NET برای جستجوی امضاهای الکترونیکی تعبیه‌شده در فرمت‌هایی مانند PDF، Word، Excel، ارائه‌ها و تصاویر بهره ببرید."

############################# Header ############################
title: "جستجوی امضاهای دیجیتال PDF" 
description: "فهرستی کامل از امضاهای الکترونیکی را از چندین فرمت، از جمله PDF، Word، Excel، ارائه‌ها و تصاویر، با قدرت GroupDocs.Signature for Python via .NET استخراج کنید."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "همین حالا دانلود کنید"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "پتانسیل GroupDocs.Signature for Python via .NET را آزاد کنید"
    link: "/signature/python-net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) قابلیت‌های پیشرفته‌ای برای امضا و مدیریت اسناد دیجیتال ارائه می‌دهد. با پشتیبانی از بیش از 60 فرمت فایل، از جمله PDF، اسناد آفیس، تصاویر و فایل‌های ZIP، می‌توانید امضاهای متنی، تصویری، بارکدها، کدهای QR، گواهی‌نامه‌های دیجیتال و مهرها را اضافه، جستجو، تأیید، ویرایش یا حذف کنید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونگی جستجوی امضاها در PDF با استفاده از Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) یک موتور قدرتمند برای شناسایی امضاهای دیجیتال در فایل‌های PDF فراهم می‌کند. توسعه‌دهندگان Python via .NET می‌توانند به راحتی با این قابلیت، برنامه‌های خود را تقویت کنند.
      
      1. مسیر فایل PDF را برای جستجوی امضا فراهم کنید.
      2. از SearchOptions برای تصحیح معیارهای جستجو استفاده کنید.
      3. متد Search را فراخوانی کنید تا نتایج را بازیابی کنید.
      4. فهرست امضاهای شناسایی شده را مرور کنید.
   
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

            # شیء Signature را با مسیر فایل سند مقداردهی اولیه کنید
            with sg.Signature('input.pdf') as signature:

                # یک نمونه از TextSearchOptions برای جستجو در تمام صفحات ایجاد کنید
                options = sg.TextSearchOptions()
                options.AllPages = True

                # جستجو را برای پیدا کردن هر گونه امضای متنی در سند اجرا کنید
                signatures = signature.Search(options)
                print("\nSource document contains following text signature(s).")

                # فهرستی از امضاهای پیدا شده را برای بررسی دقیق جمع‌آوری کنید
                for textSignature in signatures:
                    print("\nFound Text signature at page ", textSignature.PageNumber)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "یک پلتفرم کامل برای امضای اسناد"
  description: "یک راه‌حل امضای قدرتمند و پر ویژگی را تجربه کنید که اسناد شما را با انواع مختلف امضا در فرمت‌های متنوع ایمن می‌کند."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "جستجو و مدیریت امضاها"
  features:
    # feature loop
    - title: "امضا و ایمن‌سازی اسناد تجاری"
      content: "امضاهای الکترونیکی را در هر نقطه از یک سند اضافه کنید. GroupDocs.Signature از انواع مختلف امضا، از جمله متن، تصاویر، بارکدها، متاداده، مهرها و گواهی‌نامه‌های دیجیتال پشتیبانی می‌کند و اعتبار و امنیت سند را تضمین می‌نماید."

    # feature loop
    - title: "مدیریت جامع امضا"
      content: "پس از امضا شدن یک سند، از ویژگی جستجو برای یافتن تمام امضاهای تعبیه‌شده استفاده کنید. می‌توانید امضاها را تغییر یا حذف کنید و کنترل کامل بر تمامیت سند را در اختیار داشته باشید."

    # feature loop
    - title: "اطمینان از تمامیت سند"
      content: "از ابزارهای پیشرفته برای مدیریت متاداده‌های پنهان در اسناد استفاده کنید. متاداده را اضافه یا حذف کنید و از گواهی‌نامه‌های دیجیتال برای محافظت از اسناد خود در برابر تغییرات غیرمجاز استفاده کرده و اصالت آن‌ها را تضمین کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "جستجوی امضاهای تصویری"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان یک امضای تصویری را در یک سند خاص پیدا کرد.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # سند منبع را به سازنده منتقل کنید
              with sg.Signature('input.pdf') as signature:

                    # هرگونه امضای متنی را جستجو کنید
                    signatures = signature.Search(sg.SignatureType.Image)
                    print("\nSource document contains following image signature(s).")

                    # ویژگی‌های دقیق امضاهای شناسایی شده را نمایش دهید
                    for imageSignature in signatures:
                        print("\nFound image signature at page ", imageSignature.PageNumber)
          ```
        platform: "python-net"
        copy_title: "کپی"
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
    title: "ویژگی‌های اصلی"
    exclude: "search"
    description: "API ما انعطاف‌پذیری گسترده‌ای را فراهم می‌کند که به کاربران اجازه می‌دهد اسناد را امضا کرده و اقدام‌های پس از امضا مانند جستجو، تأیید و ویرایش امضاها را انجام دهند."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/python-net/esign/pdf/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/python-net/text/pdf/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/python-net/image/pdf/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/python-net/barcode/pdf/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pdf/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/python-net/stamp/pdf/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "استخراج امضاها از فرمت‌های متنوع فایل"
    exclude: "PDF"
    description: "API GroupDocs.Signature for Python via .NET به شما امکان می‌دهد امضاها را از مجموعه متنوعی از فرمت‌های سند استخراج و مدیریت کنید. به راحتی امضاهای تعبیه‌شده را از انواع اصلی فایل‌ها برای تجزیه و تحلیل یا پردازش بیشتر بازیابی کنید."
    items: 
          
        # format loop 1
        - name: "جستجوی امضاها در PDF"
          format: "PDF"
          link: "/signature/python-net/search/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "یافتن امضاها در DOCX"
          format: "DOCX"
          link: "/signature/python-net/search/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "یافتن امضاها در PPTX"
          format: "PPTX"
          link: "/signature/python-net/search/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "جستجوی امضاها در XLSX"
          format: "XLSX"
          link: "/signature/python-net/search/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---