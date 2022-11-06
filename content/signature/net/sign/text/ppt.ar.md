---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Ppt
productName: .NET
lang: ar
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Ppt for C#

############################# Head ############################
head_title: "إنشاء توقيعات إلكترونية نصية إلى ملف Ppt باستخدام C#"
head_description: "ضع Text توقيعًا إلكترونيًا على ملف Ppt لـ .NET باستخدام بضعة أسطر من التعليمات البرمجية. استخدم GroupDocs Document Signature API لتوقيع عشرات تنسيقات الملفات."

############################# Header ############################
title: "توقيع ملفات Ppt بتوقيعات Text في C#"
description: "كيفية إضافة توقيع Text ببضعة أسطر من كود .NET"
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
    title: "حول واجهة برمجة تطبيقات GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) هي واجهة برمجة تطبيقات شائعة للتوقيع الإلكتروني للمستندات الرقمية. التوقيعات مثل النصوص والصور والشهادات الرقمية والباركود ورموز QR والطوابع أو البيانات الوصفية متوفرة. يمكن وضع التوقيعات على ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. يمكن للعملاء التوقيع على مستنداتهم وتحديثها أو البحث عنها أو التحقق منها أو حذفها أو معاينة التوقيعات الإلكترونية التي تم وضعها على تلك المستندات. علاوة على ذلك ، يتم توفير الكثير من القدرات لتخصيص التوقيعات.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "خطوات تسجيل Ppt باستخدام Text في C#"
    content_left: |
        يوفر [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) إمكانية توقيع مستندات Ppt بتوقيعات Text بسرعة وسهولة.
        
        * قم بإنشاء مثيل لفئة التوقيع بتوفير ملف Ppt من المفترض أن يتم توقيعه كمسار أو دفق ذاكرة
        * إنشاء فئة SignOptions وتعيين جميع البيانات المطلوبة.
        * استدعاء أسلوب Signature.Sign () تمرير ملف الإخراج Ppt أو دفق الذاكرة

    title_right: " متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for .NET على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * احصل على أحدث إصدار من GroupDocs.Signature for .NET من [Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ppt file
        string filePath = "input.ppt";
        // Set up output file
        string outputFilePath = "output.ppt";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Ppt document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "توقيع مستندات Ppt باستخدام العرض التوضيحي المباشر Text"
    content: |
       وقّع ملف Ppt بتوقيعات مختلفة الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). عرض تجريبي مجاني على الإنترنت في انتظارك.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "توقيعات Text المدعومة الأخرى لـ C#"
    content: |
        "يمكنك أيضًا توقيع Ppt بأنواع التوقيع الأخرى. يرجى الاطلاع على القائمة أدناه."
    format: 
       
       
back_to_top:
    enable: true
---