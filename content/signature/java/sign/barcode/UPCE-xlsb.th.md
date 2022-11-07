---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: UPCE
fileformat: Xlsb
productName: Java
lang: th
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Xlsb for Java

############################# Head ############################
head_title: "eSign Xlsb เอกสารด้วยบาร์โค้ด UPCE ใน Java"
head_description: "สร้าง UPCE Barcode Signature และใส่ลงในเอกสาร Xlsb ด้วย Java โดยใช้โค้ดสองสามบรรทัด ใช้ GroupDocs Document Signature API สำหรับการลงนามรูปแบบไฟล์ต่างๆ"

############################# Header ############################
title: "สร้าง UPCE ลายเซ็นบาร์โค้ดสำหรับเอกสาร Xlsb ใน Java"
description: "eSign เอกสารทางธุรกิจ Xlsb ของคุณด้วยบาร์โค้ด UPCE สร้างลายเซ็นบาร์โค้ดอย่างรวดเร็วและง่ายดายด้วยรหัสสองสามบรรทัดเพื่อตั้งค่าตัวเลือกการเซ็นชื่อ"
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
    title: "เกี่ยวกับ API ลายเซ็นบาร์โค้ด GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) เป็น API ที่ง่ายและรวดเร็วในการจัดการการลงนามเอกสารดิจิทัลโดยใช้ประเภทบาร์โค้ด เช่น UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 และอื่นๆ อีกมากมาย ลูกค้าสามารถสร้างบาร์โค้ดได้อย่างง่ายดายโดยระบุข้อความที่ต้องการและใส่ลงใน PDF, เอกสาร Microsoft Office Words, เวิร์กบุ๊ก Microsoft Office Excel, งานนำเสนอ MS PowerPoint, ไฟล์ Adobe Photoshop และรูปแบบรูปภาพต่างๆ บาร์โค้ดที่อยู่ในเอกสารสามารถอัปเดต ค้นหา ตรวจสอบ ลบ หรือดูตัวอย่างได้ นอกจากนี้ยังรองรับการปรับแต่งบาร์โค้ดอีกด้วย
    

############################# Steps ############################
steps:
    enable: true
    title_left: "ขั้นตอนในการลงนาม Xlsb กับ Barcode ใน Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ให้ความสามารถในการลงนามในเอกสาร Xlsb ด้วยลายเซ็น Barcode อย่างรวดเร็วและง่ายดาย
        
        * สร้างอินสแตนซ์ของคลาส Signature โดยให้ไฟล์ Xlsb ที่ควรเซ็นชื่อเป็นเส้นทางหรือสตรีมหน่วยความจำ
        * สร้างอินสแตนซ์คลาส SignOptions และตั้งค่าข้อมูลที่ต้องการทั้งหมด
        * เรียกใช้เมธอด Signature.Sign() ผ่านไฟล์เอาต์พุต Xlsb หรือสตรีมหน่วยความจำ

    title_right: " ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for Java ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * รับ GroupDocs.Signature for Java ล่าสุดจาก [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";
        // Set up output file
        String outputFilePath = "output.xlsb";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.UPCE);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Xlsb document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "การลงนามเอกสาร Xlsb ด้วย Barcode Live Demo"
    content: |
       ลงชื่อไฟล์ Xlsb ด้วยลายเซ็นต่างๆ ทันทีโดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) สาธิตออนไลน์ฟรีรอคุณอยู่

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About UPCE Barcode"
          content: |
            รหัสสินค้าสากลเป็นสัญลักษณ์บาร์โค้ดที่ใช้กันอย่างแพร่หลายทั่วโลกในการติดตามรายการการค้าในร้านค้า UPCE เป็นรูปแบบ 8 หลักหาก UPC
          characterset: |
             รองรับเฉพาะตัวเลข (0-9)
          textcapacity: |
             ความจุของข้อความ: 7 หลัก + 1 เช็คหลัก
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAEAAAABjCAYAAAArUQZGAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAUTSURBVHhe7ZBBqmQBCAP7/pfuMUwXyMcIkuV7BRK1wIWf78N5H/DLx/I+4JeP5X3ALx/L+oDP57/+m0I9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE548xDeB/zysbwP+OVjefgDvt9/E/iHbcwlZ5QAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "ลายเซ็น Barcode อื่นๆ ที่รองรับสำหรับ Java"
    content: |
        "คุณยังสามารถเซ็นชื่อ Xlsb ด้วยลายเซ็นประเภทอื่นๆ โปรดดูรายการด้านล่าง"
    format: 
        
       
back_to_top:
    enable: true
---