---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Potx
productName: .NET
lang: th
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Potx for C#

############################# Head ############################
head_title: "ลบลายเซ็น Text จากไฟล์ Potx ผ่าน C#"
head_description: "การลบลายเซ็น Text เฉพาะจากเอกสาร Potx ที่ลงนามแล้วอาจทำได้ง่ายๆ ด้วยรหัส .NET แบบสั้น"

############################# Header ############################
title: "ลบลายเซ็น Text ที่อยู่ใน Potx files"
description: "ลบลายเซ็น Text ต่างๆ จากเอกสาร Potx การลบลายเซ็น Text ต้องใช้โค้ด C# อย่างง่าย"
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
    title: "รับข้อมูลเกี่ยวกับคุณสมบัติ API ของ GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API มีหลายวิธีในการประมวลผลเอกสารของคุณโดยใช้ลายเซ็นอิเล็กทรอนิกส์ ลายเซ็นดิจิทัล เช่น ข้อความ รูปภาพ ใบรับรองดิจิทัล บาร์โค้ด คิวอาร์โค้ด แสตมป์ หรือข้อมูลเมตา ลูกค้าสามารถเพิ่ม ลบ อัปเดต ตรวจสอบหรือค้นหาลายเซ็นดิจิทัลได้ที่ PDF, เอกสาร MS Word, สมุดงาน MS Excel, งานนำเสนอ MS PowerPoint, ไฟล์ Adobe Photoshop และรูปแบบรูปภาพต่างๆ มีคุณลักษณะและการตั้งค่าที่เป็นประโยชน์มากมาย
    

############################# Steps ############################
steps:
    enable: true
    title_left: "วิธีลบลายเซ็น Text ออกจากเอกสาร Potx ของคุณ"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) มีคุณลักษณะที่เป็นประโยชน์สำหรับการล้างเอกสาร Potx ของ Text ลายเซ็นด้วยโค้ดไม่กี่บรรทัด
        
        * ขั้นแรก ยกตัวอย่างวัตถุ Signature ที่ส่งพาธไปยังเอกสารของคุณเป็นพารามิเตอร์ Constructor
        * จากนั้นสร้างวัตถุลายเซ็นที่เหมาะสมและตั้งค่าตัวระบุที่ไม่ซ้ำกัน
        * หลังจากนั้นให้เรียกใช้เมธอด Delete ผ่านวัตถุลายเซ็นซึ่งต้องถูกลบ
        * สุดท้าย ประมวลผลผลการดำเนินการ

    title_right: "ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for .NET ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * ดาวน์โหลด GroupDocs.Signature for .NET เวอร์ชันล่าสุดจาก [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Potx file
        string filePath = "input.potx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to delete
                // set up particular signature id
                TextSignature signatureToDelete = new TextSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "การลงนามด้วยลายเซ็น Text การสาธิตสด"
    content: |
       เพิ่มลายเซ็นอิเล็กทรอนิกส์ต่างๆ ลงในไฟล์ Potx โดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family)          

############################# More Formats ############################
more_formats:
    enable: true
    title: "ลบลายเซ็น Text ของคุณด้วย C#"
    content: |
        "การลบลายเซ็นอิเล็กทรอนิกส์ที่เพิ่มลงในรูปแบบเอกสารต่างๆ ลบลายเซ็นอย่างรวดเร็วโดยไม่ต้องใช้รหัสพิเศษ"
    format: 
       
       
back_to_top:
    enable: true
---