---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Doc
productName: .NET
lang: th
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for C#

############################# Head ############################
head_title: "การตรวจสอบลายเซ็น Digital สำหรับไฟล์ Doc ผ่าน C#"
head_description: "ใช้โค้ด .NET เพียงไม่กี่บรรทัดเพื่อยืนยันเอกสาร Doc และลายเซ็น Digital"

############################# Header ############################
title: "Digital การตรวจสอบลายเซ็นสำหรับไฟล์ Doc"
description: "API สำหรับ .NET ให้โอกาสในการตรวจสอบลายเซ็น Digital ที่เอกสาร Doc การยืนยันลายเซ็นอิเล็กทรอนิกส์ภายในเอกสาร Doc ของคุณอาจดำเนินการได้อย่างรวดเร็วและง่ายดาย"
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
    title: "ค้นพบคุณสมบัติ API ใหม่ของ GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API มีวิธีมากมายในการประมวลผลเอกสารรูปแบบต่างๆ โดยใช้ลายเซ็นอิเล็กทรอนิกส์ รองรับลายเซ็นดิจิทัลหลายประเภท เช่น ข้อความ รูปภาพ ใบรับรองดิจิทัล บาร์โค้ด คิวอาร์โค้ด แสตมป์ หรือเมตาดาต้า ลูกค้าสามารถเพิ่ม ลบ แก้ไข ตรวจสอบหรือค้นหาลายเซ็นดิจิทัลได้ที่ PDF, เอกสาร MS Word, สมุดงาน MS Excel, งานนำเสนอ MS PowerPoint, ไฟล์ Adobe Photoshop และรูปแบบภาพต่างๆ มีฟีเจอร์และการตั้งค่าเพิ่มเติมมากมายที่น่าอัศจรรย์
    

############################# Steps ############################
steps:
    enable: true
    title_left: "วิธีตรวจสอบลายเซ็น Digital ในเอกสาร Doc ของคุณ"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) มีคุณลักษณะที่เป็นประโยชน์ เช่น การตรวจสอบลายเซ็น Digital ที่วางไว้ในเอกสาร Doc ใช้โอกาสนี้โดยไม่ต้องติดตั้งโค้ดเพิ่มเติม
        
        * ประการแรก สร้างอินสแตนซ์คลาส Signature ให้เป็นพาธพารามิเตอร์ Constructor ไปยังเอกสารที่ควรได้รับการตรวจสอบ
        * ประการที่สอง สร้างวัตถุ VerifyOptions ใหม่และตั้งค่าคุณสมบัติที่จำเป็นทั้งหมด
        * สุดท้าย เรียกใช้เมธอด Verify วัตถุของ Signature ผ่านอินสแตนซ์ VerifyOptions
        * จากนั้นประมวลผลผลการตรวจสอบ

    title_right: "ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for .NET ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * ดาวน์โหลด GroupDocs.Signature for .NET เวอร์ชันล่าสุดจาก [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                DigitalVerifyOptions options = new DigitalVerifyOptions()
                {
                    // Digital signature comment
                    Comments = "Approved by co-owner",
                    // specify period of signatures
                    SignDateTimeFrom = new DateTime(year: 2021, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2022, month: 12, day: 31)
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "การลงนามด้วยลายเซ็น Digital การสาธิตสด"
    content: |
       เพิ่มลายเซ็นอิเล็กทรอนิกส์ต่างๆ ลงในไฟล์ Doc โดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family)          

############################# More Formats ############################
more_formats:
    enable: true
    title: "ตรวจสอบลายเซ็น Digital อื่นๆ โดยใช้ C#"
    content: |
        "การตรวจสอบลายเซ็นอิเล็กทรอนิกส์ที่อยู่ในเอกสารต่างๆ ตรวจสอบคุณภาพของลายเซ็นในรูปแบบไฟล์ยอดนิยมดังที่แสดงด้านล่าง"
    format: 
       
       
back_to_top:
    enable: true
---