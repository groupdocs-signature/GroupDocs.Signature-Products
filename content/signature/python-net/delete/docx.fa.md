



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:43
draft: false
lang: fa
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "حذف امضاها از DOCX با استفاده از Python"
head_description: "به راحتی امضاهای دیجیتال، بارکد، متن، تصویر و متاداده را از مستندات DOCX با GroupDocs.Signature for Python via .NET حذف کنید."

############################# Header ############################
title: "حذف امضاها از DOCX" 
description: "علاوه بر امضای مستندات، GroupDocs.Signature for Python via .NET مجموعه کاملی از ابزارها را برای شناسایی و حذف انواع مختلف امضاها از فایل‌های شما ارائه می‌دهد."
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
    title: "GroupDocs.Signature for Python via .NET چیست؟"
    link: "/signature/python-net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) یک راه‌حل قدرتمند برای مدیریت امضاهای مختلف، شامل متن، تصاویر، بارکدها، گواهی‌های دیجیتال و مهرها است. با پشتیبانی از بیش از 60 فرمت مختلف مانند PDF، مستندات MS Office، تصاویر و فایل‌های ZIP، حداکثر انعطاف‌پذیری را در مدیریت مستندات ارائه می‌دهد. شما می‌توانید به راحتی امضاها را اضافه، تأیید، به‌روزرسانی یا حذف کنید.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل حذف امضاهای الکترونیکی از DOCX با استفاده از Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) به توسعه‌دهندگان Python via .NET این امکان را می‌دهد تا امضاهای الکترونیکی را از فایل‌های DOCX با پیروی از این مراحل ساده حذف کنند:
      
      1. مدرک DOCX را به نمونه کلاس Signature بارگذاری کنید.
      2. از تابع جستجو برای پیدا کردن همه امضاها در سند استفاده کنید.
      3. یک یا چند امضای پیدا شده را حذف کنید.
      4. پس از پردازش نتایج را بررسی کنید.
   
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

            # مدرکی با امضاها را به نمونه Signature منتقل کنید
            with sg.Signature('input.docx') as signature:

                # فهرست امضاهای دیجیتال موجود در سند را دریافت کنید
                options = sg.DigitalSearchOptions()

                signatures = signature.Search(options)

                # اولین امضا را از فهرست حذف کنید
                digitalSignature = signatures[0]
                result = signature.Delete(digitalSignature)

                # نتایج حذف را پردازش و تأیید کنید
                if result:
                    print("\nDigital signature in DOCX was deleted successfully")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "مدیریت مستندات را با ویژگی‌های پیشرفته امضا ساده کنید"
  description: "GroupDocs.Signature for Python via .NET به طور تخصصی طراحی شده است تا فرآیند افزودن، تأیید، ویرایش و حذف امضاها را در فرمت‌های کلیدی مستندات تجاری بهبود بخشد."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضای مستندات خود"
      content: "به سرعت امضاهای متنی، تصویری، بارکدی، کد QR یا مهرها را در هر صفحه اعمال کنید. علاوه بر این، می‌توانید متاداده‌های پنهان مانند EXIF در تصاویر را مدیریت کرده و با گواهی‌های دیجیتال از یکپارچگی مستندات اطمینان حاصل کنید."

    # feature loop
    - title: "شناسایی و تأیید امضاها"
      content: "از ابزارهای قدرتمند ما برای شناسایی و تأیید امضاها در مستندات خود استفاده کنید و فهرست کاملی از همه امضاها برای مدیریت جامع دریافت کنید."

    # feature loop
    - title: "ویرایش امضاها"
      content: "به راحتی امضاهای موجود را با تغییر متن، جابجایی عناصر یا تنظیم رنگ‌ها مطابق با سلیقه خود اصلاح کنید."

    # feature loop
    - title: "حذف امضاهای نامطلوب"
      content: "کنترل کامل بر امضاهای مستندات را با عملیات کامل ایجاد، خواندن، به‌روزرسانی و حذف (CRUD) داشته باشید و به شما اجازه می‌دهد هر نوع امضا را در صورت نیاز حذف کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "حذف همه امضاهای بارکدی"
      content: |
        یاد بگیرید چگونه همه امضاهای بارکدی را از یک سند حذف کنید.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # سندی که شامل امضاهای بارکدی است را فراهم کنید
              with sg.Signature('input.docx') as signature:

                    # تمام امضاهای بارکدی را حذف کنید
                    result = signature.Delete(SignatureType.Barcode)

                    # نتایج فرآیند حذف را بررسی کنید
                    if result.Succeeded.Count > 0:
                        print("\n DOCX barcode signatures were deleted") 
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
    title: "ویژگی‌های کلیدی ما را کشف کنید"
    exclude: "delete"
    description: "دامنه وسیعی از انواع امضاها و عملیات‌های موجود با راه‌حل ما را بررسی کنید."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/python-net/esign/docx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/python-net/text/docx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/python-net/image/docx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/python-net/barcode/docx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/docx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/python-net/stamp/docx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/python-net/search/docx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/python-net/verify/docx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/python-net/modify/docx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/python-net/delete/docx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "حذف امضاها از چندین فرمت فایل"
    exclude: "DOCX"
    description: "GroupDocs.Signature for Python via .NET برای پشتیبانی از حذف امضاها از بیش از 60 فرمت فایل مختلف ساخته شده است و اطمینان از سازگاری و سهولت استفاده را تضمین می‌کند."
    items: 
          
        # format loop 1
        - name: "حذف امضاهای PDF"
          format: "PDF"
          link: "/signature/python-net/delete/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "حذف امضاهای DOCX"
          format: "DOCX"
          link: "/signature/python-net/delete/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "حذف امضاهای PPTX"
          format: "PPTX"
          link: "/signature/python-net/delete/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "حذف امضاهای XLSX"
          format: "XLSX"
          link: "/signature/python-net/delete/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---