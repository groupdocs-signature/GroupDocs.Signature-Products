---
############################# Static ############################
layout: "landing"
date: 2024-09-25T13:59:03
draft: false

lang: fa
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java" 
    # supported_platforms loop
    - title: "Python"
      tag: "python-net"  

############################# Head ############################
head_title: "{index-content-python-net.head_title}"
head_description: "{index-content-python-net.head_description}"

############################# Header ############################
title: "{index-content-python-net.title}"
description: "{index-content-python-net.description}"
words:
  for: "برای"

actions:
  main: "{index-content-python-net.actions_main}"
  main_link: "https://pypi.org/project/groupdocs-signature-net/"
  alt: "صدور مجوز"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
  title: "برای شروع آماده اید؟"
  description: "ویژگی های GroupDocs.Signature را به صورت رایگان امتحان کنید یا درخواست مجوز کنید"

release:
  title: "نسخه {0} منتشر شد"
  notes: "ببینید چه چیز جدیدی است"
  downloads: "دانلودها"

code:
  title: "{index-content-python-net.code_title}"
  more: "نمونه های بیشتر"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
  install: "pip install groupdocs-signature-net"
  content: |
    ```python {style=abap}   
    import groupdocs.signature as sg

    def run():

        # سند PDF را انتخاب کنید
        with sg.Signature('sample.pdf') as signature:

            # متن ارائه دهید
            options = sg.TextSignOptions("John Smith")
    
            # تنظیم رنگ
            options.ForeColor = sg.Color.Red
    
            # سند را امضا کرده و در فایل ذخیره کنید
            signature.Sign('signed.pdf', options)
    ```

############################# Overview ############################
overview:
  enable: true
  title: "نمای کلی GroupDocs.Signature"
  description: "{index-content-python-net.overview_description}"
  features:
    # feature loop
    - title: "{index-content-python-net.overview_feature_1.title}"
      content: "{index-content-python-net.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-python-net.overview_feature_2.title}"
      content: "{index-content-python-net.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-python-net.overview_feature_3.title}"
      content: "{index-content-python-net.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال سکو"
  description: "{index-content-python-net.platforms_description}"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت های فایل پشتیبانی شده"
  description: |
    {index-content-python-net.formats_description}
  groups:
    # group loop
    - color: "green"
      content: |
        ### فرمت های مایکروسافت آفیس
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### تصاویر و فرمت های دیگر
        * **قابل حمل:** PDF
        * **تصاویر:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **سایر فرمت های اداری:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### فرمت های دیگر
        * **وب:** HTML, MHTML
        * **آرشیوها:** ZIP, TAR, 7Z
        * **گواهینامه ها:** PFX

############################# Features ############################
features:
  enable: true
  title: "{index-content-python-net.features.title}"
  description: "{index-content-python-net.features.description}"

  items:
    # feature loop
    - icon: "sign"
      title: "{index-content-python-net.features.feature_1.title}"
      content: "{index-content-python-net.features.feature_1.content}"

    # feature loop
    - icon: "custom"
      title: "{index-content-python-net.features.feature_2.title}"
      content: "{index-content-python-net.features.feature_2.content}"

    # feature loop
    - icon: "password"
      title: "{index-content-python-net.features.feature_3.title}"
      content: "{index-content-python-net.features.feature_3.content}"

    # feature loop
    - icon: "protect"
      title: "{index-content-python-net.features.feature_4.title}"
      content: "{index-content-python-net.features.feature_4.content}"

    # feature loop
    - icon: "convert"
      title: "{index-content-python-net.features.feature_5.title}"
      content: "{index-content-python-net.features.feature_5.content}"

    # feature loop
    - icon: "preview"
      title: "{index-content-python-net.features.feature_6.title}"
      content: "{index-content-python-net.features.feature_6.content}"

    # feature loop
    - icon: "search"
      title: "{index-content-python-net.features.feature_7.title}"
      content: "{index-content-python-net.features.feature_7.content}"

    # feature loop
    - icon: "validate"
      title: "{index-content-python-net.features.feature_8.title}"
      content: "{index-content-python-net.features.feature_8.content}"

    # feature loop
    - icon: "update"
      title: "{index-content-python-net.features.feature_9.title}"
      content: "{index-content-python-net.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه کد"
  description: "{index-content-python-net.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-python-net.code_title_sample_1}"
      content: |
        {index-content-python-net.code_samples_sample_1_content_1} {index-content-python-net.code_samples_sample_1_content_2}
        {{< landing/code title="نحوه قرار دادن کد QR در PDF.">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # سند را برای امضا بارگیری کنید
            with sg.Signature('file_to_sign.pdf') as signature:

                # گزینه های کد QR را با متن از پیش تعریف شده ایجاد کنید
                options = sg.QrCodeSignOptions('The document is approved by John Smith')
        
                # نوع و موقعیت رمزگذاری کد QR را در صفحه پیکربندی کنید
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 100
                options.Top = 100
            
                # سند را امضا کنید و آن را به عنوان فایل نتیجه ذخیره کنید
                signature.Sign('file_with_QR.pdf', options)
        ```
        {{< /landing/code >}}

    # code sample loop
    - title: "{index-content-python-net.code_title_sample_2}"
      content: |
        {index-content-python-net.code_samples_sample_2_content_1} {index-content-python-net.code_samples_sample_2_content_2}
        {{< landing/code title="در اینجا نحوه اطمینان از یکپارچگی سند آمده است.">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # سند را برای امضای دیجیتال بارگیری کنید
            with sg.Signature('file_to_sign.docx') as signature:
        
                # گزینه های امضای دیجیتال را مشخص کنید و مسیر فایل گواهی را ارائه دهید
                options = sg.DigitalSignOptions('certificate.pfx')

                # رمز عبور گواهی را تنظیم کنید
                options.Password = '1234567890'

                # سند را امضا کرده و در مسیر مورد نظر ذخیره کنید
                signature.Sign('digitally_signed.docx', options)
        ```
        {{< /landing/code >}}

---
