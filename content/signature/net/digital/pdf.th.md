



---
############################# Static ############################
layout: "format"
date:  2024-11-20T08:57:23
draft: false
lang: th
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "การเพิ่มลายเซ็นดิจิทัลลงในไฟล์ PDF ด้วย C#"
head_description: "เพิ่มลายเซ็นดิจิทัลลงในไฟล์ PDF โดยใช้ C# ด้วยโค้ดเพียงไม่กี่บรรทัด ใช้ GroupDocs.Signature for .NET เพื่อเซ็นชื่อในรูปแบบไฟล์หลายรูปแบบ"

############################# Header ############################
title: "eSign PDF ด้วยลายเซ็นดิจิทัล" 
description: "ปกป้องความสมบูรณ์ของเอกสารทางธุรกิจของคุณโดยการปิดผนึกด้วยใบรับรองดิจิทัลโดยใช้คุณสมบัติที่แข็งแกร่งของ GroupDocs.Signature for .NET เรามีโซลูชันที่หลากหลายเพื่อทำเครื่องหมายและรักษาความปลอดภัยของเอกสารของคุณ"
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
    title: "เกี่ยวกับ GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) เป็นโซลูชันการเซ็นชื่อที่ซับซ้อนซึ่งช่วยให้จัดการงานการประมวลผลเอกสารได้หลากหลาย มันช่วยให้คุณสามารถฝังข้อความ, รูปภาพ, ใบรับรองดิจิทัล และตราประทับลงในไฟล์กว่า 60 แฟ้มฟอร์แมต รวมถึง PDF, MS Office, รูปภาพ, ไฟล์ ZIP และรูปแบบธุรกิจที่สำคัญอื่น ๆ นอกจากนี้ เอกสารที่ลงนามสามารถค้นหา, ยืนยัน, แก้ไข หรือถูกลบได้ตามความจำเป็น

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการรักษาความปลอดภัยให้กับ PDF ด้วยใบรับรองดิจิทัลใน C#"
    content: |
      [GroupDocs.Signature](/signature/net/) ช่วยให้นักพัฒนา .NET สามารถรักษาความปลอดภัยเอกสาร PDF จากการเปลี่ยนแปลงโดยใช้ลายเซ็นดิจิทัล เสริมสร้างแอปพลิเคชันทางธุรกิจของคุณด้วยความสามารถในการป้องกันข้อมูลที่มีความแข็งแกร่ง
      
      1. ส่งเอกสาร PDF ไปยังตัวสร้างของคลาส Signature
      2. ใช้ใบรับรองดิจิทัลและรหัสผ่านของมันเพื่อรักษาความปลอดภัยให้กับเอกสาร
      3. เพิ่มการนำเสนอภาพลักษณ์ของลายเซ็นดิจิทัลลงในหน้าของเอกสารถ้าจำเป็น
      4. เซ็นเอกสารเพื่อให้แน่ใจว่าเอกสารถูกเก็บไว้ไม่เปลี่ยนแปลง
   
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
        // ใช้ Signature ในการเซ็นชื่อเอกสารดิจิทัล
        using (Signature signature = new Signature("input.pdf"))
        {
            // จัดเตรียมใบรับรองดิจิทัลและรหัสผ่านที่เกี่ยวข้อง
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // กำหนดการนำเสนอภาพลักษณ์ตามต้องการ
                PageNumber = 1,
                Left = 50,
                Top = 50
            };

            // รักษาความปลอดภัยของเอกสารด้วยใบรับรองดิจิทัล
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เพิ่มหรือปกป้องเนื้อหาเอกสารด้วยลายเซ็น"
  description: "ไลบรารี GroupDocs.Signature for .NET ได้รับการออกแบบมาเพื่อเซ็นชื่อในรูปแบบไฟล์ที่แพร่หลายทั้งหมด ทำให้กระบวนการทางธุรกิจของคุณเร็วขึ้นโดยการเพิ่ม แก้ไข ยืนยัน หรือเอาลายเซ็นหลากหลายประเภทออกได้อย่างง่ายดาย"
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "คุณสมบัติหลักของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "ฝังลายเซ็นลงในเอกสาร"
      content: "ฝังลายเซ็นประเภทข้อความ, รูปภาพ, บาร์โค้ด, QR-Code หรือ ตราประทับด้วยความแม่นยำบนหน้าทุกหน้าของเอกสารที่รองรับ คุณยังสามารถเพิ่มหรือแก้ไขข้อมูลเมตาภาพที่ซ่อนอยู่ เช่น EXIF ในรูปภาพและประเภทไฟล์ส่วนใหญ่ เพื่อให้มั่นใจในความสมบูรณ์ของเนื้อหาเอกสารของคุณด้วยลายเซ็นดิจิทัล"

    # feature loop
    - title: "ค้นหาและยืนยันลายเซ็น"
      content: "การประมวลผลหลังการเซ็นชื่อเปิดโอกาสมากมาย ยืนยันว่าเอกสารที่ลงนามของคุณได้รับการประมวลผลอย่างถูกต้อง เพื่อความควบคุมที่มากขึ้น รับรายการลายเซ็นทั้งหมดอย่างครอบคลุมผ่านฟังก์ชันค้นหา"

    # feature loop
    - title: "แก้ไขลายเซ็น"
      content: "ลายเซ็นประเภทส่วนใหญ่สามารถแก้ไขได้เต็มที่ คุณสามารถปรับแก้ข้อความ, ย้ายอิลิเมนต์, เปลี่ยนสี, เปลี่ยนขนาด และอีกมากมาย"

    # feature loop
    - title: "ลบลายเซ็นที่ไม่จำเป็น"
      content: "โซลูชันของเรามีการดำเนินการ CRUD เต็มรูปแบบสำหรับลายเซ็น หากจำเป็น คุณสามารถลบประเภทลายเซ็นที่หลากหลาย รวมถึงใบรับรองดิจิทัล ออกจากเอกสารของคุณ"
      
  code_samples_ext:
    # code sample ext loop
    - title: "รักษาความปลอดภัยเอกสารด้วยลายเซ็นดิจิทัล"
      content: |
        ค้นพบวิธีป้องกันการเปลี่ยนแปลงเอกสารโดยใช้ลายเซ็นดิจิทัล
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // จัดเตรียมเอกสารที่จะเซ็นชื่อ
          using (Signature signature = new Signature("input.pdf"))
          {
              // ใช้ใบรับรองดิจิทัลที่ใช้งานได้กับรหัสผ่านที่เกี่ยวข้อง
              DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
              {
                    Password = "1234567890",

                    // ระบุข้อมูลข้อความเพิ่มเติม
                    Reason = "Security issue",
                    Contact = "John Smith",
                    Location = "Office D.W.",

                    // ฝังภาพและตัวเลือกอื่น ๆ สำหรับการนำเสนอภาพลักษณ์
                    ImageFilePath = "image.png",
                    AllPages = true,
                    VerticalAlignment = VerticalAlignment.Center,
                    HorizontalAlignment = HorizontalAlignment.Left,
                    Width = 60,
                    Height = 80,

                    Margin = new Padding() {  Bottom = 10, Right = 10 }
              };

              // บันทึกเอกสารที่ปลอดภัยไปยังตำแหน่งที่กำหนด
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
            link: "/examples/signature/formats/signature_digital.pdf"
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
    title: "ดูคุณสมบัติที่โดดเด่นของเรา"
    exclude: "digital"
    description: "เรานำเสนอคุณสมบัติของลายเซ็นที่หลากหลายและการดำเนินการที่ทรงพลัง"
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
    title: "เซ็นเอกสารในรูปแบบต่างๆ"
    exclude: "PDF"
    description: "API .NET ช่วยให้คุณสามารถประมวลผลรูปแบบต่างๆ กว่า 60 รูปแบบ คุณสามารถสร้างและฝังลายเซ็นที่หลากหลายอย่างราบรื่นในทุกหน้า ใช้ใบรับรองดิจิทัลเพื่อรักษาความปลอดภัยของเนื้อหา และจัดการลายเซ็นที่มีอยู่ในเอกสารได้อย่างมีประสิทธิภาพ"
    items: 
          
        # format loop 1
        - name: "ปกป้อง PDF"
          format: "PDF"
          link: "/signature/net/digital/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ปกป้อง DOCX"
          format: "DOCX"
          link: "/signature/net/digital/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "ปกป้อง PPTX"
          format: "PPTX"
          link: "/signature/net/digital/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 4
        - name: "ปกป้อง XLSX"
          format: "XLSX"
          link: "/signature/net/digital/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---