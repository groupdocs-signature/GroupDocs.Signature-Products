---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Doc
productName: .NET
lang: fa
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Doc for C#

############################# Head ############################
head_title: "تأیید امضاهای Qrcode برای فایل های Doc از طریق C#"
head_description: "فقط از چند خط کد .NET برای تأیید اسناد Doc و امضاهای Qrcode آنها استفاده کنید."

############################# Header ############################
title: "تأیید امضاهای Qrcode برای فایل‌های Doc"
description: "API برای .NET فرصتی برای تأیید امضاهای Qrcode در اسناد Doc فراهم می‌کند. تأیید امضاهای الکترونیکی در اسناد Doc شما ممکن است به سرعت و به راحتی انجام شود."
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
    title: "ویژگی‌های جدید API GroupDocs.Signature for .NET را کشف کنید"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API طیف وسیعی از راه‌ها را برای پردازش قالب‌های اسناد متعدد با استفاده از امضای الکترونیکی ارائه می‌کند. بسیاری از انواع امضاهای دیجیتال مانند متون، تصاویر، گواهی های دیجیتال، بارکدها، کدهای QR، تمبرها یا ابرداده ها پشتیبانی می شوند. مشتریان می‌توانند امضاهای دیجیتال را در فایل‌های PDF، اسناد MS Word، کتاب‌های کار MS Excel، ارائه‌های MS PowerPoint، فایل‌های Adobe Photoshop و فرمت‌های تصویری مختلف اضافه، حذف، ویرایش، اعتبارسنجی یا جستجو کنند. تعداد شگفت انگیزی از ویژگی ها و تنظیمات اضافی در دسترس است.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "نحوه تأیید اعتبار امضاهای Qrcode در سند Doc"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) شامل ویژگی‌های مفیدی مانند تأیید امضاهای Qrcode قرار گرفته در اسناد Doc است. از این فرصت بدون پیاده سازی کد اضافی استفاده کنید.
        
        * ابتدا، کلاس Signature را به عنوان یک مسیر پارامتر سازنده به سندی که قرار است تأیید شود، ارائه دهید.
        * در مرحله دوم، یک شی VerifyOptions جدید ایجاد کنید و تمام ویژگی های مورد نیاز را تنظیم کنید.
        * در نهایت، شیء Signature's Verify را با عبور از نمونه VerifyOptions فراخوانی کنید.
        * سپس نتایج تأیید را پردازش کنید.

    title_right: "سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for .NET در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * آخرین نسخه GroupDocs.Signature for .NET را از [Nuget](https://www.nuget.org/packages/groupdocs.signature) دانلود کنید
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
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
    title: "امضا کردن با امضاهای Qrcode نمایش زنده"
    content: |
       با مراجعه به وب‌سایت [GroupDocs.Signature App](https://products.groupdocs.app/signature/family)، همین حالا امضاهای الکترونیکی مختلف را به فایل Doc اضافه کنید.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "تأیید سایر امضاهای Qrcode با استفاده از C#"
    content: |
        "تأیید امضای الکترونیکی در اسناد مختلف. همانطور که در زیر نشان داده شده است، کیفیت امضاها را در قالب‌های فایل محبوب بررسی کنید."
    format: 
       
       
back_to_top:
    enable: true
---