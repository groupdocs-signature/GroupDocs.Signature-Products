



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:11
draft: false
lang: fa
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "قرار دادن امضای تصویر در فایل‌های JPEG با Python"
head_description: "امضای تصویری را در اسناد JPEG برای Python تنها با چند خط کد قرار دهید. از API GroupDocs.Signature for Python via .NET استفاده کنید تا امضای مبتنی بر تصویر را به آسانی اضافه کنید."

############################# Header ############################
title: "اضافه کردن امضای تصویر به JPEG" 
description: "از GroupDocs.Signature for Python via .NET برای گنجاندن امضای تصویری به راحتی در قالب‌های مختلف اسناد اداری، از جمله PDF، Word، Excel و فایل‌های تصویری استفاده کنید. اضافه کردن تصویری از امضای مدیر شما به حرفه‌ای بودن اسناد کمک کرده و تأثیر بصری و اعتبار سند را افزایش می‌دهد."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "رایگان دانلود کنید"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "کشف GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) گزینه‌های متنوعی را برای گنجاندن امضاهای تصویری در هر کجای اسناد تجاری شما ارائه می‌دهد. با استفاده از کتابخانه قدرتمند ما، فرآیندها را با اضافه کردن تصاویر به PDFs، اسناد Word، شیت‌های Excel، ارائه‌های PowerPoint و فرمت‌های رایج تصویری ساده کنید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه یک امضای تصویر به فایل JPEG با استفاده از Python اضافه کنیم"
    content: |
      استفاده از [GroupDocs.Signature](/signature/python-net/) برای ارائه قابلیت به برنامه‌های Python via .NET جهت اضافه کردن دقیق امضاهای تصویر در هر جا در اسناد JPEG. با ادغام راه‌حل ما، محصول خود را تقویت کنید.
      
      1. یک نمونه Signature با سند JPEG ایجاد کنید.
      2. تنظیم ImageSignOptions با تصویر دلخواه برای امضا.
      3. دقیقاً تصویر را در محل انتخابی خود در سند قرار دهید.
      4. سند امضا شده را در مکان مشخص ذخیره کنید.
   
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

            # درست کردن Signature با مسیر سند
            with sg.Signature('input.jpeg') as signature:

                # تنظیم ImageSignOptions با تصویر انتخاب شده برای امضا
                options = sg.ImageSignOptions("company_logo.jpg")

                # قرار دادن تصویر در گوشه بالا-چپ هر صفحه
                options.AllPages = True
                options.Left = 100
                options.Top = 200
                
                # ذخیره سند امضا شده
                result = signature.Sign("output.jpeg", options)
        ```          

############################# More features ############################
more_features:
  enable: true
  title: "ویژگی‌های گسترده امضای اسناد"
  description: "API ما از دامنه وسیعی از قابلیت‌های امضای مستندات پشتیبانی می‌کند. شما به راحتی می‌توانید انواع مختلف امضاها، از جمله امضاهای مبتنی بر تصویر را اضافه، به‌روزرسانی، حذف، جستجو و اعتبارسنجی کنید."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "یکپارچه‌سازی امضای تصویر"
  features:
    # feature loop
    - title: "قرار دادن تصاویر در اسناد اداری"
      content: "امضاهای الکترونیکی و تصاویر را در هر نقطه انتخاب شده در یک سند قرار دهید. اسناد خود را با تصاویر، بارکدها، متن، متاداده یا گواهی‌های دیجیتال بهبود دهید تا عملکرد و امنیت را افزایش دهید."

    # feature loop
    - title: "جستجوی امضا و اعتبارسنجی"
      content: "با تأیید اعتبار امضاها، یکپارچگی سند را تضمین کنید. فهرستی دقیق از تمامی امضاها در یک سند را بازیابی کنید و خواص فردی آن‌ها را ارزیابی کنید."

    # feature loop
    - title: "ویرایش امضاهای موجود"
      content: "محتوا، ظاهر، اندازه یا موقعیت امضاها در اسناد خود را به سادگی به‌روزرسانی کنید تا به نیازهای متغیر پاسخ دهید."

    # feature loop
    - title: "حذف امضاهای غیرضروری"
      content: "API ما کنترل کامل را فراهم می‌آورد و به شما اجازه می‌دهد تا هر زمان که لازم باشد، امضاها را از بیشتر فرمت‌های پشتیبانی‌شده حذف کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "افزایش اسناد با امضاهای تصویر"
      content: |
        یاد بگیرید که چگونه امضاهای تصویر را در اسناد تجاری خود گنجانده و محتوا را غنی کنید.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # سندی که می‌خواهید امضا شود را انتخاب کنید
              with sg.Signature('input.jpeg') as signature:

                    # تنظیم گزینه‌های تصویر با مسیر فایل تصویر
                    options = sg.ImageSignOptions("manager_signature.jpg")

                    # اندازه امضای تصویر را مشخص کنید
                    options.Width = 100
                    options.Height = 100

                    # تصویر را در گوشه پایین-راست صفحه قرار دهید
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right

                    # در صورت نیاز، از لبه‌های صفحه فاصله‌گذاری کنید
                    options.Margin = sg.Padding()
                    options.Margin.Bottom = 120
                    options.Margin.Right = 120

                    # به صورت اختیاری، دور تصویر حاشیه‌ای اضافه کنید
                    options.Border = sg.Border()
                    options.Border.Visible = True
                    options.Border.Color = sg.Color.OrangeRed
                    options.Border.DashStyle = sg.DashStyle.DashDotDot
                    options.Border.Weight = 5

                    # تصویر را بچرخانید تا تراز درست شود
                    options.RotationAngle = 45

                    # سند به‌روز شده را ذخیره کنید
                    result = signature.Sign("output.jpeg", options)
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
            link: "/examples/signature/formats/signature_image.jpeg"
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
    title: "ویژگی‌های ما را کشف کنید"
    exclude: "image"
    description: "امضاهای بزرگ مختلف و عملیاتی که پلتفرم ما ارائه می‌دهد را کشف کنید."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/python-net/esign/jpeg/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/python-net/text/jpeg/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/python-net/image/jpeg/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/python-net/barcode/jpeg/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/python-net/stamp/jpeg/"
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
    title: "قرار دادن تصاویر در فرمت‌های متنوع"
    exclude: "JPEG"
    description: "از API Python via .NET برای قرار دادن تصاویر در فرمت‌های مختلف اسناد استفاده کنید. به راحتی اندازه، موقعیت، صفحات خاص را انتخاب کنید و امضای مبتنی بر تصویر را اعمال کنید و کنترل کامل بر روی چینش سند خود داشته باشید."
    items: 
          
        # format loop 1
        - name: "امضای PDF با تصویر"
          format: "PDF"
          link: "/signature/python-net/image/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "امضای DOCX با تصویر"
          format: "DOCX"
          link: "/signature/python-net/image/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "امضای JPEG با تصویر"
          format: "JPEG"
          link: "/signature/python-net/image/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "امضای PPTX با تصویر"
          format: "PPTX"
          link: "/signature/python-net/image/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "امضای XLSX با تصویر"
          format: "XLSX"
          link: "/signature/python-net/image/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---