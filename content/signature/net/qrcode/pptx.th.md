



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: th
format: Pptx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "สร้าง QR code สำหรับไฟล์ PPTX โดยใช้ C#"
head_description: "ใช้ API GroupDocs.Signature เพื่อสร้าง QR code สำหรับไฟล์ PPTX ลง QR codes ได้อย่างราบรื่นในทุกหน้าเพื่อเพิ่มฟังก์ชันการทำงาน"

############################# Header ############################
title: "สร้าง QR codes สำหรับ PPTX" 
description: "สร้างบาร์โค้ด 2D ได้อย่างมีประสิทธิภาพโดยใช้ข้อมูลข้อความหรือตัวเลข และนำไปใช้ในหลายหน้าและฟอร์แมต รวมถึง PDFs, Word, Excel และอื่น ๆ ผ่าน GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "เริ่มทดลองใช้ฟรีของคุณ"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "สำรวจความสามารถของ GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) มีฟีเจอร์ที่หลากหลาย ทำให้ผู้ใช้สามารถสร้างและฝังประเภทลายเซ็นต่าง ๆ ลงในฟอร์แมตเอกสารชั้นนำ เช่น PDFs, เอกสาร Word, แผ่นงาน Excel, งานนำเสนอ PowerPoint หรือไฟล์ภาพ เพื่อยกระดับเอกสารของคุณด้วยลายเซ็น Text, Image, Barcode, QR Code, Metadata, Digital และ Stamp.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการสร้างและแทรก QR code ในตำแหน่งใดก็ได้ภายใน PPTX"
    content: |
      [GroupDocs.Signature](/signature/net/) อำนวยความสะดวกในการสร้าง QR codes ในรูปแบบยอดนิยมหลายรายการ และตำแหน่งบนหน้าของ PPTX สนับสนุน QR codes มากกว่า 10 ประเภท ห้องสมุดของเราสามารถรวมเข้ากับแอปพลิเคชัน .NET ได้อย่างราบรื่น เสริมเอกสารของคุณด้วยลายเซ็น QR code โดยใช้ผลิตภัณฑ์ของเรา.
      
      1. รับไฟล์ PPTX หรือสตรีมที่ต้องการลงนามด้วย QR code.
      2. ให้เนื้อหาที่จำเป็นกับ QrCodeSignOptions.
      3. ปรับแต่งพารามิเตอร์ด้านภาพ เช่น สี, ตำแหน่ง, ขนาด ฯลฯ.
      4. บันทึกเอกสารที่มี QR code ฝังอยู่.
   
    code:
      platform: "net"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "ตัวอย่างลายเซ็น"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // เริ่มต้นกรณีใหม่ของ Signature ด้วยเอกสาร
        using (Signature signature = new Signature("input.pptx"))
        {
            // ใช้ QrCodeSignOptions เพื่อฝัง QR code ลงในเอกสาร
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // กำหนดประเภทลายเซ็นและระบุตำแหน่งบนหน้า
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // บันทึกเอกสารพร้อม QR code ที่ฝังอยู่
            SignResult result = signature.Sign("output.pptx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "การรวมลายเซ็นที่ครอบคลุมสำหรับเอกสาร"
  description: "ด้วย API GroupDocs.Signature for .NET, ผู้ใช้สามารถสร้าง, แก้ไข, ค้นหา, ตรวจสอบ และลบประเภทลายเซ็นต่าง ๆ ได้อย่างมีประสิทธิภาพ ทำให้การทำงานของเอกสารเป็นไปอย่างแม่นยำ"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "ลงนามเอกสารด้วยลายเซ็นหลายประเภท"
      content: "GroupDocs.Signature อนุญาตให้การใช้ลายเซ็น Text, Image, Barcode, QR Code, และ Stamp ในนามเอกสารใด ๆ ลายเซ็นสามารถวางในตำแหน่งที่แม่นยำบนหน้าใดก็ได้ และสามารถจัดการเมตาดาต้าได้อย่างราบรื่นผ่านลายเซ็นเมตาดาต้า ปกป้องความสมบูรณ์ของเอกสารของคุณโดยการใช้ใบรับรองดิจิตอลที่ป้องกันการเปลี่ยนแปลงที่ไม่ได้รับอนุญาต."

    # feature loop
    - title: "การค้นหาและตรวจสอบลายเซ็น"
      content: "ตรวจสอบความถูกต้องและความแม่นยำของลายเซ็นเอกสารผ่านกระบวนการตรวจสอบขั้นสูง สามารถดึงรายชื่อรายละเอียดของลายเซ็นทั้งหมดที่ฝังอยู่ในเอกสารได้อย่างง่ายดาย."

    # feature loop
    - title: "การแก้ไขลายเซ็นที่ปรับแต่งได้"
      content: "อัปเดตและปรับปรุงลายเซ็นที่ใช้ไปก่อนหน้านี้โดยการปรับแต่งเนื้อหา, ตำแหน่ง, สี, ขนาด และคุณสมบัติอื่น ๆ ตามความต้องการของคุณ."

    # feature loop
    - title: "การลบลายเซ็นที่มีประสิทธิภาพ"
      content: "ทำให้การจัดการเอกสารของคุณมีประสิทธิภาพมากขึ้นโดยการลบลายเซ็นที่ไม่ต้องการผ่านโปรแกรม ไม่ว่าจะเป็นใบรับรองดิจิตอลหรือลายเซ็นประเภทอื่น ๆ การลบสามารถทำได้อย่างรวดเร็วและมีประสิทธิภาพ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีการสร้าง QR code ด้วยตัวเลือกต่าง ๆ?"
      content: |
        ตัวอย่างนี้แสดงให้เห็นถึงวิธีการวาง QR code ที่ปรับแต่งได้ในหน้า PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // ดึงเอกสารที่จะลงนามและส่งไปยัง Signature
          using (Signature signature = new Signature("input.pptx"))
          {
              // ตั้งค่าตัวเลือก QR code ด้วยข้อความที่จำเป็น
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // ระบุตำแหน่งสัมพัทธ์ของ QR code บนหน้า
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // ตั้งค่าระยะห่างของลายเซ็น
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // ระบุสีของ QR code
                    ForeColor = Color.Red,

                    // กำหนดตัวเลือกฟอนต์สำหรับข้อความ
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // ปรับแต่งสีพื้นหลังของ QR code และแปรง
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // ฝัง QR code ลงในเอกสาร
              SignResult result = signature.Sign("output.pptx", options);
          }
          ```
        platform: "net"
        copy_title: "คัดลอก"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "คลิกเพื่อคัดลอก"
          copy_done: "คัดลอกแล้ว"
        top_links:
          #  loop
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.pptx"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นใช้งานหรือยัง?"
  description: "ลองฟีเจอร์ของ GroupDocs.Signature ฟรี หรือขอรับใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลด Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "การออกใบอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "เรียนรู้เกี่ยวกับโซลูชันลายเซ็นของเรา"
    exclude: "qrcode"
    description: "เราภูมิใจนำเสนอประเภทลายเซ็นที่หลากหลายและฟีเจอร์การใช้งาน"
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/net/esign/pptx/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/net/text/pptx/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/net/image/pptx/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/net/barcode/pptx/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/net/qrcode/pptx/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/net/digital/pptx/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/net/stamp/pptx/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/net/search/pptx/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/net/verify/pptx/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/net/modify/pptx/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/net/delete/pptx/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "สร้าง QR codes สำหรับฟอร์แมตเอกสารอื่น ๆ"
    exclude: "PPTX"
    description: "เพิ่มความสามารถในการฝัง QR codes ลงในฟอร์แมตไฟล์มาตรฐานอุตสาหกรรม ผ่าน API .NET. เก็บและเข้ารหัสข้อมูลสำคัญลงในบาร์โค้ด 2D เพื่อการสแกนและการดึงข้อมูลที่ราบรื่น."
    items: 
          
        # format loop 1
        - name: "QR-Code สำหรับ PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "QR-Code สำหรับ DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Code สำหรับ JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "QR-Code สำหรับ PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Code สำหรับ XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---