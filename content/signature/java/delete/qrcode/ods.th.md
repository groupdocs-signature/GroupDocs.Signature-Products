---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Ods
productName: Java
lang: th
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Ods for Java

############################# Head ############################
head_title: "ลบลายเซ็น Qrcode จากไฟล์ Ods ผ่าน Java"
head_description: "การลบลายเซ็น Qrcode เฉพาะจากเอกสาร Ods ที่ลงนามแล้วอาจทำได้ง่ายๆ ด้วยรหัส Java แบบสั้น"

############################# Header ############################
title: "ลบลายเซ็น Qrcode ที่อยู่ใน Ods files"
description: "ลบลายเซ็น Qrcode ต่างๆ จากเอกสาร Ods การลบลายเซ็น Qrcode ต้องใช้โค้ด Java อย่างง่าย"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "รับข้อมูลเกี่ยวกับคุณสมบัติ API ของ GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API มีหลายวิธีในการประมวลผลเอกสารของคุณโดยใช้ลายเซ็นอิเล็กทรอนิกส์ ลายเซ็นดิจิทัล เช่น ข้อความ รูปภาพ ใบรับรองดิจิทัล บาร์โค้ด คิวอาร์โค้ด แสตมป์ หรือข้อมูลเมตา ลูกค้าสามารถเพิ่ม ลบ อัปเดต ตรวจสอบหรือค้นหาลายเซ็นดิจิทัลได้ที่ PDF, เอกสาร MS Word, สมุดงาน MS Excel, งานนำเสนอ MS PowerPoint, ไฟล์ Adobe Photoshop และรูปแบบรูปภาพต่างๆ มีคุณลักษณะและการตั้งค่าที่เป็นประโยชน์มากมาย
    

############################# Steps ############################
steps:
    enable: true
    title_left: "วิธีลบลายเซ็น Qrcode ออกจากเอกสาร Ods ของคุณ"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) มีคุณลักษณะที่เป็นประโยชน์สำหรับการล้างเอกสาร Ods ของ Qrcode ลายเซ็นด้วยโค้ดไม่กี่บรรทัด
        
        * ขั้นแรก ยกตัวอย่างวัตถุ Signature ที่ส่งพาธไปยังเอกสารของคุณเป็นพารามิเตอร์ Constructor
        * จากนั้นสร้างวัตถุลายเซ็นที่เหมาะสมและตั้งค่าตัวระบุที่ไม่ซ้ำกัน
        * หลังจากนั้นให้เรียกใช้เมธอด Delete ผ่านวัตถุลายเซ็นซึ่งต้องถูกลบ
        * สุดท้าย ประมวลผลผลการดำเนินการ

    title_right: "ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for Java ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * ดาวน์โหลด GroupDocs.Signature for Java เวอร์ชันล่าสุดจาก [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";
        // Set up output file
        String outputFilePath = "output.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to delete
        QrCodeSignature signatureToDelete = new QrCodeSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "การลงนามด้วยลายเซ็น Qrcode การสาธิตสด"
    content: |
       เพิ่มลายเซ็นอิเล็กทรอนิกส์ต่างๆ ลงในไฟล์ Ods โดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family)          

############################# More Formats ############################
more_formats:
    enable: true
    title: "ลบลายเซ็น Qrcode ของคุณด้วย Java"
    content: |
        "การลบลายเซ็นอิเล็กทรอนิกส์ที่เพิ่มลงในรูปแบบเอกสารต่างๆ ลบลายเซ็นอย่างรวดเร็วโดยไม่ต้องใช้รหัสพิเศษ"
    format: 
       
       
back_to_top:
    enable: true
---