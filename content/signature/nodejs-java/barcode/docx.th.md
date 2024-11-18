



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:07
draft: false
lang: th
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "สร้างบาร์โค้ดสำหรับ DOCX โดยใช้แอปพลิเคชัน JavaScript"
head_description: "สร้างและฝังลายเซ็นบาร์โค้ดในเอกสาร DOCX ด้วย JavaScript โดยใช้เพียงไม่กี่บรรทัดของโค้ด GroupDocs.Signature สนับสนุนการลงนามในหลายรูปแบบไฟล์."

############################# Header ############################
title: "สร้างและเพิ่มบาร์โค้ดใน DOCX ได้อย่างรวดเร็ว" 
description: "ใช้ GroupDocs.Signature for Node.js via Java เพื่อนำบาร์โค้ดไปใช้ในเอกสารธุรกิจของคุณ โดยวางไว้ในจุดที่ต้องการ โซลูชันของเรามีตัวเลือกการปรับแต่งที่หลากหลายให้คุณสามารถปรับแต่งลายเซ็นบาร์โค้ดตามความต้องการได้."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดทันที – ฟรี!"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "การแนะนำ GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) เป็นเครื่องมือในการลงนามเอกสารที่ทรงพลัง รองรับรูปแบบลายเซ็นที่หลากหลายรวมถึงข้อความ รูปภาพ บาร์โค้ด ใบรับรองดิจิทัล และตราประทับ ด้วยความเข้ากันได้กับรูปแบบไฟล์มากกว่า 60 รูปแบบ เช่น PDFs, ไฟล์ MS Office, รูปภาพ และ ZIP archives ทำให้สามารถจัดการเอกสารได้อย่างครบถ้วน เส้นทางการลงนามในเอกสารสามารถค้นหา ตรวจสอบ แก้ไข หรือทำการลบได้ตามความต้องการ.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการสร้างและฝังบาร์โค้ดในไฟล์ DOCX"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) ช่วยในการสร้างและวางบาร์โค้ดในรูปแบบยอดนิยมหลากหลายอย่างในหน้า DOCX โดยมีการสนับสนุนมากกว่า 60 ประเภทของบาร์โค้ด แอปพลิเคชัน Node.js via Java สามารถปรับปรุงด้วยฟีเจอร์การลงนามบาร์โค้ดได้อย่างง่ายดายโดยการรวมไลบรารีของเราเข้าด้วยกัน.
      
      1. จัดเตรียมไฟล์ DOCX หรือสตรีมสำหรับการประมวลผล.
      2. ส่งข้อความบาร์โค้ดไปยังอ็อบเจ็กต์ BarcodeSignOptions.
      3. ปรับแต่งการตั้งค่าบาร์โค้ด เช่น ตำแหน่ง ขนาด ฯลฯ.
      4. บันทึกเอกสารพร้อมกับบาร์โค้ดที่เพิ่มเข้าไปใหม่.
   
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

        // สร้างอ็อบเจ็กต์ Signature พร้อมกับพาธเอกสาร
        const signature = new signatureLib.Signature('input.docx');

        // ใช้ BarcodeSignOptions เพื่อรวมบาร์โค้ดลงในเอกสาร
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // กำหนดประเภทบาร์โค้ดและพารามิเตอร์เพิ่มเติม
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // บันทึกเอกสารที่มีลายเซ็น
        signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เสริมสร้างและรักษาความปลอดภัยให้เอกสารของคุณด้วยตัวเลือกลายเซ็นขั้นสูง"
  description: "ไลบรารี GroupDocs.Signature for Node.js via Java ถูกออกแบบมาเพื่อทำให้กระบวนการลงนามและการจัดการกับรูปแบบเอกสารยอดนิยมทำได้ง่ายและรวดเร็ว เพิ่ม แก้ไข ตรวจสอบ หรือทำการลบลายเซ็นที่หลากหลายได้อย่างรวดเร็ว."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "ฟังก์ชันหลักของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "การลงนามเอกสารแบบไดนามิก"
      content: "ลงนามในเอกสารของคุณในหน้าใดก็ได้โดยใช้ลายเซ็นที่หลากหลายรวมถึงข้อความ รูปภาพ บาร์โค้ด QR โค้ด และตราประทับ นอกจากนี้ คุณสามารถฝังข้อมูลเมตาดาต้าแบบซ่อน เช่น ข้อมูล EXIF ในรูปภาพ หรือรักษาความปลอดภัยให้เอกสารด้วยการใช้ใบรับรองดิจิทัลเพื่อป้องกันการแก้ไขที่ไม่ได้รับอนุญาต."

    # feature loop
    - title: "การตรวจสอบและค้นหาลายเซ็นที่เชื่อถือได้"
      content: "โซลูชันของเราเสนอเครื่องมือที่หลากหลายในการจัดการเอกสารที่ได้รับการลงนาม ตรวจสอบความถูกต้องของลายเซ็นเพื่อให้มั่นใจในความสมบูรณ์ของเอกสาร และใช้ฟีเจอร์ค้นหาเพื่อลิสต์ลายเซ็นทั้งหมดที่ฝังอยู่ภายในเอกสาร."

    # feature loop
    - title: "แก้ไขลายเซ็นได้อย่างง่ายดาย"
      content: "ลายเซ็นที่ถูกเพิ่มเข้ามาก่อนได้รับการปรับแก้ไขได้โดยง่าย อัปเดตข้อความ ปรับตำแหน่ง หรือเปลี่ยนรูปลักษณ์ของลายเซ็นให้ตรงตามความต้องการของคุณ."

    # feature loop
    - title: "การลบลายเซ็นที่ราบรื่น"
      content: "ด้วยการสนับสนุนการดำเนินการ CRUD อย่างครบถ้วน เครื่องมือของเราช่วยให้สามารถลบลายเซ็นจากเอกสารของคุณได้อย่างมีประสิทธิภาพ เพื่อให้แน่ใจว่าลายเซ็นที่มีความสำคัญที่สุดจะยังคงอยู่."
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีการใช้ลายเซ็นบาร์โค้ด"
      content: |
        ตัวอย่างนี้แสดงวิธีการฝังบาร์โค้ดที่กำหนดเองลงในหน้าเอกสาร DOCX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // จัดเตรียมเอกสารที่จะทำการลงนาม
          const signature = new signatureLib.Signature('input.docx');

          // ใช้ BarcodeSignOptions เพื่อรวมบาร์โค้ดลงในเอกสาร
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // กำหนดประเภทบาร์โค้ดและพารามิเตอร์เพิ่มเติม
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // กำหนดการเว้นระยะบาร์โค้ดจากขอบหน้า
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // เลือกสีของบาร์
          signOptions.setForeColor(signatureLib.Color.RED);

          // ระบุรูปแบบฟอนต์สำหรับข้อความ
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // ระบุตำแหน่งของข้อความ
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // ลงนามและบันทึกเอกสาร
          signature.sign('output.docx', signOptions);

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
            link: "/examples/signature/formats/signature_barcode.docx"
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
    title: "สัมผัสกับฟีเจอร์หลักของเรา"
    exclude: "barcode"
    description: "สำรวจลายเซ็นและเครื่องมือที่หลากหลายที่เรามีให้."
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
    title: "ลงนามในหลายรูปแบบเอกสาร"
    exclude: "DOCX"
    description: "API Node.js via Java ช่วยให้คุณสามารถลงนามในรูปแบบไฟล์มากกว่า 60 รูปแบบ ไม่ว่าจะเป็นการเพิ่มลายเซ็นในหน้าเฉพาะหรือการวางลายเซ็นในตำแหน่งที่ต้องการ เครื่องมือของเราทำให้การใช้ลายเซ็นประเภทต่าง ๆ ทำได้ง่าย."
    items: 
          
        # format loop 1
        - name: "เพิ่มบาร์โค้ดใน PDF"
          format: "PDF"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "เพิ่มบาร์โค้ดใน DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "เพิ่มบาร์โค้ดใน JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "เพิ่มบาร์โค้ดใน PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "เพิ่มบาร์โค้ดใน XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---