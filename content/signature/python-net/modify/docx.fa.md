



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:18
draft: false
lang: fa
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "ویرایش امضای DOCX در برنامه‌های Python"
head_description: "از API Python برای اصلاح امضاها در اسناد DOCX، از جمله فایل‌های PDF، Word، Excel، ارائه‌ها و تصاویر استفاده کنید."

############################# Header ############################
title: "به‌راحتی امضاهای DOCX را به‌روز کنید" 
description: "کنترل کامل برای ویرایش انواع امضاهای الکترونیکی در فرمت‌های اصلی مانند PDF، Word، Excel، ارائه‌ها و تصاویر را با ویژگی‌های پیشرفته GroupDocs.Signature for Python via .NET به دست آورید."
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
    title: "قابلیت‌های GroupDocs.Signature for Python via .NET را کشف کنید"
    link: "/signature/python-net/"
    link_title: "بیشتر بخوانید"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) فقط امضای مستندات را ارائه نمی‌دهد، بلکه به شما این امکان را می‌دهد که به راحتی امضاهای موجود را ویرایش کنید. ویژگی‌های امضاها را در فرمت‌های پرکاربردی مانند PDF، Word، Excel و ارائه‌های پاورپوینت با حداقل تلاش تنظیم کنید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه امضاها را در DOCX با استفاده از Python ویرایش کنیم"
    content: |
      [GroupDocs.Signature](/signature/python-net/) به توسعه‌دهندگان Python via .NET امکان می‌دهد که امضاهای متنی که در فایل‌های DOCX قرار داده شده‌اند را ویرایش کنند. قابلیت‌های پیشرفته را به برنامه‌های Python via .NET خود اضافه کنید.
      
      1. سند DOCX را به نمونه Signature بارگذاری کنید.
      2. فهرستی از تمام امضاها در سند را بازیابی کنید.
      3. محتوای هر امضای شناسایی‌شده را ویرایش کنید.
      4. نتایج تغییرات امضا را تأیید کنید.
   
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

            # یک شی Signature با مسیر سند ایجاد کنید
            with sg.Signature('input.docx') as signature:

                # جستجوی امضاهای متنی در سند
                options = sg.TextSearchOptions()
                signatures = signature.Search(options)

                if signatures.Count > 0:

                    # محتوای اولین امضای پیدا شده را به‌روز کنید
                    textSignature = signatures[0]
                    textSignature.Text = "New Text"
                    result = signature.Update(textSignature)

                    # نتایج به‌روزرسانی امضا را تأیید کنید
                    if result:
                        print("\nSignature was updated successfully")
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "مدیریت کامل امضاها برای اسناد"
  description: "GroupDocs.Signature for Python via .NET روند کاری مستندات شما را ساده می‌کند و به شما امکان می‌دهد به راحتی امضاها را به مستندات اضافه، به‌روز، جستجو، تأیید یا حذف کنید و این کار را در تمام فرمت‌های اصلی فایل انجام دهید."
  image: "/img/signature/features_modify.webp" # 500x500 px
  image_description: "ویرایش پیشرفته امضا"
  features:
    # feature loop
    - title: "امضای انعطاف‌پذیر مستندات"
      content: "امضای گسترده‌ای از جمله متن، تصاویر، بارکدها و مهرها را به هر قسمت از مستند خود اعمال کنید. متاداده‌های درون‌ساخته مانند داده‌های EXIF در تصاویر را تغییر دهید و مستندات را در برابر تغییرات غیرمجاز با استفاده از گواهینامه‌های دیجیتال محافظت کنید."

    # feature loop
    - title: "جستجو و تأیید امضا"
      content: "با ابزارهای قدرتمند ما به راحتی امضاها را تأیید کنید. یک فهرست کامل از امضاها در یک سند را بازیابی کنید که تأیید سریع و دقیقی را تضمین می‌کند."

    # feature loop
    - title: "به‌روزرسانی ساده امضا"
      content: "به راحتی امضاهای قبلاً درون‌ساخته شده را به‌روز کنید. محتوای امضا، سبک، مکان یا هر جنبه دیگری از امضا را تنظیم کنید تا با نیازهای جدید مطابقت داشته باشد."

    # feature loop
    - title: "حذف بی‌دردسر امضا"
      content: "کنترل کامل بر مدیریت امضاها را به دست آورید و قادر باشید هر نوع امضا را از مستند خود حذف کنید و این به شما انعطاف‌پذیری کامل در محتوای آن را می‌دهد."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ویرایش امضای بارکد"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توانید برنامه‌نویسی امضای بارکد را در یک سند ویرایش کنید.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # یک سندی که حاوی امضای بارکد است را بارگذاری کنید
              with sg.Signature('input.docx') as signature:

                  # به جستجوی تمامی امضاهای بارکد موجود بپردازید
                  options = sg.BarcodeSearchOptions()
                  signatures = signature.Search(options)

                  if signatures.Count > 0:

                      # موقعیت اولین بارکد پیدا شده را تغییر داده و سند را ذخیره کنید
                      barcodeSignature = signatures[0]
                      barcodeSignature.Left = 100
                      barcodeSignature.Top = 100
                      result = signature.Update(barcodeSignature)

                      # تأیید کنید که تغییر بارکد با موفقیت انجام شده است
                      if result:
                          print("\nBarcode was updated successfully.")
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
    title: "کاوش در مجموعه کامل ویژگی‌ها"
    exclude: "modify"
    description: "فهرست گسترده فرمت‌ها و عملیات‌های امضاهای پشتیبانی‌شده توسط پلتفرم ما را مرور کنید."
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
    title: "ویرایش امضاها در چندین فرمت"
    exclude: "DOCX"
    description: "با استفاده از API Python via .NET، می‌توانید به راحتی اسناد امضا شده را ویرایش کنید. داده‌های امضا را از فرمت‌های پشتیبانی شده استخراج و به‌روز کنید و کنترل کامل بر یکپارچگی سند خود را حفظ کنید."
    items: 
          
        # format loop 1
        - name: "تغییر امضاهای PDF"
          format: "PDF"
          link: "/signature/python-net/modify/pdf/"
          description: "فرمت مستند قابل حمل Adobe"
          
        # format loop 2
        - name: "ویرایش امضاهای DOCX"
          format: "DOCX"
          link: "/signature/python-net/modify/docx/"
          description: "مستند XML باز Microsoft Word"
          
        # format loop 3
        - name: "ویرایش امضاهای PPTX"
          format: "PPTX"
          link: "/signature/python-net/modify/pptx/"
          description: "ارائه XML باز PowerPoint"
          
        # format loop 4
        - name: "تغییر امضاهای XLSX"
          format: "XLSX"
          link: "/signature/python-net/modify/xlsx/"
          description: "صفحه گسترده XML باز Microsoft Excel"


          

---