



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: th
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "สร้าง QR code ในเอกสาร XLSX ด้วย JavaScript"
head_description: "ใช้ API GroupDocs.Signature เพื่อสร้างและรวมบาร์โค้ด 2 มิติในไฟล์ XLSX วาง QR code ได้อย่างสะดวกบนหน้ากระดาษเอกสารใดๆ"

############################# Header ############################
title: "สร้าง QR codes สำหรับ XLSX" 
description: "สร้างและฝังบาร์โค้ด 2 มิติที่มาพร้อมกับเนื้อหาที่ปรับแต่งได้ รวมถึงข้อความและข้อมูลตัวเลขในเอกสารประเภทต่างๆ เช่น PDFs, Word, Excel และ ภาพ ด้วย GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ทดลองใช้ฟรี"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "สำรวจความสามารถของ GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) นำเสนอเครื่องมือปรับปรุงเอกสารที่ล้ำสมัย ช่วยให้สามารถสร้างและฝังลายเซ็นหลากหลายประเภท รวมถึง QR codes ในรูปแบบไฟล์ยอดนิยม ลงนามและรักษาความปลอดภัย PDF, Word, Excel, PowerPoint และภาพ ด้วยลายเซ็นประเภทข้อความ, รูปภาพ, บาร์โค้ด, QR code, เมตาดาทา, ดิจิทัล และตราประทับ

############################# Steps ############################
steps:
    enable: true
    title: "คู่มือการสร้างและฝัง QR code ในตำแหน่งใดก็ได้ภายใน XLSX"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) รองรับการสร้าง QR codes ในรูปแบบที่ใช้กันทั่วไปและสามารถรวมเข้ากับหน้า XLSX ได้ รองรับ QR code ประเภทต่างๆ มากกว่า 10 ประเภท เราจึงสามารถรวมเข้ากับแอปพลิเคชัน Node.js via Java ได้อย่างราบรื่น เพิ่มความสามารถในการลงนาม QR code ให้กับแอปพลิเคชันของคุณ.
      
      1. ให้ไฟล์หรือสตรีม XLSX สำหรับการลงนาม QR code.
      2. ป้อนข้อความที่ต้องการในอินสแตนซ์ QrCodeSignOptions.
      3. ปรับการตั้งค่าทางภาพ เช่น สี ตำแหน่ง ขนาด เป็นต้น.
      4. บันทึกเอกสารที่มี QR code.
   
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

        // สร้างตัวอย่าง Signature และส่งเอกสารไปยังพาธ
        const signature = new signatureLib.Signature('input.xlsx');

        // ใช้ QrCodeSignOptions เพื่อแทรก QR code ในเอกสาร
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // กำหนดประเภทลายเซ็นและตำแหน่งบนหน้า
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // บันทึกเอกสารที่มี QR code ใหม่ที่เพิ่มเข้ามา
        signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "การรวมลายเซ็นและ QR code อย่างครบถ้วน"
  description: "ด้วย API GroupDocs.Signature for Node.js via Java คุณสามารถจัดการลายเซ็นได้หลากหลายประเภทได้ง่ายดาย สร้าง ปรับแต่ง ตรวจสอบ ค้นหา และลบลายเซ็นอย่างมีประสิทธิภาพในเอกสารประเภทต่างๆ มอบความยืดหยุ่นที่ไม่เปรียบเทียบให้กับกระบวนการทำงานของคุณ"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "คุณสมบัติของลายเซ็นและ QR code"
  features:
    # feature loop
    - title: "การลงนามเอกสารหลายรูปแบบ"
      content: "เพิ่มหลายประเภทของลายเซ็น รวมถึงลายเซ็นประเภทข้อความ, รูปภาพ, บาร์โค้ด, QR code, และตราประทับ ลงในรูปแบบเอกสารที่รองรับใดๆ วางพวกเขาในหน้าที่ต้องการ และจัดการเมตาดาทาของเอกสาร มั่นใจในความปลอดภัยของเอกสารผ่านใบรับรองดิจิทัลเพื่อป้องกันการเปลี่ยนแปลงที่ไม่ได้รับอนุญาต"

    # feature loop
    - title: "การตรวจสอบลายเซ็นอย่างมีประสิทธิภาพ"
      content: "ตรวจสอบลายเซ็นทั้งหมดภายในเอกสารเพื่อให้แน่ใจว่าตรงตามมาตรฐานที่กำหนด ค้นหาและตรวจสอบลายเซ็นได้อย่างง่ายดายผ่านฟังก์ชันการค้นหาที่มีในตัว"

    # feature loop
    - title: "การแก้ไขลายเซ็นที่ยืดหยุ่น"
      content: "ปรับปรุงหรือตัดต่อรายละเอียดของลายเซ็นที่มีอยู่ ปรับเปลี่ยนเนื้อหา ตำแหน่ง ขนาด และสีให้เหมาะสมกับความต้องการของเอกสารหลังจากการลงนามครั้งแรก"

    # feature loop
    - title: "การลบลายเซ็นได้ง่าย"
      content: "ลบลายเซ็นที่ไม่ต้องการหรือไม่เป็นปัจจุบัน ซึ่งรวมถึงใบรับรองดิจิทัล ได้อย่างง่ายดาย การควบคุมการจัดการลายเซ็นอย่างเต็มรูปแบบช่วยให้เอกสารของคุณมีความสะอาดและเป็นระเบียบ"
      
  code_samples_ext:
    # code sample ext loop
    - title: "ปรับแต่ง QR code ที่สร้างขึ้น"
      content: |
        ตัวอย่างนี้ให้รายละเอียดเกี่ยวกับกระบวนการเพิ่ม QR code ที่ปรับแต่งลงในหน้า XLSX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // รับเอกสารที่จะลงนามและส่งไปยัง Signature
          const signature = new signatureLib.Signature('input.xlsx');

          // ตั้งค่าตัวเลือก QR code พร้อมข้อความที่ต้องการ
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // ระบุตำแหน่ง QR code บนหน้า
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // ระบุกระแสการเซ็นชื่อ
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // เลือกสีของ QR code
          signOptions.setForeColor(signatureLib.Color.RED);

          // กำหนดตัวเลือกฟอนต์สำหรับข้อความที่แนบมา
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // ปรับแต่งสีพื้นหลังและแปรงสำหรับ QR code
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // ฝัง QR code ลงในเอกสาร
          signature.sign('output.xlsx', signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.xlsx"
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
    title: "ทำความเข้าใจกับความสามารถหลักของเรา"
    exclude: "qrcode"
    description: "เรามีการให้บริการลายเซ็นรูปแบบและการดำเนินการที่กว้างขวางซึ่งปรับให้เหมาะสมกับความต้องการของคุณ"
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "รวม QR codes กับรูปแบบไฟล์ต่างๆ"
    exclude: "XLSX"
    description: "ใช้ API Node.js via Java เพื่อสร้าง QR codes และฝังลงในรูปแบบไฟล์ที่ใช้กันอย่างแพร่หลาย สื่อสารข้อมูลสำคัญภายในบาร์โค้ดเพื่อการรวมเข้าที่ราบรื่นและการเรียกคืนในอนาคต"
    items: 
          
        # format loop 1
        - name: "QR-Code สำหรับ PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "QR-Code สำหรับ DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Code สำหรับ JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "QR-Code สำหรับ PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Code สำหรับ XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---