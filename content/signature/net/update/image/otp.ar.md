---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Otp
productName: .NET
lang: ar
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Otp for C#

############################# Head ############################
head_title: "تحديث Image التوقيعات الموضوعة في ملفات Otp باستخدام C#"
head_description: "استخدم رمز .NET البسيط والسهل الفهم لتحديث التوقيعات Image في المستندات الموقعة Otp."

############################# Header ############################
title: "قم بتحرير وتحديث توقيعات Image الموضوعة في ملفات Otp"
description: "توفر واجهة برمجة التطبيقات لـ .NET وظيفة لتحديث توقيعات Image في مستندات Otp. قم بتحديث التوقيعات الإلكترونية داخل مستندات Otp باستخدام سطرين من كود C# بسرعة وسهولة."
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
    title: "تعرف على ميزات واجهة برمجة التطبيقات GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) تحتوي وظيفة واجهة برمجة التطبيقات على مجموعة كبيرة من وسائل المعالجة بتنسيقات المستندات المطلوبة باستخدام التوقيعات الإلكترونية. يتم دعم مجموعة واسعة من التوقيعات الإلكترونية مثل النصوص أو الصور أو الشهادات الرقمية أو الرموز الشريطية أو رموز QR أو الطوابع أو البيانات الوصفية. يمكن للعملاء إضافة أو إزالة أو تحرير أو التحقق من صحة أو البحث عن التوقيعات الرقمية في ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. تتوفر العديد من الميزات والإعدادات المفيدة.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "كيفية تغيير توقيعات Image في مستندك Otp"
    content_left: |
        يتضمن [GroupDocs.Signature for .NET] (https://products.groupdocs.com/signature/net/) ميزات مفيدة مثل تحديث توقيعات Image الموضوعة في مستندات Otp. يجعل من الممكن تغيير ميزات التوقيعات بدون رمز إضافي.
        
        * للبدء ، قم بإنشاء كائن التوقيع الذي يمر كمسار معلمة منشئ إلى مستند من المفترض أن يتم تحديثه.
        * بعد ذلك ، قم بإنشاء مثيل لكائن توقيع معين مناسب وقم بإعداد معرفه وخصائصه التي يجب تغييرها.
        * أخيرًا ، قم باستدعاء طريقة تحديث التوقيع لتمرير كائن توقيع معين.
        * عملية تحديث النتائج لإشعارك.

    title_right: "متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for .NET على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * تنزيل أحدث إصدار من GroupDocs.Signature for .NET من [Nuget] (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Otp file
        string filePath = "input.otp";

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
    title: "تحديث توقيعات Image على صفحات الوثيقة - العرض التوضيحي المباشر"
    content: |
       قم بتحرير التواقيع الإلكترونية المتنوعة لمستند Otp الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "تحديث العديد من توقيعات Image عبر C#"
    content: |
        "تحرير التوقيعات الرقمية الموضوعة في تنسيقات مستندات مختلفة. تحديث بيانات التوقيعات بدون كود إضافي."
    format: 
       
       
back_to_top:
    enable: true
---