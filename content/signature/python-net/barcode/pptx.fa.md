



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:07
draft: false
lang: fa
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "یک بارکد را با Python در PPTX قرار دهید"
head_description: "با چند خط در Python، امضای بارکد را به اسناد PPTX به طور موثر اضافه کنید. GroupDocs.Signature راه‌حل‌های امضای یکپارچه‌ای برای چندین فرمت سند ارائه می‌دهد."

############################# Header ############################
title: "ایجاد بارکد برای PPTX" 
description: "با GroupDocs.Signature for Python via .NET، می‌توانید بارکدها را در هر نقطه از اسناد تجاری خود قرار دهید. راه‌حل ما گزینه‌های انعطاف‌پذیری برای سفارشی‌سازی امضای بارکد ارائه می‌دهد."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "نسخه آزمایشی رایگان"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "درباره GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) ابزاری قدرتمند برای امضای اسناد است که از طیف وسیعی از انواع امضاها، از جمله متن، تصاویر، بارکدها، گواهی‌های دیجیتال و مهرها پشتیبانی می‌کند. این ابزار با بیش از ۶۰ فرمت فایل، از جمله PDF، MS Office، تصاویر، ZIP و غیره سازگار است و به شما این امکان را می‌دهد که امضاها را اعمال کنید و همچنین به جستجو، تأیید، اصلاح یا حذف آنها بپردازید.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل تولید و درج یک بارکد در PPTX"
    content: |
      [GroupDocs.Signature](/signature/python-net/) به شما این امکان را می‌دهد که بارکدها را به سرعت و به آسانی در اسناد PPTX تولید و درج کنید. پشتیبانی از بیش از ۶۰ فرمت بارکد، برنامه‌های Python via .NET می‌توانند به‌راحتی قابلیت‌های امضای بارکد را با ادغام کتابخانه ما اضافه کنند.
      
      1. فایل یا جریان PPTX را برای پردازش فراهم کنید.
      2. متن بارکد را به شیء BarcodeSignOptions اختصاص دهید.
      3. گزینه‌های بارکد، مانند موقعیت و اندازه را تنظیم کنید.
      4. سند را با بارکد درج شده ذخیره کنید.
   
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

            # شیء Signature را با مسیر سند اولیه‌سازی کنید
            with sg.Signature('input.pptx') as signature:

                # از BarcodeSignOptions برای افزودن یک بارکد به سند استفاده کنید
                options = sg.BarcodeSignOptions('Business data')

                # نوع بارکد را تنظیم کرده و ویژگی‌های آن را پیکربندی کنید
                options.EncodeType = sg.BarcodeTypes.Code128
                options.Left = 50
                options.Top = 150

                # سند امضا شده را ذخیره کنید
                result = signature.Sign('output.pptx', options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "مدارک خود را با ویژگی‌های امضای پیشرفته بهبود بخشید"
  description: "کتابخانه GroupDocs.Signature for Python via .NET راه‌حل‌های جامعی برای امضای اسناد و پردازش آنها در فرمت‌های متداول ارائه می‌دهد. می‌توانید به راحتی انواع مختلف امضا را اضافه، اصلاح، تأیید یا حذف کنید تا به نیازهای خود پاسخ دهید."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضای انعطاف‌پذیر اسناد"
      content: "در هر صفحه از اسناد پشتیبانی‌شده با متن، تصاویر، بارکدها، کدهای QR یا مهرها امضا کنید. متادیتای پنهان مانند داده‌های EXIF در تصاویر اضافه کنید و با استفاده از گواهی‌های دیجیتال از محافظت از محتوا اطمینان حاصل کنید تا از تغییرات غیرمجاز جلوگیری شود."

    # feature loop
    - title: "جستجو و تأیید امضاها"
      content: "ابزار ما با فعال کردن تأیید امضا، از یکپارچگی اسناد شما اطمینان می‌یابد. همچنین می‌توانید فهرست کاملی از تمام امضاها در یک سند را برای مدیریت آسان بازیابی کنید."

    # feature loop
    - title: "امضاها را به راحتی ویرایش کنید"
      content: "امضاهای موجود را به راحتی اصلاح کنید. متن را تنظیم کنید، عناصر را جابجا کنید یا رنگ‌ها را به صورتی تغییر دهید که به نیازهای سند شما پاسخ دهد."

    # feature loop
    - title: "به راحتی امضاها را حذف کنید"
      content: "با قابلیت کامل CRUD، GroupDocs.Signature for Python via .NET این امکان را به شما می‌دهد که هر امضا غیرمطلوب یا قدیمی را از اسناد خود به سادگی حذف کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ایجاد و قرار دادن یک امضای بارکد"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان یک بارکد سفارشی را در یک سند PPTX درج کرد.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # سندی که باید امضا شود را فراهم کنید
              with sg.Signature('input.pptx') as signature:

                  # متن بارکد و گزینه‌های امضا را تنظیم کنید
                  options = sg.BarcodeSignOptions('Accepted')
                  options.EncodeType = sg.BarcodeTypes.Code39FullASCII

                  # موقعیت بارکد را در صفحه انتخاب کنید
                  options.VerticalAlignment = sg.VerticalAlignment.Top
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left

                  # فاصله بین بارکد و لبه صفحه را تعریف کنید
                  options.Margin = sg.Padding()
                  options.Margin.Top = 180
                  options.Margin.Right = 20

                  # رنگ میله‌های بارکد را مشخص کنید
                  options.ForeColor = sg.Color.Red

                  # سبک فونت برای پیام بارکد را انتخاب کنید
                  options.Font = sg.SignatureFont()
                  options.Font.Size = 12
                  options.Font.FamilyName = 'Arial'

                  # موقعیت متن پیام را تعیین کنید
                  options.CodeTextAlignment = sg.CodeTextAlignment.Above

                  # سند را امضا کرده و ذخیره کنید
                  result = signature.Sign('output.pptx', options)
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
            link: "/examples/signature/formats/signature_barcode.pptx"
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
    title: "ویژگی‌های کلیدی ما را کاوش کنید"
    exclude: "barcode"
    description: "ما گزینه‌ها و عملیات مختلفی برای نیازهای سند شما ارائه می‌دهیم."
    items: 
          
        # operation loop 1
        - name: "امضاهای الکترونیکی"
          operation: "esign"
          link: "/signature/python-net/esign/pptx/"
          description: "انواع مختلفی از امضاها را به فرمت‌های فایل پشتیبانی‌شده اضافه کنید"

        # operation loop 2
        - name: "متن را به اسناد اضافه کنید"
          operation: "text"
          link: "/signature/python-net/text/pptx/"
          description: "محتوای سند را با امضاهای متنی قابل تنظیم تقویت کنید"

        # operation loop 3
        - name: "امضاهای تصویری"
          operation: "image"
          link: "/signature/python-net/image/pptx/"
          description: "هر تصویری را در هر نقطه‌ای از سند قرار دهید"

        # operation loop 4
        - name: "ایجاد بارکد"
          operation: "barcode"
          link: "/signature/python-net/barcode/pptx/"
          description: "بارکدهای مختلفی را ایجاد و در اسناد پشتیبانی‌شده درج کنید"

        # operation loop 5
        - name: "ایجاد QR کد"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pptx/"
          description: "QR کدها را برای امضای اسناد تولید کنید"
          
        # operation loop 6
        - name: "گواهی‌های دیجیتال"
          operation: "digital"
          link: "/signature/python-net/digital/pptx/"
          description: "اسناد را با گواهی‌های دیجیتال ایمن کنید"

        # operation loop 7
        - name: "امضاهای مهر"
          operation: "stamp"
          link: "/signature/python-net/stamp/pptx/"
          description: "از سازنده مهر برای ایجاد مهرهای دایره‌ای یا مربعی سفارشی استفاده کنید"
          
        # operation loop 8
        - name: "جستجوی امضاها"
          operation: "search"
          link: "/signature/python-net/search/pptx/"
          description: "هر امضای قبلاً اضافه‌شده را در سند پیدا کنید"
          
        # operation loop 9
        - name: "تأیید امضاء"
          operation: "verify"
          link: "/signature/python-net/verify/pptx/"
          description: "پس از اعمال امضاها، صحت آن‌ها را بررسی کنید"
          
        # operation loop 10
        - name: "تغییر امضاها"
          operation: "modify"
          link: "/signature/python-net/modify/pptx/"
          description: "امضاهای مختلف را در داخل سند ویرایش نمایید"
          
        # operation loop 11
        - name: "حذف امضاها"
          operation: "delete"
          link: "/signature/python-net/delete/pptx/"
          description: "مجموعه وسیعی از امضاهای قبلاً اعمال‌شده را حذف کنید"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "امضای اسناد در فرمت‌های متنوع"
    exclude: "PPTX"
    description: "API Python via .NET از امضای بیش از ۶۰ فرمت فایل پشتیبانی می‌کند و به شما این امکان را می‌دهد که انواع مختلف امضاها را به هر صفحه یا مکان خاصی در اسناد خود اضافه کنید."
    items: 
          
        # format loop 1
        - name: "اضافه کردن بارکد به PDF"
          format: "PDF"
          link: "/signature/python-net/barcode/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "اضافه کردن بارکد به DOCX"
          format: "DOCX"
          link: "/signature/python-net/barcode/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "اضافه کردن بارکد به JPEG"
          format: "JPEG"
          link: "/signature/python-net/barcode/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "اضافه کردن بارکد به PPTX"
          format: "PPTX"
          link: "/signature/python-net/barcode/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "اضافه کردن بارکد به XLSX"
          format: "XLSX"
          link: "/signature/python-net/barcode/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---