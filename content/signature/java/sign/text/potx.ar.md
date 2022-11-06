---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Potx
productName: Java
lang: ar
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Potx for Java

############################# Head ############################
head_title: "إنشاء توقيعات إلكترونية نصية إلى ملف Potx باستخدام Java"
head_description: "ضع Text توقيعًا إلكترونيًا على ملف Potx لـ Java باستخدام بضعة أسطر من التعليمات البرمجية. استخدم GroupDocs Document Signature API لتوقيع عشرات تنسيقات الملفات."

############################# Header ############################
title: "توقيع ملفات Potx بتوقيعات Text في Java"
description: "كيفية إضافة توقيع Text ببضعة أسطر من كود Java"
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
    title: "حول واجهة برمجة تطبيقات GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) هي واجهة برمجة تطبيقات شائعة للتوقيع الإلكتروني للمستندات الرقمية. التوقيعات مثل النصوص والصور والشهادات الرقمية والباركود ورموز QR والطوابع أو البيانات الوصفية متوفرة. يمكن وضع التوقيعات على ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. يمكن للعملاء التوقيع على مستنداتهم وتحديثها أو البحث عنها أو التحقق منها أو حذفها أو معاينة التوقيعات الإلكترونية التي تم وضعها على تلك المستندات. علاوة على ذلك ، يتم توفير الكثير من القدرات لتخصيص التوقيعات.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "خطوات تسجيل Potx باستخدام Text في Java"
    content_left: |
        يوفر [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) إمكانية توقيع مستندات Potx بتوقيعات Text بسرعة وسهولة.
        
        * قم بإنشاء مثيل لفئة التوقيع بتوفير ملف Potx من المفترض أن يتم توقيعه كمسار أو دفق ذاكرة
        * إنشاء فئة SignOptions وتعيين جميع البيانات المطلوبة.
        * استدعاء أسلوب Signature.Sign () تمرير ملف الإخراج Potx أو دفق الذاكرة

    title_right: " متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for Java على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * احصل على أحدث إصدار من GroupDocs.Signature for Java من [Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Potx file
        String filePath = "input.potx";
        // Set up output file
        String outputFilePath = "output.potx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Potx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "توقيع مستندات Potx باستخدام العرض التوضيحي المباشر Text"
    content: |
       وقّع ملف Potx بتوقيعات مختلفة الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). عرض تجريبي مجاني على الإنترنت في انتظارك.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "توقيعات Text المدعومة الأخرى لـ Java"
    content: |
        "يمكنك أيضًا توقيع Potx بأنواع التوقيع الأخرى. يرجى الاطلاع على القائمة أدناه."
    format: 
       
       
back_to_top:
    enable: true
---