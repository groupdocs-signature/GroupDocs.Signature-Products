



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:52
draft: false
lang: th
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "เพิ่มลายเซ็นรูปภาพลงในไฟล์ JPEG ด้วย JavaScript"
head_description: "ใส่ลายเซ็นรูปภาพในไฟล์ JPEG สำหรับ Node.js โดยใช้โค้ดเพียงไม่กี่บรรทัด ใช้ API GroupDocs.Signature for Node.js via Java เพื่อเพิ่มรูปภาพ."

############################# Header ############################
title: "ลงนามไฟล์ JPEG โดยใช้ลายเซ็นรูปภาพ" 
description: "ใช้ประโยชน์จากความสามารถของ GroupDocs.Signature for Node.js via Java ในการฝังรูปภาพลงในรูปแบบเอกสารสำนักงานหลายรูปแบบ เช่น PDF, Word, Excel และไฟล์รูปภาพอื่น ๆ การเพิ่มภาพลายเซ็นบริหารสามารถเพิ่มความเป็นมืออาชีพและความน่าเชื่อถือให้กับเอกสารของคุณ สร้างการนำเสนอที่ดูเรียบร้อยและน่าเชื่อถือ."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรี"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "แนะนำ GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) ช่วยให้ผู้ใช้สามารถรวมลายเซ็นรูปภาพในตำแหน่งใด ๆ ของเอกสารของคุณ เครื่องมือนี้ทำให้ธุรกิจสามารถปรับปรุงกระบวนการทำงานโดยการเพิ่มรูปภาพลงใน PDF, Word, Excel, PowerPoint และรูปแบบภาพยอดนิยม ช่วยเพิ่มประสิทธิภาพการจัดการเอกสาร.

############################# Steps ############################
steps:
    enable: true
    title: "คู่มือการเพิ่มรูปภาพใน JPEG โดยใช้ JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) ช่วยให้แอปพลิเคชัน Node.js via Java สามารถรวมลายเซ็นรูปภาพเข้าไปในเอกสาร JPEG ได้อย่างราบรื่น ปรับปรุงความสามารถของแอปพลิเคชันของคุณด้วยไลบรารีที่ครอบคลุมของเรา.
      
      1. สร้าง Signature ด้วยเอกสาร JPEG
      2. ใช้ ImageSignOptions เพื่อระบุภาพลายเซ็น
      3. วางรูปภาพในตำแหน่งที่ต้องการในหน้าใดก็ได้
      4. บันทึกเอกสารที่ลงนามไปยังตำแหน่งที่ต้องการ
   
    code:
      platform: "nodejs-java"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "ตัวอย่างลายเซ็น"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // เริ่มต้น Signature ด้วยเส้นทางไปยังเอกสาร
        const signature = new signatureLib.Signature('input.jpeg');

        // ตั้งค่า ImageSignOptions เพื่อรวมลายเซ็นรูปภาพที่ต้องการ
        const options = new signatureLib.ImageSignOptions('company_logo.jpg');

        // วางรูปภาพในมุมซ้ายบนของทุกหน้า
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);
        
        // บันทึกเอกสารพร้อมลายเซ็นรูปภาพที่ใช้
        const result = signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ความสามารถในการลงนามเอกสารขั้นสูง"
  description: "API ของเรามีชุดฟังก์ชันที่ช่วยให้การลงนามอิเล็กทรอนิกส์เป็นเรื่องง่าย คุณสามารถเพิ่ม แก้ไข ลบ ค้นหา และตรวจสอบลายเซ็นหลายประเภท รวมถึงลายเซ็นรูปภาพได้."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "ลายเซ็นรูปภาพ"
  features:
    # feature loop
    - title: "รวมภาพลงในเอกสารสำนักงาน"
      content: "สามารถวางลายเซ็นรูปภาพได้ทุกที่ในเอกสารของคุณ ไม่ว่าจะเป็นไฟล์ PDF, Word หรือ Excel ปรับปรุงเอกสารของคุณโดยการเพิ่มรูปภาพ รหัสบาร์ ข้อมูลเมตา หรือใบรับรองดิจิทัลเพื่อเพิ่มฟังก์ชันการใช้งาน."

    # feature loop
    - title: "ค้นหาและตรวจสอบลายเซ็น"
      content: "ยืนยันความถูกต้องของเอกสารที่ลงนามโดยการตรวจสอบลายเซ็น ใช้ฟังก์ชันค้นหาเพื่อนำมาทบทวนลายเซ็นทั้งหมดที่ฝังอยู่ในเอกสารของคุณ."

    # feature loop
    - title: "แก้ไขลายเซ็นที่มีอยู่"
      content: "API ของเราช่วยให้ผู้ใช้สามารถอัปเดตและปรับแต่งลายเซ็นตามต้องการ ปรับขนาด ตำแหน่ง หรือคุณลักษณะอื่น ๆ ของลายเซ็นที่เพิ่มไว้ก่อนหน้านี้ เพื่อความยืดหยุ่นในการจัดการเอกสาร."

    # feature loop
    - title: "ลบลายเซ็นที่ไม่จำเป็น"
      content: "จัดการเอกสารของคุณอย่างมีประสิทธิภาพโดยการลบลายเซ็นที่ไม่ต้องการอีกต่อไป API ของเราสนับสนุนการดำเนินการ CRUD แบบเต็มสำหรับเกือบทุกประเภทของลายเซ็น."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ปรับปรุงเอกสารด้วยลายเซ็นรูปภาพ"
      content: |
        เรียนรู้วิธีรวมรูปภาพลงในเอกสารธุรกิจเพื่อเพิ่มข้อมูลเพิ่มเติม.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // เลือกเอกสารที่จะลงนาม
          const signature = new signatureLib.Signature('input.jpeg');

          // ตั้งค่าตัวเลือกภาพด้วยเส้นทางของภาพ
          const options = new signatureLib.ImageSignOptions('manager_signature.jpg');

          // ปรับขนาดของลายเซ็นรูปภาพ
          options.setWidth(100);
          options.setHeight(100);

          // วางรูปภาพในมุมล่างขวา
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // เพิ่มระยะห่างจากมุมของหน้าได้หากจำเป็น
          const padding = new signatureLib.Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // เพิ่มกรอบแบบกำหนดเองให้กับรูปภาพได้ตามต้องการ
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // หมุนลายเซ็นรูปภาพเพื่อความสวยงามที่ดีที่สุด
          options.setRotationAngle(45);

          // บันทึกเอกสารที่อัปเดตไปยังตำแหน่งที่ต้องการ
          const result = signature.sign('output.jpeg', options);
          ```
        platform: "nodejs-java"
        copy_title: "คัดลอก"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "คลิกเพื่อคัดลอก"
          copy_done: "คัดลอกแล้ว"
        top_links:
          #  loop
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/signature/formats/signature_image.jpeg"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นใช้งานหรือยัง?"
  description: "ลองฟีเจอร์ของ GroupDocs.Signature ฟรี หรือขอรับใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลด NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "การออกใบอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "ค้นพบฟังก์ชันที่เรามีเสนอ"
    exclude: "image"
    description: "เราภูมิใจที่จะแสดงความหลากหลายของวิธีการและการดำเนินการลายเซ็น."
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "เพิ่มรูปภาพในไฟล์ประเภทต่าง ๆ"
    exclude: "JPEG"
    description: "API Node.js via Java ช่วยให้คุณสามารถฝังรูปภาพลงในรูปแบบเอกสารที่หลากหลาย ปรับแต่งขนาด การวางตำแหน่ง และการจัดวางหน้าเพื่อปรับปรุงกระบวนการลงนามในเอกสารของคุณ."
    items: 
          
        # format loop 1
        - name: "ลงชื่อ PDF ด้วยภาพ"
          format: "PDF"
          link: "/signature/nodejs-java/image/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ลงชื่อ DOCX ด้วยภาพ"
          format: "DOCX"
          link: "/signature/nodejs-java/image/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "ลงชื่อ JPEG ด้วยภาพ"
          format: "JPEG"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "ลงชื่อ PPTX ด้วยภาพ"
          format: "PPTX"
          link: "/signature/nodejs-java/image/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "ลงชื่อ XLSX ด้วยภาพ"
          format: "XLSX"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---