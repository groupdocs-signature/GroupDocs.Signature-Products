



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:27
draft: false
lang: th
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "ฝังบาร์โค้ดในเอกสาร JPEG ด้วย Python"
head_description: "เพิ่มลายเซ็นบาร์โค้ดอย่างมีประสิทธิภาพในเอกสาร JPEG ด้วยโค้ดไม่กี่บรรทัดใน Python. GroupDocs.Signature มอบโซลูชันการลงนามที่ราบรื่นสำหรับหลายรูปแบบเอกสาร."

############################# Header ############################
title: "สร้างบาร์โค้ดสำหรับ JPEG" 
description: "ด้วย GroupDocs.Signature for Python via .NET คุณสามารถวางบาร์โค้ดในเอกสารทางธุรกิจได้ทุกที่ที่ต้องการ โซลูชันของเรามีตัวเลือกที่ยืดหยุ่นสำหรับการปรับแต่งลายเซ็นบาร์โค้ด."
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
    title: "เกี่ยวกับ GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) เป็นเครื่องมือสำหรับลงนามเอกสารที่ทรงพลังซึ่งรองรับประเภทลายเซ็นที่หลากหลาย รวมถึงข้อความ รูปภาพ บาร์โค้ด ใบรับรองดิจิทัล และตราประทับ รองรับรูปแบบไฟล์มากกว่า 60 รูปแบบ เช่น PDF, MS Office, รูปภาพ, ZIP และอื่นๆ ไม่เพียงแค่ให้คุณสามารถใช้ลายเซ็นได้ แต่ยังช่วยให้คุณค้นหา ตรวจสอบ แก้ไข หรือเอาลายเซ็นออกตามต้องการ.

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนในการสร้างและแทรกบาร์โค้ดใน JPEG"
    content: |
      [GroupDocs.Signature](/signature/python-net/) ช่วยให้คุณสามารถสร้างและฝังบาร์โค้ดในเอกสาร JPEG ได้อย่างรวดเร็ว รองรับบาร์โค้ดมากกว่า 60 รูปแบบ แอปพลิเคชัน Python via .NET สามารถเพิ่มฟังก์ชันการลงนามบาร์โค้ดได้อย่างราบรื่นโดยการรวมไลบรารีของเรา.
      
      1. ให้ไฟล์หรือสตรีม JPEG สำหรับการประมวลผล.
      2. กำหนดข้อความบาร์โค้ดในวัตถุ BarcodeSignOptions.
      3. ปรับแต่งตัวเลือกบาร์โค้ด เช่น ตำแหน่งและขนาด.
      4. บันทึกเอกสารพร้อมบาร์โค้ดที่ฝังอยู่.
   
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

            # เริ่มต้นวัตถุ Signature ด้วยเส้นทางเอกสาร
            with sg.Signature('input.jpeg') as signature:

                # ใช้ BarcodeSignOptions เพื่อเพิ่มบาร์โค้ดลงในเอกสาร
                options = sg.BarcodeSignOptions('Business data')

                # ตั้งค่าประเภทบาร์โค้ดและกำหนดคุณสมบัติของมัน
                options.EncodeType = sg.BarcodeTypes.Code128
                options.Left = 50
                options.Top = 150

                # บันทึกเอกสารที่ลงนามแล้ว
                result = signature.Sign('output.jpeg', options)
        ```          

############################# More features ############################
more_features:
  enable: true
  title: "เสริมความสามารถให้เอกสารของคุณด้วยฟีเจอร์ลายเซ็นขั้นสูง"
  description: "ไลบรารี GroupDocs.Signature for Python via .NET ให้โซลูชันที่ครอบคลุมสำหรับการลงนามและประมวลผลเอกสารในรูปแบบที่ใช้งานทั่วไป คุณสามารถเพิ่ม แก้ไข ตรวจสอบ หรือเอาลายเซ็นประเภทต่างๆ ออกได้ตามความต้องการ."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "การลงนามเอกสารที่ยืดหยุ่น"
      content: "ลงนามในหน้าใดก็ได้ในเอกสารที่รองรับด้วยข้อความ รูปภาพ บาร์โค้ด โค้ด QR หรือตราประทับ เพิ่มข้อมูลเมตาแบบซ่อน เช่น ข้อมูล EXIF ในรูปภาพ และรับประกันการป้องกันเนื้อหาด้วยใบรับรองดิจิทัลเพื่อป้องกันการเปลี่ยนแปลงที่ไม่ได้รับอนุญาต."

    # feature loop
    - title: "ค้นหาและตรวจสอบลายเซ็น"
      content: "เครื่องมือของเราช่วยให้มั่นใจในความถูกต้องของเอกสารของคุณโดยการเปิดใช้งานการตรวจสอบลายเซ็น นอกจากนี้คุณยังสามารถดึงรายการลายเซ็นทั้งหมดในเอกสารได้เพื่อการจัดการที่สะดวก."

    # feature loop
    - title: "แก้ไขลายเซ็นได้อย่างง่ายดาย"
      content: "ปรับแก้ลายเซ็นที่มีอยู่ได้อย่างไม่ยุ่งยาก ปรับข้อความ เปลี่ยนตำแหน่งขององค์ประกอบ หรือเปลี่ยนสีให้เหมาะสมกับความต้องการของเอกสารของคุณ."

    # feature loop
    - title: "ลบลายเซ็นได้อย่างง่ายดาย"
      content: "ด้วยฟังก์ชัน CRUD แบบเต็มรูปแบบ GroupDocs.Signature for Python via .NET ทำให้การลบลายเซ็นที่ไม่ต้องการหรือเก่าออกจากเอกสารของคุณเป็นเรื่องง่าย."
      
  code_samples_ext:
    # code sample ext loop
    - title: "สร้างและวางลายเซ็นบาร์โค้ด"
      content: |
        ตัวอย่างนี้แสดงวิธีการแทรกบาร์โค้ดกำหนดเองลงในเอกสาร JPEG.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # ให้เอกสารที่จะถูกลงนาม
              with sg.Signature('input.jpeg') as signature:

                  # ตั้งค่าข้อความบาร์โค้ดและตัวเลือกการลงนาม
                  options = sg.BarcodeSignOptions('Accepted')
                  options.EncodeType = sg.BarcodeTypes.Code39FullASCII

                  # เลือกตำแหน่งสำหรับบาร์โค้ดบนหน้า
                  options.VerticalAlignment = sg.VerticalAlignment.Top
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left

                  # ตั้งค่าระยะห่างระหว่างบาร์โค้ดและขอบหน้า
                  options.Margin = sg.Padding()
                  options.Margin.Top = 180
                  options.Margin.Right = 20

                  # ระบุสีของแท่งบาร์โค้ด
                  options.ForeColor = sg.Color.Red

                  # เลือกสไตล์ฟอนต์สำหรับข้อความบาร์โค้ด
                  options.Font = sg.SignatureFont()
                  options.Font.Size = 12
                  options.Font.FamilyName = 'Arial'

                  # ตั้งค่าตำแหน่งของข้อความ
                  options.CodeTextAlignment = sg.CodeTextAlignment.Above

                  # ลงนามและบันทึกเอกสาร
                  result = signature.Sign('output.jpeg', options)
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
            link: "/examples/signature/formats/signature_barcode.jpeg"
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
    title: "สำรวจฟีเจอร์หลักของเรา"
    exclude: "barcode"
    description: "เรามีตัวเลือกและการดำเนินการที่หลากหลายสำหรับความต้องการเอกสารของคุณ."
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/python-net/esign/jpeg/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/python-net/text/jpeg/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/python-net/image/jpeg/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/python-net/barcode/jpeg/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/python-net/stamp/jpeg/"
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
    title: "ลงนามเอกสารในหลายรูปแบบ"
    exclude: "JPEG"
    description: "API Python via .NET รองรับการลงนามในรูปแบบไฟล์มากกว่า 60 รูปแบบ ทำให้คุณสามารถเพิ่มลายเซ็นประเภทต่างๆ ลงในหน้าใดก็ได้หรือตำแหน่งเฉพาะในเอกสารของคุณ."
    items: 
          
        # format loop 1
        - name: "เพิ่มบาร์โค้ดใน PDF"
          format: "PDF"
          link: "/signature/python-net/barcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "เพิ่มบาร์โค้ดใน DOCX"
          format: "DOCX"
          link: "/signature/python-net/barcode/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "เพิ่มบาร์โค้ดใน JPEG"
          format: "JPEG"
          link: "/signature/python-net/barcode/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "เพิ่มบาร์โค้ดใน PPTX"
          format: "PPTX"
          link: "/signature/python-net/barcode/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "เพิ่มบาร์โค้ดใน XLSX"
          format: "XLSX"
          link: "/signature/python-net/barcode/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---