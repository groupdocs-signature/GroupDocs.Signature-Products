---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Docm
productName: Java
lang: ar
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docm for Java

############################# Head ############################
head_title: "احذف توقيعات Digital من ملفات Docm عبر Java"
head_description: "يمكن إجراء حذف توقيعات معينة من Digital من مستندات Docm الموقعة بسهولة باستخدام رمز Java القصير."

############################# Header ############################
title: "قم بإزالة Digital التوقيعات التي يتم وضعها في ملفات Docm"
description: "احذف العديد من توقيعات Digital من مستندات Docm. تتطلب إزالة توقيعات Digital شفرة Java بسيطة."
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
    title_left: "كيفية إزالة توقيعات Digital من مستندك Docm"
    content_left: |
        يوفر [GroupDocs.Signature for Java] (https://products.groupdocs.com/signature/java/) ميزة مفيدة لمسح Docm مستندات توقيعات Digital ببضعة أسطر من التعليمات البرمجية.
        
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
                
        // Set up input Docm file
        String filePath = "input.docm";
        // Set up output file
        String outputFilePath = "output.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "a01e1940-997a-444b-89af-9309a2d559a5";

        // provide signature item to delete
        DigitalSignature signatureToDelete = new DigitalSignature(id);

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
    title: "التوقيع باستخدام توقيعات Digital Live Demo"
    content: |
       أضف توقيعات إلكترونية متنوعة إلى ملف Docm الآن من خلال زيارة موقع ويب [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "احذف توقيعات Digital باستخدام Java"
    content: |
        "حذف التوقيعات الإلكترونية التي تمت إضافتها إلى تنسيقات المستندات المختلفة. قم بإزالة التوقيعات بسرعة بدون رمز إضافي."
    format: 
       
       
back_to_top:
    enable: true
---