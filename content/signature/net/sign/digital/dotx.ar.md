---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dotx
productName: .NET
lang: ar
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dotx for C#

############################# Head ############################
head_title: "إضافة التوقيعات الإلكترونية الرقمية إلى ملف Dotx باستخدام C#"
head_description: "ضع التوقيع الرقمي على ملف Dotx لـ .NET باستخدام بضعة أسطر من التعليمات البرمجية. استخدم GroupDocs Document Signature API لتوقيع عشرات تنسيقات الملفات."

############################# Header ############################
title: "ملفات eSign Dotx ذات توقيعات Digital في C#"
description: "كيفية إضافة توقيع Digital ببضعة أسطر من كود .NET"
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
    title: "حول GroupDocs.Signature for .NET واجهة برمجة تطبيقات التوقيعات الرقمية"
    content: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) هي واجهة برمجة تطبيقات شائعة لتصميم المستندات باستخدام التوقيعات الإلكترونية الرقمية ، مع الشهادات الرقمية. بالنسبة إلى التوقيعات الرقمية ، تستخدم API ملفات شهادة PFX لتوقيع المستند باستخدام مفاتيح خاصة وعامة محمية بكلمة مرور. يمكن استخدام التواقيع الرقمية للمصادقة على مستندات الأعمال بصفحة eSign PDF معينة ، والتصديق على مستندات Microsoft Office بالكامل مثل Words و Excel وملفات Powerpoint ومستندات Open Office. يمكن للعملاء التعامل بسهولة مع التوقيعات مثل تحريرها أو إزالتها أو ضبطها. توفر واجهة برمجة التطبيقات طريقة للبحث عن التواقيع والتحقق منها. علاوة على ذلك ، يتم توفير الكثير من القدرات لتخصيص التوقيعات.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "خطوات تسجيل Dotx باستخدام Digital في C#"
    content_left: |
        يوفر [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) إمكانية توقيع مستندات Dotx بتوقيعات Digital بسرعة وسهولة.
        
        * قم بإنشاء مثيل لفئة التوقيع بتوفير ملف Dotx من المفترض أن يتم توقيعه كمسار أو دفق ذاكرة
        * إنشاء فئة SignOptions وتعيين جميع البيانات المطلوبة.
        * استدعاء أسلوب Signature.Sign () تمرير ملف الإخراج Dotx أو دفق الذاكرة

    title_right: " متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for .NET على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * احصل على أحدث إصدار من GroupDocs.Signature for .NET من [Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotx file
        string filePath = "input.dotx";
        // Set up output file
        string outputFilePath = "output.dotx";
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

                // sign Dotx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "توقيع مستندات Dotx باستخدام العرض التوضيحي المباشر Digital"
    content: |
       وقّع ملف Dotx بتوقيعات مختلفة الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). عرض تجريبي مجاني على الإنترنت في انتظارك.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "توقيعات Digital المدعومة الأخرى لـ C#"
    content: |
        "يمكنك أيضًا توقيع Dotx بأنواع التوقيع الأخرى. يرجى الاطلاع على القائمة أدناه."
    format: 
       
       
back_to_top:
    enable: true
---