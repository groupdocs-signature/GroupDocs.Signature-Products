---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Ppsm
productName: Java
lang: ar
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ppsm for Java

############################# Head ############################
head_title: "وثيقة eSign Ppsm مع Pharmacode رمز شريطي في Java"
head_description: "أنشئ Pharmacode Barcode Signature وضعه في مستند Ppsm باستخدام Java باستخدام سطرين من الشفرة. استخدم GroupDocs Document Signature API لتوقيع تنسيقات ملفات متنوعة."

############################# Header ############################
title: "إنشاء Pharmacode توقيع الرمز الشريطي للمستند Ppsm في Java"
description: "قم بتوقيع Ppsm على مستندات الأعمال باستخدام الرمز الشريطي Pharmacode. قم بإنشاء توقيع الرمز الشريطي بسرعة وسهولة باستخدام بضعة أسطر من التعليمات البرمجية لإعداد خيارات التوقيع."
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
    title: "حول GroupDocs.Signature for Java واجهة برمجة تطبيقات تواقيع الرموز الشريطية."
    content: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) هي واجهة برمجة تطبيقات سريعة وسهلة لإدارة التوقيع الإلكتروني للمستندات الرقمية باستخدام أنواع الرموز الشريطية مثل UPCA و UPCE و EAN13 و EAN14 و Code39 و Code39Extended و Code128 و Codabar و Postnet و ISBN و ITF14 وغيرها الكثير. يمكن للعملاء إنشاء رموز شريطية بسهولة لتوفير النص المطلوب ووضعها على PDF ومستندات Microsoft Office Words ومصنفات Microsoft Office Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. يمكن تحديث الرموز الشريطية الموضوعة في المستندات أو البحث فيها أو التحقق منها أو حذفها أو معاينتها. علاوة على ذلك ، يتم دعم تخصيص الباركود.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "خطوات تسجيل Ppsm باستخدام Barcode في Java"
    content_left: |
        يوفر [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) إمكانية توقيع مستندات Ppsm بتوقيعات Barcode بسرعة وسهولة.
        
        * قم بإنشاء مثيل لفئة التوقيع بتوفير ملف Ppsm من المفترض أن يتم توقيعه كمسار أو دفق ذاكرة
        * إنشاء فئة SignOptions وتعيين جميع البيانات المطلوبة.
        * استدعاء أسلوب Signature.Sign () تمرير ملف الإخراج Ppsm أو دفق الذاكرة

    title_right: " متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for Java على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * احصل على أحدث إصدار من GroupDocs.Signature for Java من [Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ppsm file
        String filePath = "input.ppsm";
        // Set up output file
        String outputFilePath = "output.ppsm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Pharmacode);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Ppsm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "توقيع مستندات Ppsm باستخدام العرض التوضيحي المباشر Barcode"
    content: |
       وقّع ملف Ppsm بتوقيعات مختلفة الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). عرض تجريبي مجاني على الإنترنت في انتظارك.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            الكود الصيدلاني ، المعروف أيضًا باسم الكود الثنائي الصيدلاني ، هو معيار الباركود ، يستخدم في صناعة الأدوية كنظام للتحكم في التعبئة.
          characterset: |
             أرقام رقمية (0-9).
          textcapacity: |
             يمثل عددًا صحيحًا واحدًا فقط من 3 إلى 131070.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "توقيعات Barcode المدعومة الأخرى لـ Java"
    content: |
        "يمكنك أيضًا توقيع Ppsm بأنواع التوقيع الأخرى. يرجى الاطلاع على القائمة أدناه."
    format: 
        
       
back_to_top:
    enable: true
---