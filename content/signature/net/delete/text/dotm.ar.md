---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Dotm
productName: .NET
lang: ar
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Dotm for C#

############################# Head ############################
head_title: "احذف توقيعات Text من ملفات Dotm عبر C#"
head_description: "يمكن إجراء حذف توقيعات معينة من Text من مستندات Dotm الموقعة بسهولة باستخدام رمز .NET القصير."

############################# Header ############################
title: "قم بإزالة Text التوقيعات التي يتم وضعها في ملفات Dotm"
description: "احذف العديد من توقيعات Text من مستندات Dotm. تتطلب إزالة توقيعات Text شفرة C# بسيطة."
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
    title: "الحصول على معلومات حول ميزات واجهة برمجة التطبيقات GroupDocs.Signature for .NET"
    content: |
        توفر واجهة برمجة تطبيقات [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) العديد من الطرق لمعالجة مستنداتك باستخدام التوقيعات الإلكترونية. التوقيعات الرقمية مثل النصوص والصور والشهادات الرقمية والباركود ورموز QR والطوابع أو البيانات الوصفية متوفرة. يمكن للعملاء إضافة أو حذف أو تحديث أو التحقق من التوقيعات الرقمية أو البحث عنها في ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. يتم توفير عدد كبير من الميزات والإعدادات المفيدة.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "كيفية إزالة توقيعات Text من مستندك Dotm"
    content_left: |
        يوفر [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) ميزة مفيدة لمسح Dotm مستندات توقيعات Text ببضعة أسطر من التعليمات البرمجية.
        
        * أولاً ، قم بإنشاء مثيل لكائن التوقيع الذي يمرر المسار إلى وثيقتك كمعامل مُنشئ.
        * ثم قم بإنشاء كائن توقيع مناسب وقم بإعداد معرفه الفريد.
        * بعد ذلك ، استدعاء طريقة Delete تمرير كائن التوقيع الذي يجب حذفه.
        * أخيرًا ، نتائج العملية العملية.

    title_right: "متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for .NET على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * تنزيل أحدث إصدار من GroupDocs.Signature for .NET من [Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotm file
        string filePath = "input.dotm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to delete
                // set up particular signature id
                TextSignature signatureToDelete = new TextSignature(id);

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
    title: "التوقيع باستخدام توقيعات Text Live Demo"
    content: |
       أضف توقيعات إلكترونية متنوعة إلى ملف Dotm الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "احذف توقيعات Text باستخدام C#"
    content: |
        "حذف التوقيعات الإلكترونية التي تمت إضافتها إلى تنسيقات المستندات المختلفة. قم بإزالة التوقيعات بسرعة بدون رمز إضافي."
    format: 
       
       
back_to_top:
    enable: true
---