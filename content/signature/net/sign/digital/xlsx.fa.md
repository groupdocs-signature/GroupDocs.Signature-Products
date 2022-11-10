---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xlsx
productName: .NET
lang: fa
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsx for C#

############################# Head ############################
head_title: "افزودن امضای الکترونیکی دیجیتال به فایل Xlsx با C#"
head_description: "با استفاده از چند خط کد، امضای دیجیتال را روی فایل Xlsx برای .NET قرار دهید. برای امضای ده ها فرمت فایل از GroupDocs Document Signature API استفاده کنید."

############################# Header ############################
title: "eSign فایلهای Xlsx با امضاهای Digital در C#"
description: "نحوه اضافه کردن امضای Digital با چند خط کد .NET"
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
    title: "درباره GroupDocs.Signature for .NET API امضای دیجیتال"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) یک API محبوب برای ثبت اسناد با امضای الکترونیکی دیجیتال، با گواهی‌های دیجیتال است. برای امضای دیجیتال API از فایل های گواهی PFX برای تنظیم سند با کلیدهای خصوصی و عمومی محافظت شده با رمز عبور استفاده می کند. امضاهای دیجیتال ممکن است برای تأیید اسناد تجاری با صفحه خاص eSign PDF، تأیید کل اسناد Microsoft Office مانند Words، Excel، فایل‌های Powerpoint و اسناد Open Office استفاده شوند. مشتریان به راحتی می توانند امضاها را مانند ویرایش، حذف یا تنظیم آن ها دستکاری کنند. API راهی برای جستجو و تأیید امضاها فراهم می کند. علاوه بر این، توانایی های زیادی برای سفارشی سازی امضا ارائه شده است.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "مراحل امضای Xlsx با Digital در C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) امکان امضای اسناد Xlsx با امضاهای Digital را سریع و آسان فراهم می‌کند.
        
        * یک نمونه از کلاس Signature ایجاد کنید که فایل Xlsx را به عنوان مسیر یا جریان حافظه امضا می کند.
        * کلاس SignOptions را راه اندازی کنید و تمام داده های درخواستی را تنظیم کنید.
        * فراخوانی متد Signature.Sign() برای ارسال خروجی Xlsx فایل یا جریان حافظه

    title_right: " سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for .NET در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * آخرین GroupDocs.Signature for .NET را از [Nuget](https://www.nuget.org/packages/groupdocs.signature) دریافت کنید
         
    code: |
        ```csharp    
                
        // Set up input Xlsx file
        string filePath = "input.xlsx";
        // Set up output file
        string outputFilePath = "output.xlsx";
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

                // sign Xlsx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "امضای اسناد Xlsx با نسخه نمایشی زنده Digital"
    content: |
       با مراجعه به وب‌سایت [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) فایل Xlsx را با امضاهای مختلف در حال حاضر امضا کنید. نسخه ی نمایشی آنلاین رایگان در انتظار شماست.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "سایر امضاهای پشتیبانی شده Digital برای C#"
    content: |
        "همچنین می‌توانید Xlsx را با سایر انواع امضا امضا کنید. لطفا لیست زیر را ببینید."
    format: 
       
       
back_to_top:
    enable: true
---