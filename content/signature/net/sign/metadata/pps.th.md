---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Pps
productName: .NET
lang: th
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Pps for C#

############################# Head ############################
head_title: "ผนวกลายเซ็นอิเล็กทรอนิกส์ข้อมูลเมตากับเอกสาร Pps ผ่าน C#"
head_description: "ใช้ข้อมูลเมตาเป็นลายเซ็นอิเล็กทรอนิกส์ที่ซ่อนอยู่ในเอกสาร Pps ของคุณโดยใช้โค้ด C# สองสามบรรทัด ใช้ GroupDocs Document Signature API เพื่อลงนามในเอกสารทางธุรกิจและไฟล์ทางอิเล็กทรอนิกส์ด้วยข้อมูลเมตาดาต้า"

############################# Header ############################
title: "ลายเซ็นอิเล็กทรอนิกส์ข้อมูลเมตาสำหรับเอกสาร Pps ผ่าน .NET นั้นง่ายและใช้งานง่าย!"
description: "ลงนามในเอกสาร Pps และสัญญาที่มีรายการ Metadata ที่ซ่อนอยู่ สร้างข้อมูลเมตาสำหรับ PDF, เอกสาร MS Word, สมุดงาน MS Excel, การนำเสนอ MS PowerPoint และรูปแบบภาพต่างๆ โดยไม่มีปัญหาและการเข้ารหัสเพิ่มเติม"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "เกี่ยวกับ API ลายเซ็นข้อมูลเมตาของ GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) เป็น API ยอดนิยมสำหรับการลงนามในเอกสารดิจิทัลทางอิเล็กทรอนิกส์ ลายเซ็น เช่น ข้อความ รูปภาพ ใบรับรองดิจิทัล บาร์โค้ด รหัส QR ตราประทับ หรือข้อมูลเมตา ลายเซ็นอาจถูกวางไว้บน PDF, เอกสาร MS Word, สมุดงาน MS Excel, การนำเสนอ MS PowerPoint, ไฟล์ Adobe Photoshop และรูปแบบภาพต่างๆ ลูกค้าสามารถลงนามในเอกสารและอัปเดต ค้นหา ตรวจสอบ ลบ หรือดูตัวอย่างลายเซ็นอิเล็กทรอนิกส์ที่ใส่ไว้ในเอกสารเหล่านั้นได้ นอกจากนี้ยังมีความสามารถมากมายสำหรับการปรับแต่งลายเซ็น
    

############################# Steps ############################
steps:
    enable: true
    title_left: "ขั้นตอนในการลงนาม Pps กับ Metadata ใน C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ให้ความสามารถในการลงนามในเอกสาร Pps ด้วยลายเซ็น Metadata อย่างรวดเร็วและง่ายดาย
        
        * สร้างอินสแตนซ์ของคลาส Signature โดยให้ไฟล์ Pps ที่ควรเซ็นชื่อเป็นเส้นทางหรือสตรีมหน่วยความจำ
        * สร้างอินสแตนซ์คลาส SignOptions และตั้งค่าข้อมูลที่ต้องการทั้งหมด
        * เรียกใช้เมธอด Signature.Sign() ผ่านไฟล์เอาต์พุต Pps หรือสตรีมหน่วยความจำ

    title_right: " ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for .NET ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * รับ GroupDocs.Signature for .NET ล่าสุดจาก [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Pps file
        string filePath = "input.pps";
        // Set up output file
        string outputFilePath = "output.pps";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Pps document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "การลงนามเอกสาร Pps ด้วย Metadata Live Demo"
    content: |
       ลงชื่อไฟล์ Pps ด้วยลายเซ็นต่างๆ ทันทีโดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) สาธิตออนไลน์ฟรีรอคุณอยู่          

############################# More Formats ############################
more_formats:
    enable: true
    title: "ลายเซ็น Metadata อื่นๆ ที่รองรับสำหรับ C#"
    content: |
        "คุณยังสามารถเซ็นชื่อ Pps ด้วยลายเซ็นประเภทอื่นๆ โปรดดูรายการด้านล่าง"
    format: 
       
       
back_to_top:
    enable: true
---