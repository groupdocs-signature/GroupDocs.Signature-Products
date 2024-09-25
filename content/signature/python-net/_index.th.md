---
############################# Static ############################
layout: "landing"
date: 2024-09-25T13:59:03
draft: false

lang: th
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
  for: "สำหรับ"

actions:
  main: "{index-content-python-net.actions_main}"
  main_link: "https://pypi.org/project/groupdocs-signature-net/"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
  title: "พร้อมที่จะเริ่มต้นหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Signature ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} เปิดตัวแล้ว"
  notes: "ดูว่ามีอะไรใหม่"
  downloads: "ดาวน์โหลด"

code:
  title: "{index-content-python-net.code_title}"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
  install: "pip install groupdocs-signature-net"
  content: |
    ```python {style=abap}   
    import groupdocs.signature as sg

    def run():

        # เลือกเอกสาร PDF
        with sg.Signature('sample.pdf') as signature:

            # ระบุข้อความ
            options = sg.TextSignOptions("John Smith")
    
            # กำหนดสี
            options.ForeColor = sg.Color.Red
    
            # ลงนามในเอกสารและบันทึกลงไฟล์
            signature.Sign('signed.pdf', options)
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature ภาพรวม"
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
  title: "ความเป็นอิสระของแพลตฟอร์ม"
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
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    {index-content-python-net.formats_description}
  groups:
    # group loop
    - color: "green"
      content: |
        ### รูปแบบของ Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### รูปภาพและรูปแบบอื่นๆ
        * **แบบพกพา:** PDF
        * **รูปภาพ:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **รูปแบบสำนักงานอื่นๆ:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### รูปแบบอื่นๆ
        * **เว็บ:** HTML, MHTML
        * **หอจดหมายเหตุ:** ZIP, TAR, 7Z
        * **ใบรับรอง:** PFX

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
  title: "ตัวอย่างโค้ด"
  description: "{index-content-python-net.code_samples_description}"
  items:
    # code sample loop
    - title: "{index-content-python-net.code_title_sample_1}"
      content: |
        {index-content-python-net.code_samples_sample_1_content_1} {index-content-python-net.code_samples_sample_1_content_2}
        {{< landing/code title="วิธีใส่รหัส QR เป็น PDF">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # โหลดเอกสารเพื่อลงนาม
            with sg.Signature('file_to_sign.pdf') as signature:

                # สร้างตัวเลือกโค้ด QR พร้อมข้อความที่กำหนดไว้ล่วงหน้า
                options = sg.QrCodeSignOptions('The document is approved by John Smith')
        
                # กำหนดค่าประเภทและตำแหน่งการเข้ารหัสโค้ด QR บนเพจ
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 100
                options.Top = 100
            
                # ลงนามในเอกสารและบันทึกเป็นไฟล์ผลลัพธ์
                signature.Sign('file_with_QR.pdf', options)
        ```
        {{< /landing/code >}}

    # code sample loop
    - title: "{index-content-python-net.code_title_sample_2}"
      content: |
        {index-content-python-net.code_samples_sample_2_content_1} {index-content-python-net.code_samples_sample_2_content_2}
        {{< landing/code title="ต่อไปนี้คือวิธีการตรวจสอบความสมบูรณ์ของเอกสาร">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # โหลดเอกสารที่จะเซ็นชื่อแบบดิจิทัล
            with sg.Signature('file_to_sign.docx') as signature:
        
                # ระบุตัวเลือกการเซ็นชื่อดิจิทัลและระบุเส้นทางไปยังไฟล์ใบรับรอง
                options = sg.DigitalSignOptions('certificate.pfx')

                # ตั้งรหัสผ่านใบรับรอง
                options.Password = '1234567890'

                # ลงนามในเอกสารและบันทึกลงในเส้นทางที่ต้องการ
                signature.Sign('digitally_signed.docx', options)
        ```
        {{< /landing/code >}}

---
