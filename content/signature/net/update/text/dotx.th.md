---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Dotx
productName: .NET
lang: th
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Dotx for C#

############################# Head ############################
head_title: "อัปเดตลายเซ็น Text ที่วางไว้ที่ไฟล์ Dotx ด้วย C#"
head_description: "ใช้โค้ด .NET ที่เข้าใจง่ายและเข้าใจง่ายสำหรับการอัปเดตลายเซ็น Text ในเอกสาร Dotx ที่ลงนามแล้ว"

############################# Header ############################
title: "แก้ไขและอัปเดตลายเซ็น Text ที่วางไว้ที่ Dotx files"
description: "API สำหรับ .NET มีฟังก์ชันสำหรับการอัปเดตลายเซ็น Text ที่เอกสาร Dotx อัปเดตลายเซ็นอิเล็กทรอนิกส์ภายในเอกสาร Dotx ของคุณด้วยโค้ด C# สองสามบรรทัดอย่างรวดเร็วและง่ายดาย"
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
    title: "เรียนรู้เกี่ยวกับ GroupDocs.Signature for .NET คุณลักษณะ API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ฟังก์ชัน API มีวิธีการประมวลผลในรูปแบบเอกสารความต้องการมากมายโดยใช้ลายเซ็นอิเล็กทรอนิกส์ รองรับลายเซ็นอิเล็กทรอนิกส์ เช่น ข้อความ รูปภาพ ใบรับรองดิจิทัล บาร์โค้ด คิวอาร์โค้ด แสตมป์ หรือเมตาดาต้า ลูกค้าสามารถเพิ่ม ลบ แก้ไข ตรวจสอบหรือค้นหาลายเซ็นดิจิทัลได้ที่ PDF, เอกสาร MS Word, สมุดงาน MS Excel, งานนำเสนอ MS PowerPoint, ไฟล์ Adobe Photoshop และรูปแบบภาพต่างๆ มีฟีเจอร์และการตั้งค่าที่มีประโยชน์มากมาย
    

############################# Steps ############################
steps:
    enable: true
    title_left: "วิธีเปลี่ยนลายเซ็น Text ในเอกสาร Dotx ของคุณ"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) มีคุณลักษณะที่เป็นประโยชน์ เช่น การอัปเดตลายเซ็น Text ที่วางไว้ในเอกสาร Dotx ทำให้สามารถเปลี่ยนคุณสมบัติลายเซ็นได้โดยไม่ต้องใช้โค้ดเพิ่มเติม
        
        * ในการเริ่มต้น สร้างวัตถุลายเซ็นที่ส่งผ่านเป็นเส้นทางพารามิเตอร์ตัวสร้างไปยังเอกสารที่ควรได้รับการอัปเดต
        * จากนั้น ให้ยกตัวอย่างอ็อบเจ็กต์ลายเซ็นที่เหมาะสม และตั้งค่าตัวระบุและคุณสมบัติของมันซึ่งจำเป็นต้องเปลี่ยน
        * สุดท้าย เรียกวิธีการอัปเดตของ Signature ผ่านวัตถุลายเซ็นเฉพาะ
        * ดำเนินการอัปเดตผลการแจ้งของคุณ

    title_right: "ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for .NET ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * ดาวน์โหลด GroupDocs.Signature for .NET เวอร์ชันล่าสุดจาก [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotx file
        string filePath = "input.dotx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                TextSignature signatureToUpdate = new TextSignature(id)
                {
                    // specify signature width
                    Width = 130,
                    // specify signature height
                    Height = 20,
                    // set left position
                    Left = 40,
                    // set top position
                    Top = 50,
                    // set up new text
                    Text = "Mr. John Smith"
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "กำลังอัปเดตลายเซ็น Text บนหน้าเอกสาร - Live Demo"
    content: |
       แก้ไขลายเซ็นอิเล็กทรอนิกส์ต่างๆ ของเอกสาร Dotx โดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family)          

############################# More Formats ############################
more_formats:
    enable: true
    title: "อัปเดตลายเซ็น Text ต่างๆ ผ่าน C#"
    content: |
        "การแก้ไขลายเซ็นดิจิทัลที่วางอยู่ในรูปแบบเอกสารต่างๆ อัปเดตข้อมูลลายเซ็นโดยไม่มีรหัสพิเศษ"
    format: 
       
       
back_to_top:
    enable: true
---