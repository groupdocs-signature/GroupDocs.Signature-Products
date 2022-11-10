---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pptx
productName: .NET
lang: th
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pptx for C#

############################# Head ############################
head_title: "การเพิ่มลายเซ็นอิเล็กทรอนิกส์ดิจิทัลลงในไฟล์ Pptx ด้วย C#"
head_description: "ใส่ลายเซ็นดิจิทัลในไฟล์ Pptx สำหรับ .NET โดยใช้โค้ดสองสามบรรทัด ใช้ GroupDocs Document Signature API เพื่อลงนามรูปแบบไฟล์มากมาย"

############################# Header ############################
title: "eSign Pptx ไฟล์ที่มีลายเซ็น Digital ใน C#"
description: "วิธีเพิ่มลายเซ็น Digital ด้วยโค้ด .NET สองสามบรรทัด"
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
    title: "เกี่ยวกับ GroupDocs.Signature for .NET ลายเซ็นดิจิทัล API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) เป็น API ที่ได้รับความนิยมในการกำหนดเอกสารด้วยลายเซ็นอิเล็กทรอนิกส์ดิจิทัล พร้อมใบรับรองดิจิทัล สำหรับลายเซ็นดิจิทัล API ใช้ไฟล์ใบรับรอง PFX เพื่อออกเอกสารด้วยคีย์ส่วนตัวและสาธารณะที่ป้องกันด้วยรหัสผ่าน ลายเซ็นดิจิทัลอาจใช้รับรองเอกสารทางธุรกิจด้วยหน้าเฉพาะ eSign PDF รับรองเอกสาร Microsoft Office ทั้งหมด เช่น Words, Excel, ไฟล์ Powerpoint และเอกสาร Open Office ลูกค้าสามารถจัดการลายเซ็นได้อย่างง่ายดาย เช่น แก้ไข ลบ หรือปรับเปลี่ยน API ให้วิธีการค้นหาและตรวจสอบลายเซ็น นอกจากนี้ยังมีความสามารถมากมายสำหรับการปรับแต่งลายเซ็น
    

############################# Steps ############################
steps:
    enable: true
    title_left: "ขั้นตอนในการลงนาม Pptx กับ Digital ใน C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ให้ความสามารถในการลงนามในเอกสาร Pptx ด้วยลายเซ็น Digital อย่างรวดเร็วและง่ายดาย
        
        * สร้างอินสแตนซ์ของคลาส Signature โดยให้ไฟล์ Pptx ที่ควรเซ็นชื่อเป็นเส้นทางหรือสตรีมหน่วยความจำ
        * สร้างอินสแตนซ์คลาส SignOptions และตั้งค่าข้อมูลที่ต้องการทั้งหมด
        * เรียกใช้เมธอด Signature.Sign() ผ่านไฟล์เอาต์พุต Pptx หรือสตรีมหน่วยความจำ

    title_right: " ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for .NET ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * รับ GroupDocs.Signature for .NET ล่าสุดจาก [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pptx file
        string filePath = "input.pptx";
        // Set up output file
        string outputFilePath = "output.pptx";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Pptx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "การลงนามเอกสาร Pptx ด้วย Digital Live Demo"
    content: |
       ลงชื่อไฟล์ Pptx ด้วยลายเซ็นต่างๆ ทันทีโดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) สาธิตออนไลน์ฟรีรอคุณอยู่          

############################# More Formats ############################
more_formats:
    enable: true
    title: "ลายเซ็น Digital อื่นๆ ที่รองรับสำหรับ C#"
    content: |
        "คุณยังสามารถเซ็นชื่อ Pptx ด้วยลายเซ็นประเภทอื่นๆ โปรดดูรายการด้านล่าง"
    format: 
       
       
back_to_top:
    enable: true
---