---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Ppsx
productName: .NET
lang: fa
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Ppsx for C#

############################# Head ############################
head_title: "افزودن امضاهای Image به فایل Ppsx با C#"
head_description: "با استفاده از چند خط کد، Image Signature را در فایل Ppsx برای .NET قرار دهید. برای امضای ده ها فرمت فایل از GroupDocs Document Signature API استفاده کنید."

############################# Header ############################
title: "امضای فایل‌های Ppsx با امضاهای Image در C#"
description: "نحوه اضافه کردن امضای Image با چند خط کد .NET"
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
    title: "درباره GroupDocs.Signature for .NET API امضاهای تصویر"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) یک API محبوب برای امضای الکترونیکی اسناد دیجیتال است. امضاهایی مانند متون، تصاویر، گواهی‌های دیجیتال، بارکدها، کدهای QR، تمبرها یا ابرداده‌ها در دسترس هستند. امضاها ممکن است روی فایل‌های PDF، اسناد MS Word، کتاب‌های کار MS Excel، ارائه‌های MS PowerPoint، فایل‌های Adobe Photoshop و فرمت‌های تصویر مختلف قرار داده شوند. مشتریان می توانند سند خود را امضا کنند و امضاهای الکترونیکی را که روی آن اسناد قرار داده شده است را به روز کنند، جستجو، تأیید، حذف یا پیش نمایش کنند. علاوه بر این، توانایی های زیادی برای سفارشی سازی امضا ارائه شده است.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "مراحل امضای Ppsx با Image در C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) امکان امضای اسناد Ppsx با امضاهای Image را سریع و آسان فراهم می‌کند.
        
        * یک نمونه از کلاس Signature ایجاد کنید که فایل Ppsx را به عنوان مسیر یا جریان حافظه امضا می کند.
        * کلاس SignOptions را راه اندازی کنید و تمام داده های درخواستی را تنظیم کنید.
        * فراخوانی متد Signature.Sign() برای ارسال خروجی Ppsx فایل یا جریان حافظه

    title_right: " سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for .NET در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * آخرین GroupDocs.Signature for .NET را از [Nuget](https://www.nuget.org/packages/groupdocs.signature) دریافت کنید
         
    code: |
        ```csharp    
                
        // Set up input Ppsx file
        string filePath = "input.ppsx";
        // Set up output file
        string outputFilePath = "output.ppsx";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Ppsx document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "امضای اسناد Ppsx با نسخه نمایشی زنده Image"
    content: |
       با مراجعه به وب‌سایت [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) فایل Ppsx را با امضاهای مختلف در حال حاضر امضا کنید. نسخه ی نمایشی آنلاین رایگان در انتظار شماست.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "سایر امضاهای پشتیبانی شده Image برای C#"
    content: |
        "همچنین می‌توانید Ppsx را با سایر انواع امضا امضا کنید. لطفا لیست زیر را ببینید."
    format: 
       
       
back_to_top:
    enable: true
---