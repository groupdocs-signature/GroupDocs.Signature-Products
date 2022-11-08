---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xltx
productName: .NET
lang: fa
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xltx for C#

############################# Head ############################
head_title: "از طریق C# امضاهای الکترونیکی فراداده را به اسناد Xltx اضافه کنید"
head_description: "با استفاده از چند خط کد C# از فراداده به عنوان امضای الکترونیکی پنهان در اسناد Xltx خود استفاده کنید. از GroupDocs Document Signature API برای امضای الکترونیکی اسناد و فایل‌های تجاری خود با اطلاعات فراداده استفاده کنید."

############################# Header ############################
title: "امضاهای الکترونیکی فراداده برای سند Xltx از طریق .NET ساده و آسان برای استفاده هستند!"
description: "اسناد و قراردادهای Xltx خود را با ورودی‌های فراداده پنهان امضا کنید. فراداده برای فایل‌های PDF، اسناد MS Word، کتاب‌های کار MS Excel، ارائه‌های MS PowerPoint و فرمت‌های تصویری مختلف بدون مشکل و کدنویسی اضافی ایجاد کنید."
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
    title: "درباره GroupDocs.Signature for .NET API امضاهای فراداده"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) یک API محبوب برای امضای الکترونیکی اسناد دیجیتال است. امضاهایی مانند متون، تصاویر، گواهی‌های دیجیتال، بارکدها، کدهای QR، تمبرها یا ابرداده‌ها در دسترس هستند. امضاها ممکن است روی فایل‌های PDF، اسناد MS Word، کتاب‌های کار MS Excel، ارائه‌های MS PowerPoint، فایل‌های Adobe Photoshop و فرمت‌های تصویر مختلف قرار داده شوند. مشتریان می توانند سند خود را امضا کنند و امضاهای الکترونیکی را که روی آن اسناد قرار داده شده است را به روز کنند، جستجو، تأیید، حذف یا پیش نمایش کنند. علاوه بر این، توانایی های زیادی برای سفارشی سازی امضا ارائه شده است.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "مراحل امضای Xltx با Metadata در C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) امکان امضای اسناد Xltx با امضاهای Metadata را سریع و آسان فراهم می‌کند.
        
        * یک نمونه از کلاس Signature ایجاد کنید که فایل Xltx را به عنوان مسیر یا جریان حافظه امضا می کند.
        * کلاس SignOptions را راه اندازی کنید و تمام داده های درخواستی را تنظیم کنید.
        * فراخوانی متد Signature.Sign() برای ارسال خروجی Xltx فایل یا جریان حافظه

    title_right: " سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for .NET در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * آخرین GroupDocs.Signature for .NET را از [Nuget](https://www.nuget.org/packages/groupdocs.signature) دریافت کنید
         
    code: |
        ```csharp    
        
        // Set up input Xltx file
        string filePath = "input.xltx";
        // Set up output file
        string outputFilePath = "output.xltx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Xltx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "امضای اسناد Xltx با نسخه نمایشی زنده Metadata"
    content: |
       با مراجعه به وب‌سایت [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) فایل Xltx را با امضاهای مختلف در حال حاضر امضا کنید. نسخه ی نمایشی آنلاین رایگان در انتظار شماست.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "سایر امضاهای پشتیبانی شده Metadata برای C#"
    content: |
        "همچنین می‌توانید Xltx را با سایر انواع امضا امضا کنید. لطفا لیست زیر را ببینید."
    format: 
       
       
back_to_top:
    enable: true
---