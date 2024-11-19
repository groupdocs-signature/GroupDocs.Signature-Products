



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:18
draft: false
lang: th
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "เพิ่มลายเซ็นดิจิทัลในไฟล์ DOCX ด้วย JavaScript"
head_description: "เพิ่มลายเซ็นดิจิทัลในไฟล์ DOCX โดยใช้ JavaScript ด้วยโค้ดเพียงไม่กี่บรรทัด ใช้ GroupDocs.Signature for Node.js via Java สำหรับเซ็นชื่อในรูปแบบไฟล์ที่หลากหลาย"

############################# Header ############################
title: "ปกป้อง DOCX ด้วยใบรับรองดิจิทัล" 
description: "มั่นใจในความปลอดภัยของเอกสารธุรกิจของคุณโดยการฝังใบรับรองดิจิทัลด้วยความสามารถที่ก้าวหน้าของ GroupDocs.Signature for Node.js via Java เรามีตัวเลือกที่ยืดหยุ่นในการปกป้องและยืนยันเอกสารของคุณ"
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
    title: "เกี่ยวกับ GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) เป็นโซลูชันการเซ็นชื่อที่ครบวงจรที่ออกแบบมาเพื่อตอบสนองความต้องการในการประมวลผลเอกสารที่หลากหลาย ช่วยให้คุณสามารถรวมข้อความ รูปภาพ ใบรับรองดิจิทัล และแสตมป์ลงในรูปแบบไฟล์กว่า 60 รูปแบบ รวมถึง PDF, MS Office, รูปภาพ และไฟล์ ZIP นอกจากนี้ เอกสารที่ถูกเซ็นสามารถค้นหา ยืนยัน แก้ไข หรือถูกลบได้อย่างง่ายดายเมื่อจำเป็น

############################# Steps ############################
steps:
    enable: true
    title: "แนวทางการป้องกัน DOCX ด้วยใบรับรองดิจิทัลใน JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) ช่วยให้นักพัฒนา Node.js via Java สามารถปกป้องเอกสาร DOCX จากการดัดแปลงโดยใช้ลายเซ็นดิจิทัล ปรับปรุงแอปพลิเคชันธุรกิจของคุณด้วยฟีเจอร์ด้านความปลอดภัยข้อมูลที่ครบถ้วน
      
      1. ส่งเอกสาร DOCX ไปยังตัวสร้างคลาส Signature
      2. ใช้ใบรับรองดิจิทัลและรหัสผ่านที่สอดคล้องกันเพื่อทำให้เอกสารปลอดภัย
      3. เลือกเพิ่มการแสดงภาพของลายเซ็นดิจิทัลในหน้าของเอกสาร
      4. เซ็นเอกสารเพื่อต้านการเปลี่ยนแปลงในอนาคต
   
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

        // ใช้ Signature เพื่อนำลายเซ็นดิจิทัลไปใช้ในเอกสาร
        const signature = new signatureLib.Signature('input.docx');

        // จัดเตรียมใบรับรองดิจิทัลและรหัสผ่านที่จำเป็น
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // กำหนดค่าการตั้งค่าลายเซ็นที่ปรากฏหากจำเป็น
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // เข้ารหัสเอกสารโดยใช้ใบรับรองดิจิทัล
        const result = signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ปรับปรุงหรือปกป้องเนื้อหาเอกสารด้วยลายเซ็น"
  description: "GroupDocs.Signature for Node.js via Java สร้างขึ้นเพื่อเซ็นชื่อในรูปแบบไฟล์หลักทั้งหมด ช่วยให้คุณมีความสามารถในการเพิ่ม ปรับแต่ง ยืนยัน หรือถอนลายเซ็นประเภทต่างๆ ได้อย่างมีประสิทธิภาพ"
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "คุณสมบัติสำคัญของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "เพิ่มลายเซ็นในเอกสารของคุณ"
      content: "วางลายเซ็นข้อความ รูปภาพ บาร์โค้ด QR-Code หรือแสตมป์ในหน้าทุกหน้าของเอกสารที่รองรับ คุณยังสามารถแทรกหรือแก้ไขเมตาดาต้าที่ซ่อนอยู่ เช่น EXIF ในรูปภาพ ปกป้องเนื้อหาเอกสารของคุณจากการเปลี่ยนแปลงที่ไม่ได้รับอนุญาตด้วยใบรับรองดิจิทัล"

    # feature loop
    - title: "ค้นหาและยืนยันลายเซ็น"
      content: "หลังจากการเซ็น เอกสารของคุณสามารถผ่านการตรวจสอบหลายครั้ง ยืนยันความสมบูรณ์ของเนื้อหาที่เซ็นชื่อ หรือดำเนินการค้นหารายละเอียดเพื่อลิสต์ลายเซ็นที่มีอยู่ทั้งหมด"

    # feature loop
    - title: "ปรับปรุงลายเซ็นที่มีอยู่"
      content: "ลายเซ็นส่วนใหญ่สามารถแก้ไขหลังการสร้างได้ คุณสามารถปรับเปลี่ยนข้อความ เปลี่ยนตำแหน่งองค์ประกอบ ปรับสี เปลี่ยนขนาด และทำการเปลี่ยนแปลงอื่นๆ ที่จำเป็นได้อย่างง่ายดาย"

    # feature loop
    - title: "ลบลายเซ็นที่ไม่จำเป็น"
      content: "โซลูชันของเราสามารถดำเนินการ CRUD เต็มรูปแบบสำหรับลายเซ็น หากจำเป็น คุณสามารถลบลายเซ็นประเภทต่างๆ รวมถึงใบรับรองดิจิทัลจากเอกสารของคุณ"
      
  code_samples:
    # code sample loop
    - title: "ปกป้องเอกสารด้วยลายเซ็นดิจิทัล"
      content: |
        เรียนรู้วิธีล็อกเอกสารเพื่อป้องกันการเปลี่ยนแปลงโดยใช้ลายเซ็นดิจิทัล
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // จัดเตรียมเอกสารที่ต้องการเซ็น
        const signature = new signatureLib.Signature('input.docx');

        // ใช้ใบรับรองดิจิทัลและรหัสผ่านที่เหมาะสม
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // รวมข้อมูลข้อความเพิ่มเติมเมื่อจำเป็น
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // เพิ่มองค์ประกอบภาพ เช่น รูปภาพ สำหรับการแสดงผลลายเซ็น
        options.setImageFilePath('image.png');
        options.setAllPages(true);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        const padding = new signatureLib.Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        
        // บันทึกเอกสารที่รักษาความปลอดภัยด้วยดิจิทัลไปยังตำแหน่งที่กำหนด
        const result = signature.sign('output.docx', options);
        ```
        {{< /landing/code >}}


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
    title: "มาทำความรู้จักกับฟังก์ชันหลักของเรา"
    exclude: "digital"
    description: "เราภูมิใจที่จะสนับสนุนชุดทางเลือกและฟังก์ชันของลายเซ็นที่ครบถ้วน"
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "เซ็นเอกสารหลายรูปแบบ"
    exclude: "DOCX"
    description: "API Node.js via Java รองรับรูปแบบกว่า 60 รูปแบบ ทำให้คุณสามารถใช้ลายเซ็นหลายประเภทในหน้าต่างๆ กำหนดมาตรการความปลอดภัยเนื้อหาด้วยใบรับรองดิจิทัล และจัดการลายเซ็นภายในเอกสารได้อย่างมีประสิทธิภาพ"
    items: 
          
        # format loop 1
        - name: "ปกป้อง PDF"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ปกป้อง DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "ปกป้อง PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 4
        - name: "ปกป้อง XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---