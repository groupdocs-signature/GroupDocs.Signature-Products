---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Pptx
productName: .NET
lang: fa
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Pptx for C#

############################# Head ############################
head_title: "حذف امضاهای Qrcode از فایل‌های Pptx از طریق C#"
head_description: "حذف امضاهای خاص Qrcode از اسناد امضا شده Pptx ممکن است به راحتی با کد کوتاه .NET انجام شود."

############################# Header ############################
title: "حذف Qrcode امضاهایی که در فایل‌های Pptx قرار گرفته‌اند."
description: "امضاهای مختلف Qrcode را از اسناد Pptx حذف کنید. حذف امضاهای Qrcode به کد C# ساده نیاز دارد."
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
    title: "اطلاعاتی درباره ویژگی‌های API GroupDocs.Signature for .NET دریافت کنید"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API راه های زیادی برای پردازش اسناد شما با استفاده از امضای الکترونیکی ارائه می دهد. امضاهای دیجیتال مانند متون، تصاویر، گواهی های دیجیتال، بارکدها، کدهای QR، تمبر یا ابرداده در دسترس هستند. مشتریان امکان افزودن، حذف، به روز رسانی، تأیید یا جستجوی امضاهای دیجیتال را در فایل های PDF، اسناد MS Word، کتاب های کار MS Excel، ارائه های MS PowerPoint، فایل های Adobe Photoshop و فرمت های تصویری مختلف دارند. تعداد زیادی از ویژگی ها و تنظیمات مفید ارائه شده است.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "نحوه حذف امضاهای Qrcode از سند Pptx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ویژگی مفیدی را برای پاک کردن اسناد Pptx از امضاهای Qrcode با چند خط کد ارائه می‌کند.
        
        * ابتدا، مسیر عبور شی Signature به سند خود را به عنوان پارامتر سازنده نمونه سازی کنید.
        * سپس، یک شی امضای مناسب ایجاد کنید و شناسه منحصر به فرد آن را تنظیم کنید.
        * پس از آن، متد Delete را فراخوانی کنید که شی امضا را ارسال می کند که باید حذف شود.
        * در نهایت، نتایج عملیات را پردازش کنید.

    title_right: "سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for .NET در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * آخرین نسخه GroupDocs.Signature for .NET را از [Nuget](https://www.nuget.org/packages/groupdocs.signature) دانلود کنید
         
    code: |
        ```csharp    
                
        // Set up input Pptx file
        string filePath = "input.pptx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to delete
                // set up particular signature id
                QrCodeSignature signatureToDelete = new QrCodeSignature(id);

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
    title: "امضا کردن با امضاهای Qrcode نمایش زنده"
    content: |
       با مراجعه به وب‌سایت [GroupDocs.Signature App](https://products.groupdocs.app/signature/family)، همین حالا امضاهای الکترونیکی مختلف را به فایل Pptx اضافه کنید.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "امضاهای Qrcode خود را با C# حذف کنید"
    content: |
        "حذف امضاهای الکترونیکی که به فرمت های مختلف اسناد اضافه شده اند. امضاها را به سرعت بدون کد اضافی حذف کنید."
    format: 
       
       
back_to_top:
    enable: true
---