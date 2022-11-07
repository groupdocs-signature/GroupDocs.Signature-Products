---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Xlsm
productName: Java
lang: th
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Xlsm for Java

############################# Head ############################
head_title: "สร้างลายเซ็นอิเล็กทรอนิกส์ข้อความไปยังไฟล์ Xlsm ด้วย Java"
head_description: "ใส่ Text eSignature ในไฟล์ Xlsm สำหรับ Java โดยใช้โค้ดสองสามบรรทัด ใช้ GroupDocs Document Signature API เพื่อลงนามรูปแบบไฟล์มากมาย"

############################# Header ############################
title: "เซ็นชื่อไฟล์ Xlsm ด้วยลายเซ็น Text ใน Java"
description: "วิธีเพิ่มลายเซ็น Text ด้วยโค้ด Java สองสามบรรทัด"
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
    title: "เกี่ยวกับ GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) เป็น API ยอดนิยมสำหรับการลงนามในเอกสารดิจิทัลทางอิเล็กทรอนิกส์ ลายเซ็น เช่น ข้อความ รูปภาพ ใบรับรองดิจิทัล บาร์โค้ด รหัส QR ตราประทับ หรือข้อมูลเมตา ลายเซ็นอาจถูกวางไว้บน PDF, เอกสาร MS Word, สมุดงาน MS Excel, การนำเสนอ MS PowerPoint, ไฟล์ Adobe Photoshop และรูปแบบภาพต่างๆ ลูกค้าสามารถลงนามในเอกสารและอัปเดต ค้นหา ตรวจสอบ ลบ หรือดูตัวอย่างลายเซ็นอิเล็กทรอนิกส์ที่ใส่ไว้ในเอกสารเหล่านั้นได้ นอกจากนี้ยังมีความสามารถมากมายสำหรับการปรับแต่งลายเซ็น
    

############################# Steps ############################
steps:
    enable: true
    title_left: "ขั้นตอนในการลงนาม Xlsm กับ Text ใน Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ให้ความสามารถในการลงนามในเอกสาร Xlsm ด้วยลายเซ็น Text อย่างรวดเร็วและง่ายดาย
        
        * สร้างอินสแตนซ์ของคลาส Signature โดยให้ไฟล์ Xlsm ที่ควรเซ็นชื่อเป็นเส้นทางหรือสตรีมหน่วยความจำ
        * สร้างอินสแตนซ์คลาส SignOptions และตั้งค่าข้อมูลที่ต้องการทั้งหมด
        * เรียกใช้เมธอด Signature.Sign() ผ่านไฟล์เอาต์พุต Xlsm หรือสตรีมหน่วยความจำ

    title_right: " ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for Java ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * รับ GroupDocs.Signature for Java ล่าสุดจาก [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsm file
        String filePath = "input.xlsm";
        // Set up output file
        String outputFilePath = "output.xlsm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Xlsm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "การลงนามเอกสาร Xlsm ด้วย Text Live Demo"
    content: |
       ลงชื่อไฟล์ Xlsm ด้วยลายเซ็นต่างๆ ทันทีโดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) สาธิตออนไลน์ฟรีรอคุณอยู่          

############################# More Formats ############################
more_formats:
    enable: true
    title: "ลายเซ็น Text อื่นๆ ที่รองรับสำหรับ Java"
    content: |
        "คุณยังสามารถเซ็นชื่อ Xlsm ด้วยลายเซ็นประเภทอื่นๆ โปรดดูรายการด้านล่าง"
    format: 
       
       
back_to_top:
    enable: true
---