---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Doc
productName: Java
lang: th
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Doc with Java

############################# Head ############################
head_title: "ค้นหาลายเซ็น Qrcode ในไฟล์ Doc ใน Java"
head_description: "ใช้ Java เพื่อค้นหาลายเซ็น Qrcode ในไฟล์ Doc โดยใช้โค้ดสองสามบรรทัด"

############################# Header ############################
title: "ค้นหาลายเซ็น Qrcode ใน Doc file"
description: "API ดั้งเดิมของ Java ช่วยให้ค้นหาลายเซ็น Qrcode ในไฟล์ Doc ที่ลงนามแล้ว ทำการค้นหาลายเซ็นอิเล็กทรอนิกส์ขั้นสูงภายในเอกสาร Doc ของคุณโดยใช้โค้ดสองสามบรรทัด"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "เกี่ยวกับ GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ให้ Java API สำหรับการประมวลผลเอกสารโดยใช้ลายเซ็นประเภทต่างๆ เช่น ข้อความ รูปภาพ ใบรับรองดิจิทัล บาร์โค้ด คิวอาร์โค้ด แสตมป์ หรือเมตาดาต้า ผู้ใช้สามารถเพิ่ม ลบ อัปเดต ตรวจสอบ หรือค้นหาลายเซ็นอิเล็กทรอนิกส์ภายใน PDF, เอกสาร MS Word, เวิร์กบุ๊ก MS Excel, งานนำเสนอ MS PowerPoint, ไฟล์ Adobe Photoshop และรูปแบบรูปภาพต่างๆ พร้อมการสนับสนุนเพิ่มเติมสำหรับการปรับแต่งคุณสมบัติลายเซ็นตามต้องการ
    

############################# Steps ############################
steps:
    enable: true
    title_left: "วิธีค้นหาลายเซ็น Qrcode ใน Doc"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ช่วยให้นักพัฒนา Java ค้นหาลายเซ็น Qrcode ในไฟล์ Doc จากแอปพลิเคชันของตนได้ง่ายขึ้นโดยใช้ขั้นตอนง่ายๆ ไม่กี่ขั้นตอน
        
        * สร้างอินสแตนซ์ใหม่ของคลาส Signature และส่งเส้นทางเอกสารต้นทางเป็นพารามิเตอร์ตัวสร้าง
        * สร้างอินสแตนซ์ออบเจ็กต์ SearchOptions ตามความต้องการของคุณและระบุตัวเลือกการค้นหา
        * วิธีการ Call Search ของอินสแตนซ์คลาส Signature และส่งผ่าน SearchOptions ไป
        * ประมวลผลผลการค้นหาตามความต้องการของคุณ

    title_right: "ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for Java ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * ดาวน์โหลด GroupDocs.Signature for Java เวอร์ชันล่าสุดจาก [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Doc file
        String filePath = "input.doc";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Doc document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "ค้นหา Qrcode ลายเซ็นอิเล็กทรอนิกส์ Live Demo"
    content: |
       ค้นหาเอกสารสำหรับลายเซ็นอิเล็กทรอนิกส์ต่างๆ ของไฟล์ Doc ได้ในขณะนี้โดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family)

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "ค้นหาลายเซ็น Qrcode อื่นๆ โดยใช้ Java"
    content: |
        "ลายเซ็นอิเล็กทรอนิกส์ค้นหาในเอกสารต่างๆ ค้นหาลายเซ็นจากรูปแบบไฟล์ยอดนิยมรูปแบบหนึ่งดังแสดงด้านล่าง"
    format: 
           
       
back_to_top:
    enable: true
---