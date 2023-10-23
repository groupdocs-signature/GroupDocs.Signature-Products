---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Zip
productName: .NET
lang: ar
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Zip with C#

############################# Head ############################
head_title: "ابحث عن توقيعات Text في ملف Zip في C#"
head_description: "استخدم .NET للبحث عن توقيعات Text في ملفات Zip باستخدام بضعة أسطر من التعليمات البرمجية."

############################# Header ############################
title: "ابحث عن توقيعات Text في ملف Zip"
description: "تسمح واجهة برمجة التطبيقات الأصلية لـ .NET بالبحث عن توقيعات Text في ملفات Zip الموقعة بالفعل. قم بإجراء بحث متقدم عن التوقيع الإلكتروني داخل مستندات Zip باستخدام بضعة أسطر من التعليمات البرمجية."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "حول واجهة برمجة تطبيقات GroupDocs.Signature for .NET"
    content: |
        يوفر [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) واجهة برمجة تطبيقات .NET لمعالجة المستندات باستخدام أنواع توقيع متنوعة مثل النصوص والصور والشهادات الرقمية والباركود ورموز الاستجابة السريعة والطوابع والبيانات الوصفية. يمكن للمستخدمين إضافة أو حذف أو تحديث أو التحقق من التوقيعات الإلكترونية أو البحث عنها ضمن ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة ، مع دعم إضافي لتخصيص خصائص التوقيعات حسب الحاجة.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "كيفية البحث عن توقيعات Text في Zip"
    content_left: |
        يسهّل [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) على مطوري .NET البحث عن توقيعات Text في ملفات Zip من تطبيقاتهم من خلال تنفيذ بضع خطوات سهلة.
        
        * قم بإنشاء مثيل جديد لفئة التوقيع وتمرير مسار المستند المصدر كمعامل مُنشئ.
        * قم بإنشاء كائن SearchOptions وفقًا لمتطلباتك وحدد خيارات البحث.
        * طريقة البحث عن المكالمات لمثيل فئة التوقيع وتمرير SearchOptions إليها.
        * نتائج البحث العملية وفقا لمتطلباتك.

    title_right: "متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for .NET على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * تنزيل أحدث إصدار من GroupDocs.Signature for .NET من [Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Zip file
        string filePath = "input.zip";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                TextSearchOptions options = new TextSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // specify text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature"
                };

                // search for Text signatures in Zip document
                List<TextSignature> signatures = signature.Search<TextSignature>(options);

                // process signatures which were found                
                foreach (TextSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "ابحث عن Text توقيعات إلكترونية Live Demo"
    content: |
       ابحث في المستند عن توقيعات إلكترونية متنوعة لملفات Zip الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "ابحث عن توقيعات Text أخرى باستخدام C#"
    content: |
        "التوقيعات الإلكترونية تبحث في وثائق مختلفة. ابحث عن التوقيعات من أحد تنسيقات الملفات الشائعة كما هو موضح أدناه."
    format: 
           
       
back_to_top:
    enable: true
---