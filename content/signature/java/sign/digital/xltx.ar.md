---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xltx
productName: Java
lang: ar
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xltx for Java

############################# Head ############################
head_title: "إضافة التوقيعات الإلكترونية الرقمية إلى ملف Xltx باستخدام Java"
head_description: "ضع التوقيع الرقمي على ملف Xltx لـ Java باستخدام بضعة أسطر من التعليمات البرمجية. استخدم GroupDocs Document Signature API لتوقيع عشرات تنسيقات الملفات."

############################# Header ############################
title: "ملفات eSign Xltx ذات توقيعات Digital في Java"
description: "كيفية إضافة توقيع Digital ببضعة أسطر من كود Java"
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
    title: "حول GroupDocs.Signature for Java واجهة برمجة تطبيقات التوقيعات الرقمية"
    content: |
        [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) هي واجهة برمجة تطبيقات شائعة لتصميم المستندات باستخدام التوقيعات الإلكترونية الرقمية ، مع الشهادات الرقمية. بالنسبة إلى التوقيعات الرقمية ، تستخدم API ملفات شهادة PFX لتوقيع المستند باستخدام مفاتيح خاصة وعامة محمية بكلمة مرور. يمكن استخدام التواقيع الرقمية للمصادقة على مستندات الأعمال بصفحة eSign PDF معينة ، والتصديق على مستندات Microsoft Office بالكامل مثل Words و Excel وملفات Powerpoint ومستندات Open Office. يمكن للعملاء التعامل بسهولة مع التوقيعات مثل تحريرها أو إزالتها أو ضبطها. توفر واجهة برمجة التطبيقات طريقة للبحث عن التواقيع والتحقق منها. علاوة على ذلك ، يتم توفير الكثير من القدرات لتخصيص التوقيعات.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "خطوات تسجيل Xltx باستخدام Digital في Java"
    content_left: |
        يوفر [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) إمكانية توقيع مستندات Xltx بتوقيعات Digital بسرعة وسهولة.
        
        * قم بإنشاء مثيل لفئة التوقيع بتوفير ملف Xltx من المفترض أن يتم توقيعه كمسار أو دفق ذاكرة
        * إنشاء فئة SignOptions وتعيين جميع البيانات المطلوبة.
        * استدعاء أسلوب Signature.Sign () تمرير ملف الإخراج Xltx أو دفق الذاكرة

    title_right: " متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for Java على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * احصل على أحدث إصدار من GroupDocs.Signature for Java من [Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltx file
        String filePath = "input.xltx";
        // Set up output file
        String outputFilePath = "output.xltx";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Xltx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "توقيع مستندات Xltx باستخدام العرض التوضيحي المباشر Digital"
    content: |
       وقّع ملف Xltx بتوقيعات مختلفة الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family). عرض تجريبي مجاني على الإنترنت في انتظارك.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "توقيعات Digital المدعومة الأخرى لـ Java"
    content: |
        "يمكنك أيضًا توقيع Xltx بأنواع التوقيع الأخرى. يرجى الاطلاع على القائمة أدناه."
    format: 
       
       
back_to_top:
    enable: true
---