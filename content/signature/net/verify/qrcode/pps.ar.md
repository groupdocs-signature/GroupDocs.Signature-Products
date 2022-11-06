---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Pps
productName: .NET
lang: ar
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Pps for C#

############################# Head ############################
head_title: "التحقق من توقيعات Qrcode لملفات Pps عبر C#"
head_description: "استخدم فقط بضعة أسطر من كود .NET للتحقق من مستندات Pps وتوقيعاتها Qrcode."

############################# Header ############################
title: "التحقق من صحة التوقيعات Qrcode لملفات Pps"
description: "توفر واجهة برمجة التطبيقات لـ .NET فرصة للتحقق من توقيعات Qrcode في مستندات Pps. قد يتم التحقق من صحة التوقيعات الإلكترونية داخل مستندات Pps بسرعة وسهولة."
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
    title: "اكتشف ميزات واجهة برمجة تطبيقات GroupDocs.Signature for .NET الجديدة"
    content: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) توفر واجهة برمجة التطبيقات مجموعة واسعة من الطرق لمعالجة العديد من تنسيقات المستندات باستخدام التوقيعات الإلكترونية. يتم دعم العديد من أنواع التوقيعات الرقمية مثل النصوص أو الصور أو الشهادات الرقمية أو الرموز الشريطية أو رموز QR أو الطوابع أو البيانات الوصفية. يمكن للعملاء إضافة أو إزالة أو تحرير أو التحقق من صحة أو البحث عن التوقيعات الرقمية في ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. يتوفر عدد مذهل من الميزات والإعدادات الإضافية.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "كيفية التحقق من صحة توقيعات Qrcode في مستندك Pps"
    content_left: |
        يتضمن [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) ميزات مفيدة مثل التحقق من التوقيعات Qrcode الموضوعة في مستندات Pps. اغتنم هذه الفرصة دون تنفيذ كود إضافي.
        
        * أولاً ، قم بإنشاء مثيل لفئة التوقيع التي توفر كمسار معلمة منشئ لمستند من المفترض أن يتم التحقق منه.
        * ثانيًا ، قم بإنشاء كائن VerifyOptions جديد وقم بإعداد جميع الخصائص المطلوبة.
        * أخيرًا ، استدعاء طريقة التحقق من كائن Signature لتمرير مثيل VerifyOptions.
        * ثم معالجة نتائج التحقق.

    title_right: "متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for .NET على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * تنزيل أحدث إصدار من GroupDocs.Signature for .NET من [Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pps file
        string filePath = "input.pps";

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
    title: "التوقيع باستخدام توقيعات Qrcode Live Demo"
    content: |
       أضف توقيعات إلكترونية متنوعة إلى ملف Pps الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "تحقق من توقيعات Qrcode الأخرى باستخدام C#"
    content: |
        "التحقق من صحة التوقيعات الإلكترونية الموضوعة في مستندات مختلفة. تحقق من جودة التوقيعات بتنسيقات الملفات الشائعة كما هو موضح أدناه."
    format: 
       
       
back_to_top:
    enable: true
---