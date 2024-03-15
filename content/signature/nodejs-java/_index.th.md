---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: th
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Node.js Digital Signature API - GroupDocs.Signature"
head_description: "ผสานรวมลายเซ็นอิเล็กทรอนิกส์ที่ปลอดภัยในแอป Node.js เข้ากับ GroupDocs.Signature ปรับปรุงเวิร์กโฟลว์การเซ็นเอกสารอย่างง่ายดายและมีประสิทธิภาพ"

############################# Header ############################
title: "เซ็นเอกสาร<br>ด้วย Node.js API"
description: "ลงนามในเอกสารดิจิทัลและรูปภาพบนแพลตฟอร์มใดก็ได้โดยใช้ API ที่ยืดหยุ่นและโซลูชันตามแอปสำหรับโปรแกรมเมอร์และผู้ใช้ปลายทาง"
words:
  for: "สำหรับ"

actions:
  main: "ดาวน์โหลดจาก NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "พร้อมที่จะเริ่มต้นหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Signature ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} เปิดตัวแล้ว"
  notes: "ดูว่ามีอะไรใหม่"
  downloads: "ดาวน์โหลด"

code:
  title: "การลงนาม PDF โดย Node.js"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // เลือกเอกสาร PDF
    let signature = new Signature("sample.pdf");
    
    // ระบุข้อความ
    let options = new TextSignOptions("John Smith");
    
    // กำหนดสี
    options.ForeColor = Color.Red;
    
    // ลงนามในเอกสารและบันทึกลงไฟล์
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature ภาพรวม"
  description: "ไลบรารีการลงนามเอกสารที่พร้อมใช้ในแอปพลิเคชัน Node.js"
  features:
    # feature loop
    - title: "โซลูชันลายเซ็นดิจิทัลสำหรับเอกสารทางธุรกิจด้วย Node.js"
      content: "GroupDocs.Signature for Node.js via Java นำเสนอชุดตัวเลือกลายเซ็นดิจิทัลที่ครอบคลุมสำหรับ PDF, เอกสาร Office และรูปภาพ ข้อความ บาร์โค้ด รูปภาพ ใบรับรองดิจิทัล และข้อมูลเมตามีให้บริการ การประมวลผลเอกสารที่คล่องตัวทำให้มั่นใจได้ถึงประสิทธิภาพ"

    # feature loop
    - title: "การจัดการขั้นสูงของเอกสารที่ลงนาม"
      content: "GroupDocs.Signature ช่วยให้คุณสามารถประมวลผลเอกสารที่ลงนามแล้ว ค้นหาและตรวจสอบลายเซ็นโดยใช้เกณฑ์ต่างๆ นอกจากนี้ ดึงข้อมูลเอกสารโดยละเอียดหรือสร้างภาพตัวอย่างหน้าต่างๆ"

    # feature loop
    - title: "รูปแบบเอาต์พุตที่หลากหลาย"
      content: "โซลูชันของเราให้การควบคุมรูปแบบเอาต์พุตของเอกสารที่เซ็นชื่ออย่างครอบคลุม วางตำแหน่งลายเซ็นบนหน้าใดๆ ได้อย่างแม่นยำและปรับแต่งลักษณะที่ปรากฏ บันทึกเอกสารที่ลงนามในรูปแบบที่รองรับมากมาย และเลือกรักษาความปลอดภัยด้วยรหัสผ่าน"

############################# Platforms ############################
platforms:
  enable: true
  title: "ความเป็นอิสระของแพลตฟอร์ม"
  description: "GroupDocs.Signature for Node.js via Java ดำเนินการประมวลผลเอกสารด้วยระบบปฏิบัติการต่างๆ"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    GroupDocs.Signature for Node.js via Java อำนวยความสะดวกในการดำเนินการสำหรับ [รูปแบบไฟล์ยอดนิยม](https://docs.groupdocs.com/signature/java/supported-document-formats/)
  groups:
    # group loop
    - color: "green"
      content: |
        ### รูปแบบของ Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### รูปภาพและรูปแบบอื่นๆ
        * **แบบพกพา:** PDF
        * **รูปภาพ:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **รูปแบบสำนักงานอื่นๆ:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### รูปแบบอื่นๆ
        * **เว็บ:** HTML, MHTML
        * **หอจดหมายเหตุ:** ZIP, TAR, 7Z
        * **ใบรับรอง:** PFX

############################# Features ############################
features:
  enable: true
  title: "คุณสมบัติของ GroupDocs.Signature"
  description: "ลงนาม PDF เอกสาร Office และรูปภาพด้วยลายเซ็นดิจิทัล"

  items:
    # feature loop
    - icon: "sign"
      title: "ลายเซ็นธุรกิจ"
      content: "ใช้ลายเซ็นประเภทต่างๆ เพื่อลงนามในเอกสาร วางลายเซ็นดิจิทัลในตำแหน่งใด ๆ ของหน้าได้อย่างแม่นยำ"

    # feature loop
    - icon: "custom"
      title: "การปรับแต่งรูปลักษณ์ของลายเซ็น"
      content: "ปรับแต่งลักษณะการมองเห็นของลายเซ็นโดยการปรับสี แบบอักษร เส้นขอบ การหมุน และอื่นๆ เพื่อให้ได้ผลลัพธ์ตามที่คุณต้องการ"

    # feature loop
    - icon: "password"
      title: "เอกสารที่มีการป้องกันด้วยรหัสผ่าน"
      content: "สำหรับรูปแบบเอกสารที่รองรับหลายรูปแบบ ให้ปกป้องเอกสารที่ลงนามด้วยรหัสผ่านเพื่อเพิ่มความปลอดภัย"

    # feature loop
    - icon: "protect"
      title: "การป้องกันการแก้ไขโดยไม่ได้รับอนุญาต"
      content: "ปกป้องเอกสารทางธุรกิจที่สำคัญที่ลงนามด้วยใบรับรองดิจิทัลจากการดัดแปลงโดยไม่ได้รับอนุญาต"

    # feature loop
    - icon: "convert"
      title: "รูปแบบเอาต์พุตที่ต้องการ"
      content: "รับเอกสารที่ลงนามในรูปแบบที่รองรับได้อย่างง่ายดาย แปลงเอกสาร MS Word เป็นรูปแบบ PDF ได้อย่างง่ายดาย"

    # feature loop
    - icon: "preview"
      title: "การดูตัวอย่างเอกสาร"
      content: "บันทึกหน้าเอกสารแต่ละหน้าเป็นรูปภาพสำหรับความต้องการในอนาคต"

    # feature loop
    - icon: "search"
      title: "ค้นหาลายเซ็น"
      content: "รับข้อมูลเกี่ยวกับลายเซ็นที่เพิ่มไว้ก่อนหน้านี้ภายในเอกสารของคุณ"

    # feature loop
    - icon: "validate"
      title: "การตรวจสอบเอกสาร"
      content: "ตรวจสอบความถูกต้องของลายเซ็นที่แสดงในเอกสารใด ๆ"

    # feature loop
    - icon: "update"
      title: "การจัดการลายเซ็น"
      content: "ลบ ย้ายตำแหน่ง หรือแก้ไขลายเซ็นใดๆ ที่วางอยู่บนหน้าเอกสารใดๆ"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างโค้ด"
  description: "ตัวอย่างที่แสดงให้เห็นการดำเนินงานทั่วไปของ GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "ทำเครื่องหมาย PDF ด้วยรหัส QR"
      content: |
        การรวม [บาร์โค้ด](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) ลงในหน้าเอกสาร PDF เฉพาะสามารถปรับปรุงกระบวนการทางธุรกิจได้ ส่วนนี้จะแสดงตัวอย่างการเพิ่มโค้ด QR โดยใช้ GroupDocs.Signature for Node.js via Java
        {{< landing/code title="วิธีใส่รหัส QR เป็น PDF">}}
        ```javascript {style=abap}
        // โหลดเอกสารเพื่อลงนาม
        let signature = new Signature("file_to_sign.pdf");
        
        // สร้างตัวเลือกโค้ด QR พร้อมข้อความที่กำหนดไว้ล่วงหน้า
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // กำหนดค่าประเภทและตำแหน่งการเข้ารหัสโค้ด QR บนเพจ
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // ลงนามในเอกสารและบันทึกเป็นไฟล์ผลลัพธ์
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "การปกป้อง DOCX ด้วยลายเซ็นดิจิทัล"
      content: |
        [ปกป้องเอกสารของคุณ](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) ด้วยลายเซ็นตามใบรับรองดิจิทัล ลายเซ็นดิจิทัลช่วยปกป้องเอกสารทางธุรกิจของคุณจากการเปลี่ยนแปลงเนื้อหา
        {{< landing/code title="ต่อไปนี้คือวิธีการตรวจสอบความสมบูรณ์ของเอกสาร">}}
        ```javascript {style=abap}   
        // โหลดเอกสารที่จะเซ็นชื่อแบบดิจิทัล
        let signature = new Signature("file_to_sign.docx");
        
        // ระบุตัวเลือกการเซ็นชื่อดิจิทัลและระบุเส้นทางไปยังไฟล์ใบรับรอง
        let options = new DigitalSignOptions("certificate.pfx");

        // ตั้งรหัสผ่านใบรับรอง
        options.Password = "1234567890";

        // ลงนามในเอกสารและบันทึกลงในเส้นทางที่ต้องการ
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
