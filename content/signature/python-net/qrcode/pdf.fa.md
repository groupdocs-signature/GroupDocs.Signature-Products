



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:03
draft: false
lang: fa
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "ایجاد بارکدهای QR برای فایل‌های PDF با استفاده از Python"
head_description: "از API GroupDocs.Signature برای تولید و درج بارکدهای QR در فایل‌های PDF استفاده کنید. بارکدهای QR را به راحتی در هر صفحه قرار دهید تا عملکرد اضافی را اضافه کنید."

############################# Header ############################
title: "ایجاد بارکدهای QR برای PDF" 
description: "با استفاده از GroupDocs.Signature for Python via .NET بارکدهای 2بعدی را با داده‌های متنی یا عددی ایجاد کرده و آن‌ها را به صفحات و فرمت‌های مختلف، از جمله PDF، Word، Excel و غیره اعمال کنید."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "آزمایش رایگان"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "ویژگی‌های GroupDocs.Signature for Python via .NET را بررسی کنید"
    link: "/signature/python-net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) قابلیت‌های گسترده‌ای را ارائه می‌دهد که به کاربران امکان می‌دهد انواع مختلف امضا را در قالب‌های مستندات اصلی تولید و درج کنند. چه این مستندات PDF، Word، Excel، PowerPoint یا تصاویر باشند، مدارک خود را با امضاهای متنی، تصویری، بارکدی، QR Code، متادیتا، دیجیتال یا مهر تقویت کنید.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل ایجاد و درج یک بارکد QR در PDF"
    content: |
      [GroupDocs.Signature](/signature/python-net/) به شما اجازه می‌دهد بارکدهای QR را در فرمت‌های محبوب ایجاد کرده و آن‌ها را در صفحات PDF قرار دهید. با پشتیبانی از بیش از 10 نوع بارکد QR، می‌توانید به راحتی این قابلیت را در برنامه‌های Python via .NET یکپارچه کنید. مدارک خود را با امضاهای بارکد QR با استفاده از محصول ما تقویت کنید.
      
      1. فایل یا جریان PDF را که بارکد QR به آن اضافه خواهد شد، به دست آورید.
      2. متن مورد نیاز را به QrCodeSignOptions ارائه دهید.
      3. تنظیمات بصری مانند رنگ، موقعیت و اندازه را سفارشی کنید.
      4. مستند را با بارکد QR درج شده ذخیره کنید.
   
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

            # یک نمونه جدید Signature را با مستند ایجاد کنید
            with sg.Signature('input.pdf') as signature:

                # از QrCodeSignOptions برای درج بارکد QR در مستند استفاده کنید
                options = sg.QrCodeSignOptions("Text Content")

                # نوع امضا را مشخص کرده و موقعیت آن را در صفحه تنظیم کنید
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # مستند را با بارکد QR درج شده ذخیره کنید
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ادغام کامل امضا برای مستندات"
  description: "با API GroupDocs.Signature for Python via .NET، کاربران می‌توانند انواع مختلف امضا را تولید، اصلاح، جستجو، تأیید و حذف کنند و جریان‌های کاری مستندات را با دقت ساده کنند."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Signature"
  features:
    # feature loop
    - title: "اعمال چندین نوع امضا"
      content: "GroupDocs.Signature امکان به کارگیری امضاهای متنی، تصویری، بارکدی، QR Code و مهر را برای هر مستند فراهم می‌کند. شما می‌توانید امضاها را به طور دقیق در هر صفحه قرار دهید و متادیتا را به راحتی مدیریت کنید. مدارک خود را از تغییرات غیرمجاز با گواهی‌های دیجیتال محافظت کنید."

    # feature loop
    - title: "جستجو و تأیید امضاها"
      content: "با استفاده از ابزارهای تأیید پیشرفته، اصالت و دقت امضاهای مستندات را بررسی کنید. به راحتی لیستی دقیق از تمام امضاهای درج شده در یک مستند را برای نظارت بهتر دریافت کنید."

    # feature loop
    - title: "اصلاح امضاهای موجود"
      content: "شما می‌توانید امضاهای قبلاً اعمال شده را با تنظیم محتوا، موقعیت، رنگ، اندازه و سایر خصوصیات مطابق نیازهای خاص خود به‌روز کنید."

    # feature loop
    - title: "حذف امضاها به راحتی"
      content: "مدیریت مستندات را با حذف سریع امضاهای ناخواسته به streamline تبدیل کنید. چه این یک گواهی دیجیتال باشد یا نوع دیگر امضا، حذف می‌تواند به صورت کارآمد انجام شود."
      
  code_samples_ext:
    # code sample ext loop
    - title: "سفارشی‌سازی بارکد QR تولید شده"
      content: |
        این مثال نشان می‌دهد چگونه یک بارکد QR سفارشی را در یک صفحه PDF قرار دهید.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # مستند که باید امضا شود را دریافت کرده و آن را به Signature منتقل کنید
              with sg.Signature('input.pdf') as signature:

                    # تنظیمات بارکد QR را با متن مورد نیاز پیکربندی کنید
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # موقعیت بارکد QR را در صفحه تنظیم کنید
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # حدود مستند را برای امضا تنظیم کنید
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # رنگ بارکد QR را انتخاب کنید
                    options.ForeColor = sg.Color.Red

                    # گزینه‌های فونت برای پیام را تعریف کنید
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # رنگ پس‌زمینه و قلم برای بارکد QR را تعیین کنید
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # بارکد QR را در مستند درج کنید
                    result = signature.Sign("output.pdf", options)
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
            link: "/examples/signature/formats/signature_qrcode.pdf"
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
    title: "راه‌حل‌های امضای ما را بررسی کنید"
    exclude: "qrcode"
    description: "ما انواع و عملیات مختلفی از امضاها را ارائه می‌دهیم تا نیازهای مستندات شما را برآورده کنیم."
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
    title: "درج بارکدهای QR در قالب‌های مختلف مستندات"
    exclude: "PDF"
    description: "از API Python via .NET برای درج بارکدهای QR در هر قالب مستند استاندارد صنعتی استفاده کنید. اطلاعات مهم را در بارکدهای 2بعدی ذخیره و کدگذاری کنید تا به راحتی اسکن و بازیابی شوند."
    items: 
          
        # format loop 1
        - name: "QR-Code برای PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "QR-Code برای DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "QR-Code برای JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "QR-Code برای PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "QR-Code برای XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---