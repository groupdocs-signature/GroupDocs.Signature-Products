



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:15
draft: false
lang: fa
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "اضافه کردن امضای متنی به DOCX با استفاده از Python"
head_description: "از API Python برای وارد کردن امضاهای متنی در فایل‌های DOCX استفاده کنید و از فرمت‌هایی مانند PDF، Word، Excel، PowerPoint، تصاویر و ZIP پشتیبانی کنید."

############################# Header ############################
title: "اضافه کردن امضای متنی به DOCX" 
description: "امضاهای متنی سفارشی را بدون دردسر به اسناد خود با استفاده از GroupDocs.Signature for Python via .NET اضافه کنید. کارهای خود را با گزینه‌های سفارشی‌سازی امضا ساده کنید."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "امتحان کنید، امروز رایگان"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "قدرت GroupDocs.Signature for Python via .NET را کشف کنید"
    link: "/signature/python-net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) یک پلتفرم جامع برای تعبیه امضاهای متنی قابل تنظیم ارائه می‌دهد که کارکردهای اسناد را هموارتر می‌کند. محتوای امضاها را در اسناد مختلف شخصی‌سازی کنید تا کارایی را افزایش داده و مدیریت اسناد را بهبود ببخشید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه امضاهای متنی DOCX با Python ایجاد کنیم"
    content: |
      [GroupDocs.Signature](/signature/python-net/) یکپارچگی آسان امضای متنی در فایل‌های DOCX را در برنامه‌های Python via .NET ممکن می‌سازد. به سرعت امکانات را به محصولات خود با این راه‌حل اضافه کنید.
      
      1. سند DOCX را به سازنده Signature ارائه دهید.
      2. تنظیمات TextSignOptions را با متن امضای خود ایجاد کنید.
      3. خصوصیات بصری امضا را تنظیم کنید.
      4. امضا را به صفحات دلخواه سند اضافه کنید.
   
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

            # دستور Signature را با مسیر سند اولیه‌سازی کنید
            with sg.Signature('input.docx') as signature:

                # تنظیمات TextSignOptions را با متن امضای موردنظر خود پیکربندی کنید
                options = sg.TextSignOptions("Approved")

                # رنگ و فونت امضا را انتخاب کنید
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # امضای متنی را به سند اعمال کنید
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "مدیریت کامل امضاهای متنی"
  description: "GroupDocs.Signature for Python via .NET به شما کمک می‌کند تا با اضافه کردن امضاهای متنی سفارشی به فرمت‌های محبوب، کارکردهای سندی خود را مدیریت کنید. به راحتی ظاهر، مکان و محتوای امضاها را مطابق نیازهای خود کنترل کنید."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "کشف ویژگی‌های GroupDocs.Signature"
  features:
    # feature loop
    - title: "امضاهای متنی انعطاف‌پذیر"
      content: "انواع مختلف امضاها—متن، تصاویر، بارکدها، کدهای QR و مهرها—را به هر صفحه سند اضافه کنید. از متاداده برای درج اطلاعات مخفی استفاده کنید و فایل‌های خود را با گواهی‌های دیجیتال ایمن کنید."

    # feature loop
    - title: "بررسی و جستجوی امضاها"
      content: "از ابزارهای پیشرفته برای بررسی صحت سندهای امضا شده خود استفاده کنید. تمام امضاها را در یک فایل برای اعتبارسنجی بیشتر جستجو و تحلیل کنید."

    # feature loop
    - title: "ویرایش یا حذف امضاها"
      content: "به راحتی محتوای امضاهای موجود را به‌روز کنید یا مکان آن‌ها را تغییر دهید. امضاهای قدیمی را حذف کنید تا اسناد شما به‌روز بمانند."

    # feature loop
    - title: "امضاهای متنی مخصوص"
      content: "امضاهای متنی خاص به اسناد، مانند واترمارک برای فایل‌های Word یا مهر برای PDF، اضافه کنید و کنترل و سفارشی‌سازی بیشتری را ارائه دهید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "اضافه کردن امضاهای متنی به اسناد"
      content: |
        یاد بگیرید چگونه امضاهای متنی را به اسناد اضافه کنید تا فرآیندهای خود را تسهیل کنید.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # سند مورد نظر برای امضا را انتخاب کنید
              with sg.Signature('input.docx') as signature:

                    # گزینه‌های متنی را با محتوای دلخواه تنظیم کنید
                    options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                    # اندازه و مکان امضا را تعریف کنید
                    options.Left = 100
                    options.Top = 180
                    options.Width = 230
                    options.Height = 30

                    # فاصله از لبه‌های صفحه را تنظیم کنید
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # رنگ متن و سبک فونت را انتخاب کنید
                    options.ForeColor = sg.Color.Red
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # یک حاشیه دور امضای متنی اضافه کنید
                    options.Border = sg.Border()
                    options.Border.Color = sg.Color.Red
                    options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                    options.Border.Transparency = 0.5
                    options.Border.Visible = True
                    options.Border.Weight = 2

                    # در صورت نیاز پس‌زمینه را سفارشی کنید
                    options.Background = sg.Background()
                    options.Background.Color = sg.Color.Yellow
                    options.Background.Transparency = 0.8

                    # اختیاری، امضا را به عنوان تصویر برای سازگاری ذخیره کنید
                    options.SignatureImplementation = sg.TextSignatureImplementation.Image

                    # سند را با امضای تعبیه‌شده ذخیره کنید
                    result = signature.Sign("output.docx", options)
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
            link: "/examples/signature/formats/signature_text.docx"
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
    title: "ویژگی‌های پیشرفته امضا"
    exclude: "text"
    description: "API ما از مدیریت کامل چرخه زندگی برای هفت نوع امضا پشتیبانی می‌کند، به شما اجازه می‌دهد امضاها را ایجاد، مدیریت، بررسی و سفارشی‌سازی کنید."
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
    title: "وارد کردن امضاهای متنی در فرمت‌های متعدد"
    exclude: "DOCX"
    description: "با API Python via .NET می‌توانید امضاهای متنی را به انواع اسناد Office اضافه کنید و کنترل کامل بر چرخه زندگی سند را به‌دست آورید و امنیت را بهبود ببخشید."
    items: 
          
        # format loop 1
        - name: "امضای متنی PDF"
          format: "PDF"
          link: "/signature/python-net/text/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "امضای متنی DOCX"
          format: "DOCX"
          link: "/signature/python-net/text/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "امضای متنی JPEG"
          format: "JPEG"
          link: "/signature/python-net/text/jpeg/"
          description: "تصویر JPEG"
          
        # format loop 4
        - name: "امضای متنی PPTX"
          format: "PPTX"
          link: "/signature/python-net/text/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 5
        - name: "امضای متنی XLSX"
          format: "XLSX"
          link: "/signature/python-net/text/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---