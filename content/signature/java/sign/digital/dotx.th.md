---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dotx
productName: Java
lang: th
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dotx for Java

############################# Head ############################
head_title: "การเพิ่มลายเซ็นอิเล็กทรอนิกส์ดิจิทัลลงในไฟล์ Dotx ด้วย Java"
head_description: "ใส่ลายเซ็นดิจิทัลในไฟล์ Dotx สำหรับ Java โดยใช้โค้ดสองสามบรรทัด ใช้ GroupDocs Document Signature API เพื่อลงนามรูปแบบไฟล์มากมาย"

############################# Header ############################
title: "eSign Dotx ไฟล์ที่มีลายเซ็น Digital ใน Java"
description: "วิธีเพิ่มลายเซ็น Digital ด้วยโค้ด Java สองสามบรรทัด"
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
    title: "เกี่ยวกับ GroupDocs.Signature for Java ลายเซ็นดิจิทัล API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) เป็น API ที่ได้รับความนิยมในการกำหนดเอกสารด้วยลายเซ็นอิเล็กทรอนิกส์ดิจิทัล พร้อมใบรับรองดิจิทัล สำหรับลายเซ็นดิจิทัล API ใช้ไฟล์ใบรับรอง PFX เพื่อออกเอกสารด้วยคีย์ส่วนตัวและสาธารณะที่ป้องกันด้วยรหัสผ่าน ลายเซ็นดิจิทัลอาจใช้รับรองเอกสารทางธุรกิจด้วยหน้าเฉพาะ eSign PDF รับรองเอกสาร Microsoft Office ทั้งหมด เช่น Words, Excel, ไฟล์ Powerpoint และเอกสาร Open Office ลูกค้าสามารถจัดการลายเซ็นได้อย่างง่ายดาย เช่น แก้ไข ลบ หรือปรับเปลี่ยน API ให้วิธีการค้นหาและตรวจสอบลายเซ็น นอกจากนี้ยังมีความสามารถมากมายสำหรับการปรับแต่งลายเซ็น
    

############################# Steps ############################
steps:
    enable: true
    title_left: "ขั้นตอนในการลงนาม Dotx กับ Digital ใน Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ให้ความสามารถในการลงนามในเอกสาร Dotx ด้วยลายเซ็น Digital อย่างรวดเร็วและง่ายดาย
        
        * สร้างอินสแตนซ์ของคลาส Signature โดยให้ไฟล์ Dotx ที่ควรเซ็นชื่อเป็นเส้นทางหรือสตรีมหน่วยความจำ
        * สร้างอินสแตนซ์คลาส SignOptions และตั้งค่าข้อมูลที่ต้องการทั้งหมด
        * เรียกใช้เมธอด Signature.Sign() ผ่านไฟล์เอาต์พุต Dotx หรือสตรีมหน่วยความจำ

    title_right: " ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for Java ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * รับ GroupDocs.Signature for Java ล่าสุดจาก [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Dotx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "การลงนามเอกสาร Dotx ด้วย Digital Live Demo"
    content: |
       ลงชื่อไฟล์ Dotx ด้วยลายเซ็นต่างๆ ทันทีโดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) สาธิตออนไลน์ฟรีรอคุณอยู่          

############################# More Formats ############################
more_formats:
    enable: true
    title: "ลายเซ็น Digital อื่นๆ ที่รองรับสำหรับ Java"
    content: |
        "คุณยังสามารถเซ็นชื่อ Dotx ด้วยลายเซ็นประเภทอื่นๆ โปรดดูรายการด้านล่าง"
    format: 
       
       
back_to_top:
    enable: true
---