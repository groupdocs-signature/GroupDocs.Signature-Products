---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: UPCE
fileformat: Ppsx
productName: .NET
lang: ar
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ppsx for C#

############################# Head ############################
head_title: "وثيقة eSign Ppsx مع UPCE رمز شريطي في C#"
head_description: "أنشئ UPCE Barcode Signature وضعه في مستند Ppsx باستخدام .NET باستخدام سطرين من الشفرة. استخدم GroupDocs Document Signature API لتوقيع تنسيقات ملفات متنوعة."

############################# Header ############################
title: "إنشاء UPCE توقيع الرمز الشريطي للمستند Ppsx في C#"
description: "قم بتوقيع Ppsx على مستندات الأعمال باستخدام الرمز الشريطي UPCE. قم بإنشاء توقيع الرمز الشريطي بسرعة وسهولة باستخدام بضعة أسطر من التعليمات البرمجية لإعداد خيارات التوقيع."
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
    title: "حول GroupDocs.Signature for .NET واجهة برمجة تطبيقات تواقيع الرموز الشريطية."
    content: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) هي واجهة برمجة تطبيقات سريعة وسهلة لإدارة التوقيع الإلكتروني للمستندات الرقمية باستخدام أنواع الرموز الشريطية مثل UPCA و UPCE و EAN13 و EAN14 و Code39 و Code39Extended و Code128 و Codabar و Postnet و ISBN و ITF14 وغيرها الكثير. يمكن للعملاء إنشاء رموز شريطية بسهولة لتوفير النص المطلوب ووضعها على PDF ومستندات Microsoft Office Words ومصنفات Microsoft Office Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. يمكن تحديث الرموز الشريطية الموضوعة في المستندات أو البحث فيها أو التحقق منها أو حذفها أو معاينتها. علاوة على ذلك ، يتم دعم تخصيص الباركود.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "خطوات تسجيل Ppsx باستخدام Barcode في C#"
    content_left: |
        يوفر [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) إمكانية توقيع مستندات Ppsx بتوقيعات Barcode بسرعة وسهولة.
        
        * قم بإنشاء مثيل لفئة التوقيع بتوفير ملف Ppsx من المفترض أن يتم توقيعه كمسار أو دفق ذاكرة
        * إنشاء فئة SignOptions وتعيين جميع البيانات المطلوبة.
        * استدعاء أسلوب Signature.Sign () تمرير ملف الإخراج Ppsx أو دفق الذاكرة

    title_right: " متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for .NET على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * احصل على أحدث إصدار من GroupDocs.Signature for .NET من [Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ppsx file
        string filePath = "input.ppsx";
        // Set up output file
        string outputFilePath = "output.ppsx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.UPCE,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Ppsx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "توقيع مستندات Ppsx باستخدام العرض التوضيحي المباشر Barcode"
    content: |
       وقّع ملف Ppsx بتوقيعات مختلفة الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). عرض تجريبي مجاني على الإنترنت في انتظارك.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About UPCE Barcode"
          content: |
            رمز المنتج العالمي هو رمز شريطي يُستخدم على نطاق واسع في جميع أنحاء العالم لتتبع العناصر التجارية في المتاجر. UPCE هو تباين مكون من 8 أرقام إذا كان UPC.
          characterset: |
             يدعم فقط الأرقام الرقمية (0-9).
          textcapacity: |
             سعة النص البرمجي: 7 أرقام بالضبط + 1 خانة تحقق.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAEAAAABjCAYAAAArUQZGAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAUTSURBVHhe7ZBBqmQBCAP7/pfuMUwXyMcIkuV7BRK1wIWf78N5H/DLx/I+4JeP5X3ALx/L+oDP57/+m0I9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE54U2yH1FPMcHHQd6lzOeFNsR1STzHDxUHfpc7lhDfFdkg9xQwXB32XOpcT3hTbIfUUM1wc9F3qXE548xDeB/zysbwP+OVjefgDvt9/E/iHbcwlZ5QAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "توقيعات Barcode المدعومة الأخرى لـ C#"
    content: |
        "يمكنك أيضًا توقيع Ppsx بأنواع التوقيع الأخرى. يرجى الاطلاع على القائمة أدناه."
    format: 
        
       
back_to_top:
    enable: true
---