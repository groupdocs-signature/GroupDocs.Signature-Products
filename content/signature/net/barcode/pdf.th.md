



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:06
draft: false
lang: th
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "สร้างบาร์โค้ดสำหรับ PDF โดยใช้ C# API"
head_description: "สร้างลายเซ็นบาร์โค้ดและรักษาความปลอดภัยให้กับเอกสาร PDF โดยใช้ C# ด้วยโค้ดเพียงไม่กี่บรรทัด ใช้ GroupDocs.Signature สำหรับการลงนามในไฟล์รูปแบบหลากหลาย."

############################# Header ############################
title: "สร้างบาร์โค้ดสำหรับเอกสาร PDF" 
description: "ใช้ GroupDocs.Signature for .NET วางบาร์โค้ดที่ใดก็ได้ภายในเอกสารธุรกิจของคุณ API ของเราเสนอทางเลือกการปรับแต่งที่กว้างขวางสำหรับลายเซ็นบาร์โค้ด."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรี"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "ภาพรวมของ GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) เป็นโซลูชั่นการลงนามเอกสารที่ซับซ้อนซึ่งรองรับประเภทลายเซ็นที่หลากหลายรวมถึงข้อความ, รูปภาพ, บาร์โค้ด, ใบรับรองดิจิทัล, และตรายาง รองรับไฟล์รูปแบบมากกว่า 60 รูปแบบ—เช่น PDF, MS Office, รูปภาพ, ไฟล์ ZIP, และอื่นๆ—เครื่องมือนี้ช่วยให้คุณสามารถไม่เพียงแต่ใช้ลายเซ็น แต่ยังค้นหา, ตรวจสอบ, ดัดแปลง, หรือถอดออกตามความจำเป็น.

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนการสร้างและฝังบาร์โค้ดในไฟล์ PDF"
    content: |
      [GroupDocs.Signature](/signature/net/) อำนวยความสะดวกในการสร้างบาร์โค้ดในรูปแบบยอดนิยมหลายรูปแบบและวางบาร์โค้ดในหน้า PDF รองรับบาร์โค้ดชนิดมากกว่า 60 ชนิด แอปพลิเคชัน .NET สามารถขยายฟังก์ชันการเซ็นบาร์โค้ดได้อย่างง่ายดายโดยการรวมไลบรารีของเราเข้าด้วยกัน.
      
      1. จัดเตรียมไฟล์ PDF หรือสตรีมสำหรับการประมวลผล.
      2. ส่งข้อความบาร์โค้ดไปยังออบเจ็กต์ BarcodeSignOptions.
      3. ปรับแต่งตัวเลือกบาร์โค้ด เช่น ตำแหน่ง, ขนาด, เป็นต้น.
      4. บันทึกไฟล์พร้อมบาร์โค้ดที่เพิ่มเข้ามา.
   
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
        // สร้างออบเจ็กต์ Signature ใหม่พร้อมกับพาธเอกสาร
        using (Signature signature = new Signature("input.pdf"))
        {
            // ใช้ BarcodeSignOptions เพื่อเพิ่มบาร์โค้ดลงในเอกสาร
            BarcodeSignOptions options = new BarcodeSignOptions("Business data")
            {
                // กำหนดประเภทบาร์โค้ดและคุณสมบัติเสริม
                EncodeType = BarcodeTypes.Code128,
                Left = 50,
                Top = 150
            };

            // บันทึกไฟล์ที่ลงนามแล้ว
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เพิ่มความสามารถและปกป้องเอกสารของคุณด้วยฟีเจอร์ลายเซ็นขั้นสูง"
  description: "ไลบรารี GroupDocs.Signature for .NET ถูกออกแบบมาเพื่ออำนวยความสะดวกในการลงนามเอกสารและการประมวลผลควบคู่ไปกับไฟล์รูปแบบที่ใช้งานกันอย่างแพร่หลาย คุณสามารถเพิ่ม, ปรับแต่ง, ตรวจสอบ, หรือถอดลายเซ็นประเภทต่างๆ ได้อย่างสะดวก."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "ฟีเจอร์เด่นของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "การลงนามเอกสารที่หลากหลาย"
      content: "ลงนามในเอกสารที่รองรับได้อย่างมีประสิทธิภาพโดยใช้ข้อความ, รูปภาพ, บาร์โค้ด, QR โค้ด, หรือตรายาง นอกจากนี้ยังสามารถฝังเมตาดาต้าที่ซ่อนอยู่ เช่น ข้อมูล EXIF ในรูปภาพ หรือป้องกันเนื้อหาของเอกสารของคุณจากการเปลี่ยนแปลงที่ไม่ได้รับอนุญาตโดยใช้ใบรับรองดิจิทัล."

    # feature loop
    - title: "การค้นหาและตรวจสอบลายเซ็นอย่างครอบคลุม"
      content: "เครื่องมือของเราเสนอฟังก์ชันการทำงานที่เข้มแข็งสำหรับการทำงานกับเอกสารที่มีลายเซ็น ตรวจสอบความสมบูรณ์ของเอกสารของคุณโดยการตรวจสอบลายเซ็น และเรียกดูรายการลายเซ็นทั้งหมดภายในเอกสารได้อย่างง่ายดายผ่านฟีเจอร์ค้นหา."

    # feature loop
    - title: "แก้ไขลายเซ็นได้อย่างสะดวก"
      content: "ลายเซ็นที่ถูกนำไปใช้ก่อนหน้านี้เกือบทั้งหมดสามารถปรับแต่งได้ อัปเดตข้อความ, ปรับตำแหน่ง, หรือเปลี่ยนสีให้ตรงตามความต้องการของคุณ."

    # feature loop
    - title: "การลบลายเซ็นอย่างมีประสิทธิภาพ"
      content: "แนวทางของเราให้การสนับสนุนการดำเนินการ CRUD (สร้าง, อ่าน, อัปเดต, ลบ) สำหรับลายเซ็น ทำให้สามารถลบลายเซ็นที่ไม่ต้องการหรือล้าสมัยออกจากเอกสารของคุณได้อย่างรวดเร็ว."
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีสร้างลายเซ็นบาร์โค้ด"
      content: |
        ตัวอย่างนี้แสดงวิธีฝังบาร์โค้ดที่กำหนดเองลงในหน้าเอกสาร PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          using (Signature signature = new Signature("input.pdf"))
          {
              // สร้างตัวเลือกลายเซ็นด้วยข้อความที่ต้องการ
              BarcodeSignOptions options = new BarcodeSignOptions("Accepted")
              {
                  EncodeType = BarcodeTypes.Code39FullASCII,

                  // กำหนดตำแหน่งสัมพัทธ์ของบาร์โค้ดบนหน้า
                  VerticalAlignment = Domain.VerticalAlignment.Top,
                  HorizontalAlignment = Domain.HorizontalAlignment.Left,

                  // กำหนดการตั้งค่าขอบบาร์โค้ดจากขอบหน้า
                  Margin = new Padding() { Top = 180, Right = 20 },

                  // ระบุสีของแถบ
                  ForeColor = Color.Red,

                  // เลือกสไตล์ฟอนต์ข้อความ
                  Font = new SignatureFont { Size = 12, FamilyName = "Arial" },

                  // ระบุตำแหน่งข้อความ
                  CodeTextAlignment = CodeTextAlignment.Above
              };

              // ลงนามและบันทึกเอกสาร
              SignResult result = signature.Sign("output.pdf", options);
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
            link: "/examples/signature/formats/signature_barcode.pdf"
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
    title: "ค้นพบฟีเจอร์หลักของเรา"
    exclude: "barcode"
    description: "เรามีตัวเลือกและการดำเนินการลายเซ็นที่น่าประทับใจ."
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ลงนามในเอกสารในรูปแบบที่หลากหลาย"
    exclude: "PDF"
    description: "API .NET ของเรารองรับการลงนามในรูปแบบที่แตกต่างกันมากกว่า 60 รูปแบบ วางลายเซ็นประเภทต่างๆ ได้อย่างสะดวกในทุกหน้า หรือในตำแหน่งที่คุณต้องการภายในเอกสารของคุณ."
    items: 
          
        # format loop 1
        - name: "เพิ่มบาร์โค้ดใน PDF"
          format: "PDF"
          link: "/signature/net/barcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "เพิ่มบาร์โค้ดใน DOCX"
          format: "DOCX"
          link: "/signature/net/barcode/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "เพิ่มบาร์โค้ดใน JPEG"
          format: "JPEG"
          link: "/signature/net/barcode/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "เพิ่มบาร์โค้ดใน PPTX"
          format: "PPTX"
          link: "/signature/net/barcode/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "เพิ่มบาร์โค้ดใน XLSX"
          format: "XLSX"
          link: "/signature/net/barcode/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---