---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Xls
productName: .NET
lang: th
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Xls for C#

############################# Head ############################
head_title: "สร้างลายเซ็นอิเล็กทรอนิกส์ข้อความไปยังไฟล์ Xls ด้วย C#"
head_description: "ใส่ Text eSignature ในไฟล์ Xls สำหรับ .NET โดยใช้โค้ดสองสามบรรทัด ใช้ GroupDocs Document Signature API เพื่อลงนามรูปแบบไฟล์มากมาย"

############################# Header ############################
title: "เซ็นชื่อไฟล์ Xls ด้วยลายเซ็น Text ใน C#"
description: "วิธีเพิ่มลายเซ็น Text ด้วยโค้ด .NET สองสามบรรทัด"
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
    title: "เกี่ยวกับ GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) เป็น API ยอดนิยมสำหรับการลงนามในเอกสารดิจิทัลทางอิเล็กทรอนิกส์ ลายเซ็น เช่น ข้อความ รูปภาพ ใบรับรองดิจิทัล บาร์โค้ด รหัส QR ตราประทับ หรือข้อมูลเมตา ลายเซ็นอาจถูกวางไว้บน PDF, เอกสาร MS Word, สมุดงาน MS Excel, การนำเสนอ MS PowerPoint, ไฟล์ Adobe Photoshop และรูปแบบภาพต่างๆ ลูกค้าสามารถลงนามในเอกสารและอัปเดต ค้นหา ตรวจสอบ ลบ หรือดูตัวอย่างลายเซ็นอิเล็กทรอนิกส์ที่ใส่ไว้ในเอกสารเหล่านั้นได้ นอกจากนี้ยังมีความสามารถมากมายสำหรับการปรับแต่งลายเซ็น
    

############################# Steps ############################
steps:
    enable: true
    title_left: "ขั้นตอนในการลงนาม Xls กับ Text ใน C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ให้ความสามารถในการลงนามในเอกสาร Xls ด้วยลายเซ็น Text อย่างรวดเร็วและง่ายดาย
        
        * สร้างอินสแตนซ์ของคลาส Signature โดยให้ไฟล์ Xls ที่ควรเซ็นชื่อเป็นเส้นทางหรือสตรีมหน่วยความจำ
        * สร้างอินสแตนซ์คลาส SignOptions และตั้งค่าข้อมูลที่ต้องการทั้งหมด
        * เรียกใช้เมธอด Signature.Sign() ผ่านไฟล์เอาต์พุต Xls หรือสตรีมหน่วยความจำ

    title_right: " ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for .NET ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * รับ GroupDocs.Signature for .NET ล่าสุดจาก [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xls file
        string filePath = "input.xls";
        // Set up output file
        string outputFilePath = "output.xls";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Xls document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "การลงนามเอกสาร Xls ด้วย Text Live Demo"
    content: |
       ลงชื่อไฟล์ Xls ด้วยลายเซ็นต่างๆ ทันทีโดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) สาธิตออนไลน์ฟรีรอคุณอยู่          

############################# More Formats ############################
more_formats:
    enable: true
    title: "ลายเซ็น Text อื่นๆ ที่รองรับสำหรับ C#"
    content: |
        "คุณยังสามารถเซ็นชื่อ Xls ด้วยลายเซ็นประเภทอื่นๆ โปรดดูรายการด้านล่าง"
    format: 
       
       
back_to_top:
    enable: true
---