---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Pptm
productName: .NET
lang: th
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Pptm with C#

############################# Head ############################
head_title: "ค้นหาลายเซ็น Text ในไฟล์ Pptm ใน C#"
head_description: "ใช้ .NET เพื่อค้นหาลายเซ็น Text ในไฟล์ Pptm โดยใช้โค้ดสองสามบรรทัด"

############################# Header ############################
title: "ค้นหาลายเซ็น Text ใน Pptm file"
description: "API ดั้งเดิมของ .NET ช่วยให้ค้นหาลายเซ็น Text ในไฟล์ Pptm ที่ลงนามแล้ว ทำการค้นหาลายเซ็นอิเล็กทรอนิกส์ขั้นสูงภายในเอกสาร Pptm ของคุณโดยใช้โค้ดสองสามบรรทัด"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "เกี่ยวกับ GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ให้ .NET API สำหรับการประมวลผลเอกสารโดยใช้ลายเซ็นประเภทต่างๆ เช่น ข้อความ รูปภาพ ใบรับรองดิจิทัล บาร์โค้ด คิวอาร์โค้ด แสตมป์ หรือเมตาดาต้า ผู้ใช้สามารถเพิ่ม ลบ อัปเดต ตรวจสอบ หรือค้นหาลายเซ็นอิเล็กทรอนิกส์ภายใน PDF, เอกสาร MS Word, เวิร์กบุ๊ก MS Excel, งานนำเสนอ MS PowerPoint, ไฟล์ Adobe Photoshop และรูปแบบรูปภาพต่างๆ พร้อมการสนับสนุนเพิ่มเติมสำหรับการปรับแต่งคุณสมบัติลายเซ็นตามต้องการ
    

############################# Steps ############################
steps:
    enable: true
    title_left: "วิธีค้นหาลายเซ็น Text ใน Pptm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ช่วยให้นักพัฒนา .NET ค้นหาลายเซ็น Text ในไฟล์ Pptm จากแอปพลิเคชันของตนได้ง่ายขึ้นโดยใช้ขั้นตอนง่ายๆ ไม่กี่ขั้นตอน
        
        * สร้างอินสแตนซ์ใหม่ของคลาส Signature และส่งเส้นทางเอกสารต้นทางเป็นพารามิเตอร์ตัวสร้าง
        * สร้างอินสแตนซ์ออบเจ็กต์ SearchOptions ตามความต้องการของคุณและระบุตัวเลือกการค้นหา
        * วิธีการ Call Search ของอินสแตนซ์คลาส Signature และส่งผ่าน SearchOptions ไป
        * ประมวลผลผลการค้นหาตามความต้องการของคุณ

    title_right: "ความต้องการของระบบ"
    content_right: |
        GroupDocs.Signature for .NET ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบให้แน่ใจว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ไว้ในระบบของคุณแล้ว

        * ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        * สภาพแวดล้อมการพัฒนา: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * ดาวน์โหลด GroupDocs.Signature for .NET เวอร์ชันล่าสุดจาก [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pptm file
        string filePath = "input.pptm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                TextSearchOptions options = new TextSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // specify text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature"
                };

                // search for Text signatures in Pptm document
                List<TextSignature> signatures = signature.Search<TextSignature>(options);

                // process signatures which were found                
                foreach (TextSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "ค้นหา Text ลายเซ็นอิเล็กทรอนิกส์ Live Demo"
    content: |
       ค้นหาเอกสารสำหรับลายเซ็นอิเล็กทรอนิกส์ต่างๆ ของไฟล์ Pptm ได้ในขณะนี้โดยไปที่เว็บไซต์ [GroupDocs.Signature App](https://products.groupdocs.app/signature/family)

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "ค้นหาลายเซ็น Text อื่นๆ โดยใช้ C#"
    content: |
        "ลายเซ็นอิเล็กทรอนิกส์ค้นหาในเอกสารต่างๆ ค้นหาลายเซ็นจากรูปแบบไฟล์ยอดนิยมรูปแบบหนึ่งดังแสดงด้านล่าง"
    format: 
           
       
back_to_top:
    enable: true
---