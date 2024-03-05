---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:01
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: th
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

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
head_title: ".NET, Java, Cloud API และแอปลายเซ็นเอกสารออนไลน์"
head_description: "รับโซลูชันลายเซ็นอิเล็กทรอนิกส์เอกสารแบบครบวงจรสำหรับ .NET, Java และแอปพลิเคชันบนคลาวด์ เซ็นชื่อในรูปแบบเอกสารทั่วไปทางออนไลน์โดยใช้คุณสมบัติการลากและวางที่เรียบง่าย"

############################# Header ############################
title: "เซ็นเอกสาร<br>ผ่านทางจาวา API"
description: "ลงนามในเอกสารดิจิทัลและรูปภาพบนแพลตฟอร์มใดก็ได้โดยใช้ API ที่ยืดหยุ่นและโซลูชันตามแอปสำหรับโปรแกรมเมอร์และผู้ใช้ปลายทาง"
words:
  for: "สำหรับ"

actions:
  main: "ดาวน์โหลดฟรี Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "พร้อมที่จะเริ่มต้นหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Signature ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} เปิดตัวแล้ว"
  notes: "ดูว่ามีอะไรใหม่"
  downloads: "ดาวน์โหลด"

code:
  title: "ลงนามไฟล์ PDF ใน Java"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // เลือกเอกสาร PDF
    Signature signature = new Signature("sample.pdf");
    
    // ระบุข้อความ
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // ลงนามในเอกสารและบันทึกลงไฟล์
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature ภาพรวม"
  description: "API สำหรับดำเนินการลงนามเอกสารและการดำเนินการที่เกี่ยวข้องในแอปพลิเคชัน Java"
  features:
    # feature loop
    - title: "ปรับปรุงเอกสารทางธุรกิจด้วยลายเซ็นดิจิทัลใน Java"
      content: "การลงนามที่รวดเร็วและปรับแต่งได้: GroupDocs.Signature สำหรับ Java นำเสนอตัวเลือกลายเซ็นดิจิทัลที่หลากหลายสำหรับ PDF รูปภาพ และเอกสาร Office คุณสามารถใช้ข้อความ บาร์โค้ด รหัส QR ใบรับรองดิจิทัล รูปภาพ หรือข้อมูลเมตาที่ซ่อนอยู่ได้ การประมวลผลเอกสารรวดเร็วและมีประสิทธิภาพ"

    # feature loop
    - title: "จัดการเอกสารที่ลงนาม"
      content: "การประมวลผลเอกสารขั้นสูงเกี่ยวข้องกับการดำเนินการที่มีประสิทธิภาพกับเอกสารที่เซ็นชื่อโดยใช้ GroupDocs.Signature สำหรับ Java คุณสามารถค้นหาและตรวจสอบความถูกต้องของลายเซ็นที่ถูกเพิ่มลงในเอกสารทางธุรกิจโดยใช้เกณฑ์ที่เป็นประโยชน์ต่างๆ นอกจากนี้ คุณสามารถเข้าถึงข้อมูลโดยละเอียดเกี่ยวกับเอกสารหรือรับภาพตัวอย่างของหน้าต่างๆ ได้"

    # feature loop
    - title: "ตัวเลือกเอาต์พุตที่หลากหลาย"
      content: "ตัวเลือกการลงนามที่มีประสิทธิภาพช่วยให้คุณปรับแต่งเอาต์พุตสำหรับเอกสารที่ลงนามด้วย GroupDocs.Signature สำหรับ Java คุณสามารถวางตำแหน่งลายเซ็นบนหน้าเอกสารใดก็ได้อย่างแม่นยำ และกำหนดค่าลักษณะที่ปรากฏได้หลายวิธี Java API รองรับการบันทึกเอกสารทางธุรกิจที่เซ็นชื่อในรูปแบบที่รองรับมากมาย และมีตัวเลือกสำหรับการรักษาความปลอดภัยด้วยรหัสผ่าน"

############################# Platforms ############################
platforms:
  enable: true
  title: "ความเป็นอิสระของแพลตฟอร์ม"
  description: "GroupDocs.Signature สำหรับ Java รองรับระบบปฏิบัติการ เฟรมเวิร์ก และตัวจัดการแพ็คเกจต่อไปนี้"
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    GroupDocs.Signature สำหรับ Java รองรับการดำเนินการกับ [รูปแบบไฟล์](https://docs.groupdocs.com/signature/java/supported-document-formats/) ต่อไปนี้
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
  title: "คุณสมบัติ GroupDocs.Signature"
  description: "การลงนาม PDF เอกสาร Office และรูปภาพด้วยลายเซ็นดิจิทัล"

  items:
    # feature loop
    - icon: "sign"
      title: "การเพิ่มลายเซ็น"
      content: "ลงนามในเอกสารโดยใช้ลายเซ็นหลายประเภทที่รองรับโดยการวางลายเซ็นดิจิทัลในตำแหน่งใดก็ได้บนหน้าใดก็ได้อย่างแม่นยำ"

    # feature loop
    - icon: "custom"
      title: "การปรับแต่งผลลัพธ์"
      content: "ปรับแต่งลักษณะลายเซ็นโดยการปรับสี แบบอักษร เส้นขอบ การหมุน และคุณสมบัติอื่นๆ เพื่อให้ได้ผลลัพธ์ตามที่ต้องการ"

    # feature loop
    - icon: "password"
      title: "การรักษาความปลอดภัยเอกสารด้วยรหัสผ่าน"
      content: "สำหรับเอกสารที่รองรับหลายประเภท คุณสามารถป้องกันเอกสารที่ลงนามด้วยรหัสผ่านได้"

    # feature loop
    - icon: "protect"
      title: "ป้องกันการเปลี่ยนแปลงโดยไม่ได้รับอนุญาต"
      content: "ปกป้องเอกสารทางธุรกิจที่สำคัญที่ลงนามด้วยใบรับรองดิจิทัลจากการแก้ไขโดยไม่ได้รับอนุญาต"

    # feature loop
    - icon: "convert"
      title: "ได้ผลลัพธ์ในรูปแบบที่ต้องการ"
      content: "รับไฟล์ผลลัพธ์ที่ลงนามในรูปแบบที่รองรับได้อย่างง่ายดาย คุณยังสามารถแปลงเอกสาร MS Word เป็น PDF ได้อย่างง่ายดาย"

    # feature loop
    - icon: "preview"
      title: "การแสดงตัวอย่างเอกสาร"
      content: "บันทึกหน้าใดๆ ของเอกสารเป็นรูปภาพสำหรับการประมวลผลในอนาคต"

    # feature loop
    - icon: "search"
      title: "กำลังค้นหาลายเซ็น"
      content: "สามารถรับข้อมูลเกี่ยวกับลายเซ็นที่เพิ่มไว้ก่อนหน้านี้ในเอกสารเฉพาะได้"

    # feature loop
    - icon: "validate"
      title: "กำลังตรวจสอบเอกสาร"
      content: "ตรวจสอบความถูกต้องของลายเซ็นในเอกสารที่ลงนาม"

    # feature loop
    - icon: "update"
      title: "การจัดการลายเซ็น"
      content: "เมื่อวางลายเซ็นบนหน้าเอกสารแล้ว จะสามารถลบ ย้าย หรืออัปเดตลายเซ็นได้ตามต้องการ"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างโค้ด"
  description: "กรณีการใช้งานบางอย่างของ GroupDocs.Signature ทั่วไปสำหรับการดำเนินการ Java"
  items:
    # code sample loop
    - title: "เสริมเอกสาร PDF ด้วยรหัส QR"
      content: |
        การปรับปรุงกระบวนการทางธุรกิจโดยการเพิ่ม [QR-codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) ลงในหน้าเฉพาะของเอกสาร PDF อาจมีคุณค่า มีตัวอย่างวิธีเพิ่มโค้ด QR โดยใช้ GroupDocs.Signature สำหรับ Java
        {{< landing/code title="เสริมเอกสาร PDF ด้วยรหัส QR">}}
        ```java {style=abap}
        // โหลดเอกสารเพื่อลงนาม
        Signature signature = new Signature("file_to_sign.pdf");
        
        // สร้างตัวเลือกโค้ด QR พร้อมข้อความที่กำหนดไว้ล่วงหน้า
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // กำหนดค่าประเภทและตำแหน่งการเข้ารหัสโค้ด QR บนเพจ
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // ลงนามในเอกสารและบันทึกเป็นไฟล์ผลลัพธ์
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "ใช้ลายเซ็นดิจิทัลเพื่อปกป้อง DOCX"
      content: |
        คุณสามารถ[ปกป้องเอกสาร](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) ได้โดยใช้ลายเซ็นส่วนตัวหรือลายเซ็นขององค์กรที่จัดเก็บเป็นใบรับรองดิจิทัล เอกสารที่มีการรักษาความปลอดภัยด้วยใบรับรองไม่สามารถเปลี่ยนแปลงได้โดยไม่ทำให้ลายเซ็นเป็นโมฆะ
        {{< landing/code title="ใช้ลายเซ็นดิจิทัลเพื่อปกป้อง DOCX">}}
        ```java {style=abap}   
        // โหลดเอกสารที่จะเซ็นชื่อแบบดิจิทัล
        Signature signature = new Signature("file_to_sign.docx");
        
        // ระบุตัวเลือกการเซ็นชื่อดิจิทัลและระบุเส้นทางไปยังไฟล์ใบรับรอง
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // ตั้งรหัสผ่านใบรับรอง
        options.setPassword("1234567890");

        // ลงนามในเอกสารและบันทึกลงในเส้นทางที่ต้องการ
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
