---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:07
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
platform: "Net"
platform_tag: "net"

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
title: "เซ็นเอกสาร<br>ผ่านทาง .NET API"
description: "ลงนามในเอกสารดิจิทัลและรูปภาพบนแพลตฟอร์มใดก็ได้โดยใช้ API ที่ยืดหยุ่นและโซลูชันตามแอปสำหรับโปรแกรมเมอร์และผู้ใช้ปลายทาง"
words:
  for: "สำหรับ"

actions:
  main: "ดาวน์โหลด NuGet ฟรี"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "พร้อมที่จะเริ่มต้นหรือยัง?"
  description: "ลองใช้คุณสมบัติ GroupDocs.Signature ฟรีหรือขอใบอนุญาต"

release:
  title: "เวอร์ชัน {0} เปิดตัวแล้ว"
  notes: "ดูว่ามีอะไรใหม่"
  downloads: "ดาวน์โหลด"

code:
  title: "ลงนามไฟล์ PDF ใน C #"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // เลือกเอกสาร PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // ระบุข้อความ
        var options = new TextSignOptions("John Smith")
        {
            // กำหนดสี
            ForeColor = Color.Red
        };
        // ลงนามในเอกสารและบันทึกลงไฟล์
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature ภาพรวม"
  description: "API สำหรับดำเนินการลงนามเอกสารและการดำเนินการที่เกี่ยวข้องในแอปพลิเคชัน .NET"
  features:
    # feature loop
    - title: "การเพิ่มลายเซ็นให้กับเอกสารทางธุรกิจใน C#"
      content: "การลงนามเอกสาร: ด้วย GroupDocs.Signature สำหรับ .NET คุณสามารถเพิ่มลายเซ็นหลายประเภท เช่น ข้อความ รูปภาพ บาร์โค้ด และใบรับรองดิจิทัล ลงในเอกสาร PDF และ Office API นี้ช่วยให้คุณสามารถลงนามในเอกสารของคุณด้วยข้อมูลได้เกือบทุกประเภท รวมถึงข้อมูลเมตาที่ซ่อนอยู่"

    # feature loop
    - title: "กำลังประมวลผลเอกสารที่ลงนาม"
      content: "การประมวลผลเพิ่มเติม: คุณสามารถดำเนินการที่มีประสิทธิภาพกับเอกสารที่ลงนามได้โดยใช้ GroupDocs.Signature ซึ่งรวมถึงการค้นหาลายเซ็นที่มีอยู่ในเอกสารทางธุรกิจและการตรวจสอบโดยใช้เกณฑ์เฉพาะ นอกจากนี้ คุณยังสามารถดึงข้อมูลเอกสารและดูตัวอย่างหน้าผ่าน .NET API นี้"

    # feature loop
    - title: "การปรับแต่งผลลัพธ์"
      content: "GroupDocs.Signature สำหรับ .NET มีตัวเลือกการปรับแต่งที่หลากหลาย คุณสามารถวางตำแหน่งลายเซ็นได้อย่างแม่นยำทุกที่บนหน้าเอกสาร และปรับลักษณะที่ปรากฏโดยใช้การตั้งค่าที่หลากหลาย นอกจากนี้ API นี้ยังรองรับการบันทึกเอกสารที่ประมวลผลแล้วในรูปแบบที่รองรับที่หลากหลาย"

############################# Platforms ############################
platforms:
  enable: true
  title: "ความเป็นอิสระของแพลตฟอร์ม"
  description: "GroupDocs.Signature สำหรับ. NET รองรับระบบปฏิบัติการเฟรมเวิร์กและผู้จัดการแพ็คเกจต่อไปนี้"
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
    GroupDocs.Signature สำหรับ .NET รองรับการดำเนินการกับ [รูปแบบไฟล์](https://docs.groupdocs.com/signature/net/supported-document-formats/) ต่อไปนี้
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
  description: "การลงนาม PDF เอกสาร Office และรูปภาพอย่างรวดเร็วและแม่นยำ"

  items:
    # feature loop
    - icon: "sign"
      title: "การลงนามเอกสาร"
      content: "เพิ่มลายเซ็นที่รองรับหนึ่งหรือหลายประเภทอย่างถูกต้องในตำแหน่งที่ระบุในเอกสารทางธุรกิจ"

    # feature loop
    - icon: "custom"
      title: "ปรับแต่งลายเซ็น"
      content: "ใช้คุณสมบัติต่างๆ เช่น สี แบบอักษร เส้นขอบ การหมุน ฯลฯ เพื่อกำหนดค่าลักษณะที่ปรากฏของลายเซ็น"

    # feature loop
    - icon: "password"
      title: "การป้องกันรหัสผ่านเอกสาร"
      content: "รักษาความปลอดภัยเอกสารบางประเภทโดยการตั้งรหัสผ่านหลังจากลงนาม"

    # feature loop
    - icon: "protect"
      title: "การป้องกันจากการเปลี่ยนแปลง"
      content: "ป้องกันการเปลี่ยนแปลงเอกสารทางธุรกิจที่สำคัญหลังจากต่อท้ายลายเซ็นด้วยใบรับรองดิจิทัล"

    # feature loop
    - icon: "convert"
      title: "แปลงไฟล์ที่ลงนามเป็นรูปแบบอื่น"
      content: "แปลงไฟล์ที่ลงนามเป็นรูปแบบที่ต้องการ เช่น การบันทึกเอกสาร Word เป็น PDF"

    # feature loop
    - icon: "preview"
      title: "แยกตัวอย่างหน้า"
      content: "แยกหน้าออกจากเอกสารที่ลงนามเป็นภาพแต่ละภาพเพื่อการประมวลผลในอนาคต"

    # feature loop
    - icon: "search"
      title: "ค้นหาลายเซ็นในเอกสาร"
      content: "รับข้อมูลเกี่ยวกับลายเซ็นที่เพิ่มไว้ก่อนหน้านี้ในเอกสารเฉพาะ"

    # feature loop
    - icon: "validate"
      title: "ตรวจสอบเอกสารที่ลงนาม"
      content: "ตรวจสอบการลงนามเอกสารที่เหมาะสมโดยใช้คุณสมบัติการตรวจสอบ"

    # feature loop
    - icon: "update"
      title: "อัปเดตหรือลบลายเซ็น"
      content: "เปลี่ยนตำแหน่งลายเซ็นเฉพาะบนหน้า แก้ไขข้อความ หรือลบลายเซ็นได้อย่างง่ายดายโดยไม่มีปัญหาใดๆ"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างโค้ด"
  description: "กรณีการใช้งานบางอย่างของ GroupDocs.Signature ทั่วไปสำหรับการดำเนินการ .NET"
  items:
    # code sample loop
    - title: "เพิ่มรหัส QR ลงใน PDF"
      content: |
        การเพิ่ม [QR-codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) ลงในหน้าเฉพาะของเอกสาร PDF สามารถปรับปรุงกระบวนการทางธุรกิจได้ ด้านล่างนี้คือตัวอย่างวิธีเพิ่มโค้ด QR โดยใช้ GroupDocs.Signature
        {{< landing/code title="วิธีใส่รหัส QR เป็น PDF">}}
        ```csharp {style=abap}
        // โหลดเอกสารเพื่อลงนาม
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // สร้างตัวเลือกโค้ด QR พร้อมข้อความที่กำหนดไว้ล่วงหน้า
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // กำหนดค่าประเภทและตำแหน่งการเข้ารหัสโค้ด QR บนเพจ
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // ลงนามในเอกสารและบันทึกเป็นไฟล์ผลลัพธ์
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "การปกป้องเอกสาร DOCX โดยใช้ใบรับรองดิจิทัล"
      content: |
        คุณสามารถ[ปกป้องเอกสาร](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) ได้โดยใช้ลายเซ็นส่วนตัวหรือลายเซ็นขององค์กรที่จัดเก็บเป็นใบรับรองดิจิทัล เอกสารที่ได้รับการคุ้มครองดังกล่าวไม่สามารถแก้ไขได้โดยไม่ทำให้ลายเซ็นเป็นโมฆะ
        {{< landing/code title="ต่อไปนี้คือวิธีการตรวจสอบความสมบูรณ์ของเอกสาร">}}
        ```csharp {style=abap}   
        // โหลดเอกสารที่จะเซ็นชื่อแบบดิจิทัล
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // ระบุตัวเลือกการเซ็นชื่อดิจิทัลและระบุเส้นทางไปยังไฟล์ใบรับรอง
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // ตั้งรหัสผ่านใบรับรอง
                Password = "1234567890"
            };
            // ลงนามในเอกสารและบันทึกลงในเส้นทางที่ต้องการ
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
