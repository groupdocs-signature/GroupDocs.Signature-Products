



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:23
draft: false
lang: th
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "สร้าง QR Code สำหรับไฟล์ PDF โดยใช้ Python"
head_description: "ใช้ API GroupDocs.Signature ในการสร้างและฝัง QR Code ในไฟล์ PDF เพื่อเพิ่มฟังก์ชันการทำงานที่หลากหลายให้กับเอกสารของคุณ."

############################# Header ############################
title: "สร้าง QR Code สำหรับ PDF" 
description: "สร้างบาร์โค้ด 2 มิติจากข้อมูลข้อความหรือข้อมูลตัวเลขและใช้งานได้กับหลายหน้าและรูปแบบ รวมถึง PDF, Word, Excel และอื่นๆ ด้วย GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ทดลองใช้ฟรี"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "สำรวจฟีเจอร์ของ GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) มีความสามารถที่หลากหลายช่วยให้ผู้ใช้สามารถสร้างและฝังลายเซ็นประเภทต่างๆ ลงในฟอร์แมตเอกสารหลัก ๆ ไม่ว่าจะเป็น PDF, Word, Excel, PowerPoint หรือภาพ ถ้าต้องการพัฒนาเอกสารของคุณด้วยลายเซ็นประเภทข้อความ, รูปภาพ, บาร์โค้ด, QR Code, เมตาดาต้า, ลายเซ็นดิจิทัล หรือ สแตมป์.

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนในการสร้างและแทรก QR Code ใน PDF"
    content: |
      [GroupDocs.Signature](/signature/python-net/) ช่วยให้คุณสร้าง QR Code ในรูปแบบที่นิยมและวางลงบนหน้าของ PDF รองรับ QR Code มากกว่า 10 ประเภท คุณสามารถรวมฟังก์ชันนี้เข้ากับแอปพลิเคชัน Python via .NET ได้อย่างราบรื่น พัฒนาเอกสารของคุณด้วยลายเซ็น QR Code โดยใช้ผลิตภัณฑ์ของเรา.
      
      1. รับไฟล์หรือสตรีม PDF ที่จะมีการเพิ่ม QR Code.
      2. ระบุข้อความที่จำเป็นใน QrCodeSignOptions.
      3. ปรับแต่งการตั้งค่าทางสายตาเช่น สี ตำแหน่ง และขนาด.
      4. บันทึกเอกสารที่มี QR Code ฝังอยู่.
   
    code:
      platform: "python-net"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "ตัวอย่างลายเซ็น"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # เริ่มต้นอินสแตนซ์ Signature ใหม่ด้วยเอกสาร
            with sg.Signature('input.pdf') as signature:

                # ใช้ QrCodeSignOptions เพื่อฝัง QR Code ลงในเอกสาร
                options = sg.QrCodeSignOptions("Text Content")

                # ระบุประเภทลายเซ็นและตั้งค่าตำแหน่งบนหน้า
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # บันทึกเอกสารที่มี QR Code ฝังอยู่
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "การรวมลายเซ็นอย่างครบถ้วนสำหรับเอกสาร"
  description: "ด้วย API GroupDocs.Signature for Python via .NET ผู้ใช้สามารถสร้าง แก้ไข ค้นหา ยืนยัน และลบลายเซ็นประเภทต่าง ๆ ทำให้การทำงานเอกสารเป็นไปอย่างมีประสิทธิภาพ."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "ใช้ลายเซ็นประเภทต่าง ๆ"
      content: "GroupDocs.Signature รองรับการใช้ลายเซ็นประเภทข้อความ, รูปภาพ, บาร์โค้ด, QR Code, และ สแตมป์ลงในเอกสารใด ๆ คุณสามารถวางลายเซ็นได้อย่างแม่นยำในทุกหน้าและบริหารจัดการข้อมูลเมตาได้อย่างง่ายดาย ป้องกันเอกสารของคุณจากการแก้ไขที่ไม่ได้รับอนุญาตด้วยใบรับรองดิจิทัล."

    # feature loop
    - title: "ค้นหาและยืนยันลายเซ็น"
      content: "ตรวจสอบลายเซ็นในเอกสารเพื่อความถูกต้องและความถูกต้องแม่นยำโดยใช้เครื่องมือตรวจสอบขั้นสูง รับรายชื่อแบบละเอียดของลายเซ็นทั้งหมดที่ฝังอยู่ในเอกสารได้ง่ายดายเพื่อให้มีการตรวจสอบที่ดียิ่งขึ้น."

    # feature loop
    - title: "ปรับปรุงลายเซ็นที่มีอยู่"
      content: "คุณสามารถอัปเดตลายเซ็นที่ได้ใช้ไปแล้วโดยการปรับเนื้อหา ตำแหน่ง สี ขนาด และองค์ประกอบอื่น ๆ เพื่อให้เหมาะสมกับความต้องการเฉพาะของคุณ."

    # feature loop
    - title: "ลบลายเซ็นได้อย่างรวดเร็ว"
      content: "ทำให้การจัดการเอกสารราบรื่นโดยการลบลายเซ็นที่ไม่ต้องการได้อย่างรวดเร็ว ไม่ว่าจะเป็นใบรับรองดิจิทัลหรือลายเซ็นประเภทอื่น การลบสามารถทำได้อย่างมีประสิทธิภาพ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ปรับแต่ง QR Code ที่สร้างขึ้น"
      content: |
        ตัวอย่างนี้แสดงวิธีการวาง QR Code ที่ปรับปรุงลงบนหน้าของ PDF.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # นำเอกสารที่ต้องการลายเซ็นไปและส่งไปยัง Signature
              with sg.Signature('input.pdf') as signature:

                    # ตั้งค่าตัวเลือก QR Code พร้อมข้อความที่จำเป็น
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # กำหนดตำแหน่งของ QR Code บนหน้า
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # ตั้งค่าขอบสำหรับลายเซ็น
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # เลือกสีของ QR Code
                    options.ForeColor = sg.Color.Red

                    # กำหนดตัวเลือกฟอนต์สำหรับข้อความ
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # กำหนดสีพื้นหลังและแปรงสำหรับ QR Code
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # ฝัง QR Code ลงในเอกสาร
                    result = signature.Sign("output.pdf", options)
          ```
        platform: "python-net"
        copy_title: "คัดลอก"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "คลิกเพื่อคัดลอก"
          copy_done: "คัดลอกแล้ว"
        top_links:
          #  loop
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.pdf"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นใช้งานหรือยัง?"
  description: "ลองฟีเจอร์ของ GroupDocs.Signature ฟรี หรือขอรับใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลด PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "การออกใบอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "สำรวจโซลูชันลายเซ็นของเรา"
    exclude: "qrcode"
    description: "เรามีลายเซ็นประเภทต่าง ๆ และการดำเนินการหลากหลายเพื่อตอบสนองความต้องการด้านเอกสารของคุณ."
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/python-net/esign/pdf/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/python-net/text/pdf/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/python-net/image/pdf/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/python-net/barcode/pdf/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pdf/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/python-net/stamp/pdf/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ฝัง QR Code ในรูปแบบเอกสารที่หลากหลาย"
    exclude: "PDF"
    description: "ใช้ API Python via .NET เพื่อฝัง QR Code ลงในรูปแบบเอกสารมาตรฐานอุตสาหกรรมใด ๆ เก็บและเข้ารหัสข้อมูลที่สำคัญลงในบาร์โค้ด 2 มิติสำหรับการสแกนและรับข้อมูลที่สะดวก."
    items: 
          
        # format loop 1
        - name: "QR-Code สำหรับ PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "QR-Code สำหรับ DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Code สำหรับ JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "QR-Code สำหรับ PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Code สำหรับ XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---