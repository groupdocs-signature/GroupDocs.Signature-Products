---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Odp
productName: Java
lang: ar
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Odp for Java

############################# Head ############################
head_title: "احذف توقيعات Image من ملفات Odp عبر Java"
head_description: "يمكن إجراء حذف توقيعات معينة من Image من مستندات Odp الموقعة بسهولة باستخدام رمز Java القصير."

############################# Header ############################
title: "قم بإزالة Image التوقيعات التي يتم وضعها في ملفات Odp"
description: "احذف العديد من توقيعات Image من مستندات Odp. تتطلب إزالة توقيعات Image شفرة Java بسيطة."
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
    title: "الحصول على معلومات حول ميزات واجهة برمجة التطبيقات GroupDocs.Signature for Java"
    content: |
        توفر واجهة برمجة تطبيقات [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) العديد من الطرق لمعالجة مستنداتك باستخدام التوقيعات الإلكترونية. التوقيعات الرقمية مثل النصوص والصور والشهادات الرقمية والباركود ورموز QR والطوابع أو البيانات الوصفية متوفرة. يمكن للعملاء إضافة أو حذف أو تحديث أو التحقق من التوقيعات الرقمية أو البحث عنها في ملفات PDF ومستندات MS Word ومصنفات MS Excel وعروض MS PowerPoint التقديمية وملفات Adobe Photoshop وتنسيقات الصور المختلفة. يتم توفير عدد كبير من الميزات والإعدادات المفيدة.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "كيفية إزالة توقيعات Image من مستندك Odp"
    content_left: |
        يوفر [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) ميزة مفيدة لمسح Odp مستندات توقيعات Image ببضعة أسطر من التعليمات البرمجية.
        
        * أولاً ، قم بإنشاء مثيل لكائن التوقيع الذي يمرر المسار إلى وثيقتك كمعامل مُنشئ.
        * ثم قم بإنشاء كائن توقيع مناسب وقم بإعداد معرفه الفريد.
        * بعد ذلك ، استدعاء طريقة Delete تمرير كائن التوقيع الذي يجب حذفه.
        * أخيرًا ، نتائج العملية العملية.

    title_right: "متطلبات النظام"
    content_right: |
        يتم دعم GroupDocs.Signature for Java على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.

        * أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        * بيئات التطوير: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * تنزيل أحدث إصدار من GroupDocs.Signature for Java من [Maven] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Odp file
        String filePath = "input.odp";
        // Set up output file
        String outputFilePath = "output.odp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

        // provide signature features to delete
        ImageSignature signatureToDelete = new ImageSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "التوقيع باستخدام توقيعات Image Live Demo"
    content: |
       أضف توقيعات إلكترونية متنوعة إلى ملف Odp الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "احذف توقيعات Image باستخدام Java"
    content: |
        "حذف التوقيعات الإلكترونية التي تمت إضافتها إلى تنسيقات المستندات المختلفة. قم بإزالة التوقيعات بسرعة بدون رمز إضافي."
    format: 
       
       
back_to_top:
    enable: true
---