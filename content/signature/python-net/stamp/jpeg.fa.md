



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:49
draft: false
lang: fa
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "ایجاد مهرهای گرد و مربعی در JPEG با استفاده از Python"
head_description: "ایجاد و درج مهرهای شخصی‌سازی شده در فایل‌های JPEG با API GroupDocs.Signature for Python via .NET."

############################# Header ############################
title: "ایجاد مهرها برای JPEG" 
description: "مهرهای طراحی‌شده سفارشی را به هر بخشی از اسناد خود با GroupDocs.Signature for Python via .NET اضافه کنید، که انعطاف‌پذیری بالایی برای قرارگیری و تنظیمات به نیازهای تجاری شما ارائه می‌دهد."
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
    title: "مروری بر GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) ابزاری جامع است که به شما امکان می‌دهد انواع مختلفی از امضاها را به اسناد اضافه کنید، از جمله مهرهای سفارشی. با پشتیبانی از بیش از 60 فرمت فایل—از PDF و اسناد Word تا تصاویر و فایل‌های ZIP—شما می‌توانید اسناد خود را با متن، تصویر، بارکد، متا دیتا، گواهی‌های دیجیتال و مهرها غنی کنید. همچنین کنترل کامل برای جستجو، تأیید، ویرایش یا حذف هر امضای اعمال شده را دارید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه یک مهر به JPEG با استفاده از Python اضافه کنیم"
    content: |
      [GroupDocs.Signature](/signature/python-net/) ابزارهای قدرتمندی برای ایجاد مهرها برای بهبود برنامه‌های Python via .NET ارائه می‌دهد. از آن برای طراحی و پیاده‌سازی مهرهای سفارشی برای صفحات اسناد خود استفاده کنید.
      
      1. سند JPEG  که می‌خواهید مهر بزنید را ارائه دهید.
      2. از StampSignOptions برای تنظیم تمام تنظیمات لازم استفاده کنید.
      3. اگر ضروری باشد، چندین خط مهر اضافه کنید.
      4. مهر را اعمال کرده و سند به‌روز شده را ذخیره کنید.
   
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

            # مسیر سند را به نمونه Signature متصل کنید
            with sg.Signature('input.jpeg') as signature:

                # تنظیمات StampSignOptions را با جزئیات لازم تنظیم کنید
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # یک یا چند خط به مهر اضافه کنید
                outerLine = sg.StampLine()
                outerLine.Text = "* The Best Company *"
                outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                outerLine.Font = sg.SignatureFont()
                outerLine.Font.Size = 12
                outerLine.Font.FamilyName = "Arial"
                outerLine.Height = 22
                outerLine.TextBottomIntent = 6
                outerLine.TextColor = sg.Color.WhiteSmoke
                outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                options.OuterLines.Add(outerLine)

                # سند را با مهر اعمال‌شده ذخیره کنید
                result = signature.Sign("output.jpeg", options)
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "استفاده از امضاها برای تأمین امنیت و بهبود یکپارچگی اسناد"
  description: "با کتابخانه GroupDocs.Signature for Python via .NET، می‌توانید به‌صورت یکپارچه قابلیت‌های امضا را به اسناد خود اضافه کنید. به‌سادگی مهرهای سفارشی و انواع دیگر امضاها را ایجاد، ویرایش، تأیید یا حذف کنید و به بهبود و امنیت کارکردهای سند خود بپردازید."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "امضاهای مهر با قدرت GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضای کامل سند"
      content: "اسناد خود را با افزودن امضاهایی مانند متن، تصاویر، بارکدها، کدهای QR و مهرها به هر موقعیتی در هر صفحه ارتقا دهید. متا داده‌های جاسازی‌شده را مدیریت کرده و گواهی‌های دیجیتال را برای جلوگیری از تغییرات غیرمجاز اعمال کنید."

    # feature loop
    - title: "جستجو و تأیید امضا به‌صورت مؤثر"
      content: "پس از امضا، از ابزارهای جستجوی پیشرفته برای پیدا کردن تمام امضاهای جاسازی شده استفاده کنید. به‌سادگی داده‌های امضا را تأیید یا مدیریت کنید تا یکپارچگی سند را تضمین کنید."

    # feature loop
    - title: "ویرایش و شخصی‌سازی امضاها"
      content: "تغییرات لازم را در امضاهای قبلاً اضافه‌شده اعمال کنید. چه بخواهید محتوا، موقعیت، اندازه یا رنگ ویرایش شود، GroupDocs.Signature for Python via .NET به شما کنترل کامل برای تنظیم امضاها را می‌دهد."

    # feature loop
    - title: "حذف امضاها به‌سادگی"
      content: "اگر نیاز به حذف امضاها دارید، GroupDocs.Signature for Python via .NET تمام ابزارهای لازم برای حذف هر نوع شامل مهرها و گواهی‌های دیجیتال را ارائه می‌دهد و به شما کمک می‌کند اسناد خود را به‌روز و مطابق با قوانین نگه دارید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "چگونه مهرهای سفارشی به اسناد اضافه کنیم"
      content: |
        این مثال نشان می‌دهد که چگونه مهرهای سفارشی با جزئیات متنی خاص به یک سند ایجاد و درج کنید.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # سندی را که می‌خواهید مهر بزنید ارائه دهید
              with sg.Signature('input.jpeg') as signature:

                    # تنظیمات مهر را با تنظیمات دلخواه خود تنظیم کنید
                    options = sg.StampSignOptions()

                    # اندازه و محل قرارگیری مهر را بر روی صفحه تعریف کنید
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # خطوط دایره‌ای بیرونی با متن اضافه کنید
                    outerLine = sg.StampLine()
                    outerLine.Text = "* The best  choice *"
                    outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                    outerLine.Font = sg.SignatureFont()
                    outerLine.Font.Size = 12
                    outerLine.Font.FamilyName = "Arial"
                    outerLine.Height = 22
                    outerLine.TextBottomIntent = 6
                    outerLine.TextColor = sg.Color.WhiteSmoke
                    outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                    options.OuterLines.Add(outerLine)

                    # به‌اختیاری، خطوط مربعی داخلی را اضافه کنید
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # سند مهر خورده را نهایی کرده و ذخیره کنید
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
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
    title: "امکانات کلیدی را بررسی کنید"
    exclude: "stamp"
    description: "دامنه وسیعی از گزینه‌ها برای ایجاد، مدیریت و حذف امضاها را پیدا کنید که به شما کنترل کامل بر روی کارکردهای سند می‌دهد."
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
    title: "اعمال مهرها به فرمت‌های مختلف سند"
    exclude: "JPEG"
    description: "با API GroupDocs.Signature، می‌توانید مهرهای سفارشی را به بیش از 60 نوع فایل استاندارد اضافه کنید. به‌سادگی مهرها را در هر نقطه‌ای از اسناد خود قرار دهید و شخصی‌سازی و پیگیری را بهبود بخشید."
    items: 
          
        # format loop 1
        - name: "مهر زدن PDF"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "مهر زدن DOCX"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "مهر زدن JPEG"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "مهر زدن PPTX"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "مهر زدن XLSX"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---