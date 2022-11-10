---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Png
productName: Java
lang: ar
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Png for Java

############################# Head ############################
head_title: "التحقق من توقيعات Qrcode لملفات Png عبر Java"
head_description: "استخدم فقط بضعة أسطر من كود Java للتحقق من مستندات Png وتوقيعاتها Qrcode."

############################# Header ############################
title: "التحقق من صحة التوقيعات Qrcode لملفات Png"
description: "توفر واجهة برمجة التطبيقات لـ Java فرصة للتحقق من توقيعات Qrcode في مستندات Png. قد يتم التحقق من صحة التوقيعات الإلكترونية داخل مستندات Png بسرعة وسهولة."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "اكتشف ميزات واجهة برمجة تطبيقات GroupDocs.Signature for Java الجديدة"
    content: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) توفر واجهة برمجة التطبيقات مجموعة واسعة من الطرق لمعالجة العديد من تنسيقات المستندات باستخدام التوقيعات الإلكترونية. يتم دعم العديد من أنواع التوقيعات الرقمية مثل النصوص أو الصور أو الشهادات الرقمية أو الرموز الشريطية أو رموز QR أو الطوابع أو البيانات الوصفية. يمكن للعملاء إضافة أو إزالة أو تحرير أو التحقق من صحة أو البحث عن التوقيعات الرقمية في ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. يتوفر عدد مذهل من الميزات والإعدادات الإضافية.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "كيفية التحقق من صحة توقيعات Qrcode في مستندك Png"
    content_left: |
        يتضمن [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) ميزات مفيدة مثل التحقق من التوقيعات Qrcode الموضوعة في مستندات Png. اغتنم هذه الفرصة دون تنفيذ كود إضافي.
        
        * أولاً ، قم بإنشاء مثيل لفئة التوقيع التي توفر كمسار معلمة منشئ لمستند من المفترض أن يتم التحقق منه.
        * ثانيًا ، قم بإنشاء كائن VerifyOptions جديد وقم بإعداد جميع الخصائص المطلوبة.
        * أخيرًا ، استدعاء طريقة التحقق من كائن Signature لتمرير مثيل VerifyOptions.
        * ثم معالجة نتائج التحقق.

    title_right: "متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for Java على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * تنزيل أحدث إصدار من GroupDocs.Signature for Java من [Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Png file
        String filePath = "input.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "التوقيع باستخدام توقيعات Qrcode Live Demo"
    content: |
       أضف توقيعات إلكترونية متنوعة إلى ملف Png الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "تحقق من توقيعات Qrcode الأخرى باستخدام Java"
    content: |
        "التحقق من صحة التوقيعات الإلكترونية الموضوعة في مستندات مختلفة. تحقق من جودة التوقيعات بتنسيقات الملفات الشائعة كما هو موضح أدناه."
    format: 
       
       
back_to_top:
    enable: true
---