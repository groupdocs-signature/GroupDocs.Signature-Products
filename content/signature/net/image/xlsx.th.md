



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:51
draft: false
lang: th
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "การเพิ่มลายเซ็นภาพลงในไฟล์ XLSX ด้วย C#"
head_description: "ใส่ลายเซ็นภาพในไฟล์ XLSX สำหรับ .NET โดยการเขียนโค้ดเพียงไม่กี่บรรทัด ใช้ API GroupDocs.Signature for .NET เพื่อเพิ่มภาพ."

############################# Header ############################
title: "เพิ่มลายเซ็นภาพในไฟล์ XLSX" 
description: "ใช้ GroupDocs.Signature for .NET เพื่อรวมภาพเข้าไปในรูปแบบเอกสารสำนักงานที่หลากหลาย รวมถึง PDFs, Word, Excel และไฟล์ภาพ การใส่ภาพลายเซ็นของผู้บริหารสามารถสร้างความประทับใจทางวิชาชีพที่ชัดเจน ยกระดับความดึงดูดสายตาและความถูกต้องของเอกสารของคุณ."
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
    title: "ค้นพบ GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) มีความสามารถครอบคลุมในการฝังลายเซ็นภาพในตำแหน่งใด ๆ บนหน้าใด ๆ ในเอกสารทางธุรกิจของคุณ ปรับปรุงกระบวนการทำงานของคุณโดยการรวมภาพเข้าไปใน PDFs, เอกสาร Word, สเปรดชีต Excel, การนำเสนอ PowerPoint และรูปแบบภาพยอดนิยมต่าง ๆ ผ่านห้องสมุดที่แข็งแกร่งของเรา.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการเพิ่มภาพในที่ใดก็ได้ของไฟล์ XLSX ด้วย C#"
    content: |
      ใช้ประโยชน์จาก [GroupDocs.Signature](/signature/net/) เพื่อเสริมสร้างแอปพลิเคชัน .NET ให้มีความสามารถในการฝังลายเซ็นอย่างถูกต้องในหน้าใดก็ได้ของเอกสาร XLSX เพื่อเพิ่มขีดความสามารถของผลิตภัณฑ์ของคุณอย่างราบรื่น.
      
      1. สร้างออบเจกต์ของคลาส Signature ด้วยเอกสาร XLSX.
      2. ใช้ ImageSignOptions เพื่อระบุภาพลายเซ็น.
      3. ตำแหน่งภาพอย่างแม่นยำในตำแหน่งที่ต้องการบนหน้าใดหน้า .
      4. บันทึกเอกสารที่ลงนามใหม่ไปยังตำแหน่งที่กำหนด.
   
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
        // เริ่มต้น Signature โดยใช้พาธไปยังเอกสาร
        using (Signature signature = new Signature("input.xlsx"))
        {
            // กำหนดค่า ImageSignOptions โดยใช้ภาพสำหรับลายเซ็น
            ImageSignOptions options = new ImageSignOptions("company_logo.jpg")
            {
                // ตำแหน่งภาพที่มุมซ้ายบนของทุกหน้า
                AllPages = true,
                Left = 100,
                Top = 200
            };

            // บันทึกเอกสารที่ลงนาม
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "โซลูชันการลงนามเอกสารที่ครบถ้วน"
  description: "เรามีความยินดีที่จะนำเสนอฟังก์ชันการลงนามที่หลากหลายซึ่งสนับสนุนโดย API ของเรา เพิ่ม, แก้ไข, ลบ, ค้นหา และตรวจสอบประเภทลายเซ็นที่แตกต่างกัน รวมถึงลายเซ็นที่ใช้ภาพ."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "การลงนามด้วยภาพ"
  features:
    # feature loop
    - title: "ผสานรวมภาพในเอกสารสำนักงาน"
      content: "แทรกลายเซ็นอิเล็กทรอนิกส์และภาพอย่างราบรื่นในตำแหน่งที่กำหนดในหน้าใด ๆ ของเอกสาร ปรับปรุงเนื้อหาเอกสารของคุณด้วยข้อความ, ภาพ, บาร์โค้ด, ข้อมูลเมตา, หรือใบรับรองดิจิทัลเพื่อเพิ่มฟังก์ชันและความปลอดภัย."

    # feature loop
    - title: "ค้นหาและตรวจสอบลายเซ็น"
      content: "จัดการเอกสารที่ลงนามโดยตรวจสอบความถูกต้องและความสมบูรณ์ของลายเซ็น รับรายการลายเซ็นทั้งหมดในเอกสารและตรวจสอบคุณสมบัติที่เฉพาะเจาะจง."

    # feature loop
    - title: "แก้ไขลายเซ็น"
      content: "บางครั้งลายเซ็นในเอกสารอาจต้องการการปรับปรุง สามารถปรับแต่งเนื้อหา, ลักษณะ, ขนาด หรือตำแหน่งของลายเซ็นที่มีอยู่ให้ตรงตามความต้องการที่เปลี่ยนแปลง."

    # feature loop
    - title: "ลบลายเซ็นที่ไม่จำเป็น"
      content: "API ของเราช่วยให้ทำการดำเนินการ CRUD ได้เต็มรูปแบบสำหรับประเภทลายเซ็นส่วนใหญ่ คุณสามารถลบลายเซ็นจากรูปแบบเอกสารที่สนับสนุนเกือบทั้งหมดได้อย่างมีประสิทธิภาพเมื่อจำเป็น."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ปกป้องเนื้อหาของเอกสารด้วยภาพลายเซ็น"
      content: |
        ค้นพบวิธีการปรับปรุงเอกสารทางธุรกิจโดยการฝังภาพ ซึ่งให้ข้อมูลเพิ่มเติม.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // เลือกเอกสารที่จะเซ็น
          using (Signature signature = new Signature("input.xlsx"))
          {
              // สร้างตัวเลือกภาพโดยใช้พาธของภาพที่ระบุ
              ImageSignOptions options = new ImageSignOptions("manager_signature.jpg")
              {
                    // กำหนดขนาดของลายเซ็นภาพ
                    Width = 100,
                    Height = 100,

                    // ตำแหน่งภาพที่มุมล่างขวา
                    VerticalAlignment = VerticalAlignment.Bottom,
                    HorizontalAlignment = HorizontalAlignment.Right,

                    // เพิ่มการเว้นระยะที่จำเป็นจากขอบของหน้า
                    Margin = new Padding() { Bottom = 120, Right = 120 },

                    // เลือกเพิ่มกรอบที่กำหนดเองให้กับภาพตามต้องการ
                    Border = new Border()
                    {
                        Visible = true,
                        Color = Color.Red,
                        DashStyle = DashStyle.DashDotDot,
                        Weight = 5
                    },

                    // หมุนลายเซ็นเพื่อการจัดแนวที่เหมาะสม
                    RotationAngle = 45
              };

              // บันทึกเอกสารที่อัปเดตไปยังตำแหน่งที่ต้องการ
              SignResult result = signature.Sign("output.xlsx", options);
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
            link: "/examples/signature/formats/signature_image.xlsx"
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
    title: "เข้าใจข้อเสนอในการใช้งานฟีเจอร์ของเรา"
    exclude: "image"
    description: "สำรวจชุดลายเซ็นที่หลากหลายและการดำเนินการที่แข็งแกร่งที่ให้บริการโดยแพลตฟอร์มของเรา"
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ผสานรวมภาพในรูปแบบไฟล์ที่หลากหลาย"
    exclude: "XLSX"
    description: "ใช้ API .NET เพื่อเพิ่มรูปแบบภาพที่สนับสนุนลงในเอกสารที่หลากหลาย ปรับขนาด, ตำแหน่ง, เลือกหน้าเฉพาะ และใช้ลายเซ็นที่ใช้ภาพในเอกสารของคุณ."
    items: 
          
        # format loop 1
        - name: "ลงชื่อ PDF ด้วยภาพ"
          format: "PDF"
          link: "/signature/net/image/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ลงชื่อ DOCX ด้วยภาพ"
          format: "DOCX"
          link: "/signature/net/image/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "ลงชื่อ JPEG ด้วยภาพ"
          format: "JPEG"
          link: "/signature/net/image/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "ลงชื่อ PPTX ด้วยภาพ"
          format: "PPTX"
          link: "/signature/net/image/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "ลงชื่อ XLSX ด้วยภาพ"
          format: "XLSX"
          link: "/signature/net/image/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---