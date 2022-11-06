---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Docx
productName: .NET
lang: ar
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Docx for C#

############################# Head ############################
head_title: "إلحاق التوقيعات الإلكترونية للبيانات الوصفية بمستندات Docx عبر C#"
head_description: "استخدم البيانات الوصفية كتوقيعات إلكترونية مخفية داخل مستندات Docx باستخدام سطرين من كود C#. استخدم GroupDocs Document Signature API للتوقيع الإلكتروني على مستندات العمل والملفات باستخدام معلومات البيانات الوصفية."

############################# Header ############################
title: "تعد التوقيعات الإلكترونية للبيانات الوصفية لمستند Docx عبر .NET بسيطة وسهلة الاستخدام!"
description: "قم بتوقيع مستنداتك وعقود Docx باستخدام إدخالات البيانات الوصفية المخفية. قم بإنشاء بيانات وصفية لملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وتنسيقات صور متنوعة بدون مشاكل وترميز إضافي."
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
    title: "حول GroupDocs.Signature for .NET واجهة برمجة تطبيقات تواقيع البيانات الوصفية"
    content: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) هي واجهة برمجة تطبيقات شائعة للتوقيع الإلكتروني للمستندات الرقمية. التوقيعات مثل النصوص والصور والشهادات الرقمية والباركود ورموز QR والطوابع أو البيانات الوصفية متوفرة. يمكن وضع التوقيعات على ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. يمكن للعملاء التوقيع على مستنداتهم وتحديثها أو البحث عنها أو التحقق منها أو حذفها أو معاينة التوقيعات الإلكترونية التي تم وضعها على تلك المستندات. علاوة على ذلك ، يتم توفير الكثير من القدرات لتخصيص التوقيعات.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "خطوات تسجيل Docx باستخدام Metadata في C#"
    content_left: |
        يوفر [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) إمكانية توقيع مستندات Docx بتوقيعات Metadata بسرعة وسهولة.
        
        * قم بإنشاء مثيل لفئة التوقيع بتوفير ملف Docx من المفترض أن يتم توقيعه كمسار أو دفق ذاكرة
        * إنشاء فئة SignOptions وتعيين جميع البيانات المطلوبة.
        * استدعاء أسلوب Signature.Sign () تمرير ملف الإخراج Docx أو دفق الذاكرة

    title_right: " متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for .NET على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * احصل على أحدث إصدار من GroupDocs.Signature for .NET من [Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Docx file
        string filePath = "input.docx";
        // Set up output file
        string outputFilePath = "output.docx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Docx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "توقيع مستندات Docx باستخدام العرض التوضيحي المباشر Metadata"
    content: |
       وقّع ملف Docx بتوقيعات مختلفة الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). عرض تجريبي مجاني على الإنترنت في انتظارك.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "توقيعات Metadata المدعومة الأخرى لـ C#"
    content: |
        "يمكنك أيضًا توقيع Docx بأنواع التوقيع الأخرى. يرجى الاطلاع على القائمة أدناه."
    format: 
       
       
back_to_top:
    enable: true
---