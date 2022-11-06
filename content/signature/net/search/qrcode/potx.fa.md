---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Potx
productName: .NET
lang: fa
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Potx with C#

############################# Head ############################
head_title: "جستجوی امضاهای Qrcode در فایل Potx در C#"
head_description: "از .NET برای جستجوی امضاهای Qrcode در فایل های Potx با استفاده از چند خط کد استفاده کنید."

############################# Header ############################
title: "امضاهای Qrcode را در فایل Potx جستجو کنید"
description: "API بومی .NET امکان جستجوی امضاهای Qrcode را در فایل‌های Potx از قبل امضا شده می‌دهد. با استفاده از چند خط کد، جستجوی پیشرفته امضای الکترونیکی را در اسناد Potx خود انجام دهید."
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
    title: "درباره GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API .NET را برای پردازش اسناد با استفاده از انواع مختلف امضا مانند متون، تصاویر، گواهی‌های دیجیتال، بارکد، کدهای QR، تمبر یا ابرداده ارائه می‌کند. کاربران می‌توانند امضاهای الکترونیکی را در فایل‌های PDF، اسناد MS Word، کتاب‌های کار MS Excel، ارائه‌های MS PowerPoint، فایل‌های Adobe Photoshop و فرمت‌های تصویر مختلف با پشتیبانی اضافی برای سفارشی‌سازی ویژگی‌های امضا در صورت لزوم اضافه، حذف، به‌روزرسانی، تأیید یا جستجو کنند.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "نحوه جستجوی امضاهای Qrcode در Potx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) با اجرای چند مرحله آسان، جستجوی امضاهای Qrcode در فایل‌های Potx را برای توسعه‌دهندگان .NET آسان‌تر می‌کند.
        
        * یک نمونه جدید از کلاس Signature ایجاد کنید و مسیر سند منبع را به عنوان پارامتر سازنده ارسال کنید.
        * شی SearchOptions را مطابق با نیاز خود نمونه سازی کنید و گزینه های جستجو را مشخص کنید.
        * متد Search نمونه کلاس Signature را فراخوانی کنید و SearchOptions را به آن ارسال کنید.
        * نتایج جستجو را بر اساس خواسته های خود پردازش کنید.

    title_right: "سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for .NET در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * آخرین نسخه GroupDocs.Signature for .NET را از [Nuget](https://www.nuget.org/packages/groupdocs.signature) دانلود کنید
         
    code: |
        ```csharp    
                
        // Set up input Potx file
        string filePath = "input.potx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                QrCodeSearchOptions options = new QrCodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Qrcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Qrcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Qrcode signatures in Potx document
                List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

                // process signatures which were found                
                foreach (QrCodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Qrcode امضای الکترونیکی نسخه نمایشی زنده را جستجو کنید"
    content: |
       اکنون با مراجعه به وب‌سایت [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family)، سند را برای امضاهای الکترونیکی مختلف در فایل‌های Potx جستجو کنید.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "جستجوی امضاهای دیگر Qrcode با استفاده از C#"
    content: |
        "جستجوی امضای الکترونیکی در اسناد مختلف. همانطور که در زیر نشان داده شده است، امضاها را از یکی از فرمت های فایل محبوب پیدا کنید."
    format: 
           
       
back_to_top:
    enable: true
---