---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Ods
productName: .NET
lang: fa
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Ods for C#

############################# Head ############################
head_title: "امضاهای Image قرار داده شده در فایل های Ods را با C# به روز کنید"
head_description: "از کدهای ساده و آسان برای درک .NET برای به روز رسانی امضاهای Image در اسناد Ods امضا شده استفاده کنید."

############################# Header ############################
title: "امضاهای Image قرار داده شده در فایل های Ods را ویرایش و به روز کنید"
description: "API برای .NET قابلیت به روز رسانی امضاهای Image در اسناد Ods را فراهم می کند. امضاهای الکترونیکی را در اسناد Ods خود با چند خط کد C# سریع و آسان به روز کنید."
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
    title: "درباره ویژگی‌های API GroupDocs.Signature for .NET بیاموزید"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) عملکرد API شامل مجموعه وسیعی از ابزارها برای پردازش در قالب‌های اسناد تقاضا با استفاده از امضای الکترونیکی است. طیف گسترده ای از امضاهای الکترونیکی مانند متون، تصاویر، گواهی های دیجیتال، بارکدها، کدهای QR، تمبرها یا ابرداده ها پشتیبانی می شوند. مشتریان می‌توانند امضاهای دیجیتال را در فایل‌های PDF، اسناد MS Word، کتاب‌های کار MS Excel، ارائه‌های MS PowerPoint، فایل‌های Adobe Photoshop و فرمت‌های تصویری مختلف اضافه، حذف، ویرایش، اعتبارسنجی یا جستجو کنند. ویژگی ها و تنظیمات مفید متعددی در دسترس است.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "نحوه تغییر امضاهای Image در سند Ods"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) شامل ویژگی‌های مفیدی مانند به‌روزرسانی امضاهای Image قرار گرفته در اسناد Ods است. این امکان تغییر ویژگی های امضا را بدون کد اضافی فراهم می کند.
        
        * برای شروع، شی Signature را ایجاد کنید که به عنوان یک مسیر پارامتر سازنده به سندی که قرار است به روز شود، منتقل می شود.
        * سپس، یک شی امضای خاص را نمونه‌سازی کنید و شناسه و ویژگی‌های آن را که نیاز به تغییر دارند تنظیم کنید.
        * در نهایت، متد Signature's Update را فراخوانی کنید که یک شیء امضای خاص را ارسال می کند.
        * به روز رسانی نتایج را طبق اطلاعیه خود پردازش کنید.

    title_right: "سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for .NET در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * آخرین نسخه GroupDocs.Signature for .NET را از [Nuget](https://www.nuget.org/packages/groupdocs.signature) دانلود کنید
         
    code: |
        ```csharp    
                
        // Set up input Ods file
        string filePath = "input.ods";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                ImageSignature signatureToUpdate = new ImageSignature(id)
                {
                    // specify signature width
                    Width = 170,
                    // specify signature height
                    Height = 250,
                    // set left position
                    Left = 10,
                    // set top position
                    Top = 10
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
    title: "به روز رسانی امضاهای Image در صفحات سند - نسخه نمایشی زنده"
    content: |
       اکنون با مراجعه به وب‌سایت [GroupDocs.Signature App](https://products.groupdocs.app/signature/family)، امضاهای الکترونیکی مختلف سند Ods را ویرایش کنید.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "امضاهای مختلف Image را از طریق C# به روز کنید"
    content: |
        "ویرایش امضاهای دیجیتال که در قالب های مختلف اسناد قرار می گیرند. به روز رسانی داده های امضا بدون کد اضافی."
    format: 
       
       
back_to_top:
    enable: true
---