---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Gif
productName: Java
lang: ar
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Gif for Java

############################# Head ############################
head_title: "إلحاق التوقيعات الإلكترونية للبيانات الوصفية بمستندات Gif عبر Java"
head_description: "استخدم البيانات الوصفية كتوقيعات إلكترونية مخفية داخل مستندات Gif باستخدام سطرين من كود Java. استخدم GroupDocs Document Signature API للتوقيع الإلكتروني على مستندات العمل والملفات باستخدام معلومات البيانات الوصفية."

############################# Header ############################
title: "تعد التوقيعات الإلكترونية للبيانات الوصفية لمستند Gif عبر Java بسيطة وسهلة الاستخدام!"
description: "قم بتوقيع مستنداتك وعقود Gif باستخدام إدخالات البيانات الوصفية المخفية. قم بإنشاء بيانات وصفية لملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وتنسيقات صور متنوعة بدون مشاكل وترميز إضافي."
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
    title: "حول GroupDocs.Signature for Java واجهة برمجة تطبيقات تواقيع البيانات الوصفية"
    content: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) هي واجهة برمجة تطبيقات شائعة للتوقيع الإلكتروني للمستندات الرقمية. التوقيعات مثل النصوص والصور والشهادات الرقمية والباركود ورموز QR والطوابع أو البيانات الوصفية متوفرة. يمكن وضع التوقيعات على ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. يمكن للعملاء التوقيع على مستنداتهم وتحديثها أو البحث عنها أو التحقق منها أو حذفها أو معاينة التوقيعات الإلكترونية التي تم وضعها على تلك المستندات. علاوة على ذلك ، يتم توفير الكثير من القدرات لتخصيص التوقيعات.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "خطوات تسجيل Gif باستخدام Metadata في Java"
    content_left: |
        يوفر [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) إمكانية توقيع مستندات Gif بتوقيعات Metadata بسرعة وسهولة.
        
        * قم بإنشاء مثيل لفئة التوقيع بتوفير ملف Gif من المفترض أن يتم توقيعه كمسار أو دفق ذاكرة
        * إنشاء فئة SignOptions وتعيين جميع البيانات المطلوبة.
        * استدعاء أسلوب Signature.Sign () تمرير ملف الإخراج Gif أو دفق الذاكرة

    title_right: " متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for Java على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * احصل على أحدث إصدار من GroupDocs.Signature for Java من [Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Gif file
        String filePath = "input.gif";
        // Set up output file
        String outputFilePath = "output.gif";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Gif document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "توقيع مستندات Gif باستخدام العرض التوضيحي المباشر Metadata"
    content: |
       وقّع ملف Gif بتوقيعات مختلفة الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). عرض تجريبي مجاني على الإنترنت في انتظارك.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "توقيعات Metadata المدعومة الأخرى لـ Java"
    content: |
        "يمكنك أيضًا توقيع Gif بأنواع التوقيع الأخرى. يرجى الاطلاع على القائمة أدناه."
    format: 
       
       
back_to_top:
    enable: true
---