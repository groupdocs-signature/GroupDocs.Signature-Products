---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Otp
productName: Java
lang: ar
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Otp with Java

############################# Head ############################
head_title: "ابحث عن توقيعات Metadata في ملف Otp في Java"
head_description: "استخدم Java للبحث عن توقيعات Metadata في ملفات Otp باستخدام بضعة أسطر من التعليمات البرمجية."

############################# Header ############################
title: "ابحث عن توقيعات Metadata في ملف Otp"
description: "تسمح واجهة برمجة التطبيقات الأصلية لـ Java بالبحث عن توقيعات Metadata في ملفات Otp الموقعة بالفعل. قم بإجراء بحث متقدم عن التوقيع الإلكتروني داخل مستندات Otp باستخدام بضعة أسطر من التعليمات البرمجية."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "حول واجهة برمجة تطبيقات GroupDocs.Signature for Java"
    content: |
        يوفر [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) واجهة برمجة تطبيقات Java لمعالجة المستندات باستخدام أنواع توقيع متنوعة مثل النصوص والصور والشهادات الرقمية والباركود ورموز الاستجابة السريعة والطوابع والبيانات الوصفية. يمكن للمستخدمين إضافة أو حذف أو تحديث أو التحقق من التوقيعات الإلكترونية أو البحث عنها ضمن ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة ، مع دعم إضافي لتخصيص خصائص التوقيعات حسب الحاجة.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "كيفية البحث عن توقيعات Metadata في Otp"
    content_left: |
        يسهّل [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) على مطوري Java البحث عن توقيعات Metadata في ملفات Otp من تطبيقاتهم من خلال تنفيذ بضع خطوات سهلة.
        
        * قم بإنشاء مثيل جديد لفئة التوقيع وتمرير مسار المستند المصدر كمعامل مُنشئ.
        * قم بإنشاء كائن SearchOptions وفقًا لمتطلباتك وحدد خيارات البحث.
        * طريقة البحث عن المكالمات لمثيل فئة التوقيع وتمرير SearchOptions إليها.
        * نتائج البحث العملية وفقا لمتطلباتك.

    title_right: "متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for Java على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * تنزيل أحدث إصدار من GroupDocs.Signature for Java من [Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Otp file
        String filePath = "input.otp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // search for Metadata signatures in Otp document
        List<PresentationMetadataSignature> signatures = signature.search(PresentationMetadataSignature.class, SignatureType.Metadata);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));


        ```

############################# Demos ############################
demos:
    enable: true
    title: "ابحث عن Metadata توقيعات إلكترونية Live Demo"
    content: |
       ابحث في المستند عن توقيعات إلكترونية متنوعة لملفات Otp الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "ابحث عن توقيعات Metadata أخرى باستخدام Java"
    content: |
        "التوقيعات الإلكترونية تبحث في وثائق مختلفة. ابحث عن التوقيعات من أحد تنسيقات الملفات الشائعة كما هو موضح أدناه."
    format: 
           
       
back_to_top:
    enable: true
---