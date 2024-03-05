---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ar
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "NET و Java و Cloud APIs وتطبيقات توقيع المستندات عبر الإنترنت"
head_description: "احصل على حل التوقيع الإلكتروني الشامل للمستند للتطبيقات المستندة إلى .NET و Java والتطبيقات المستندة إلى السحابة. قم بتوقيع تنسيقات المستندات الشائعة عبر الإنترنت باستخدام ميزة السحب والإفلات البسيطة"

############################# Header ############################
title: "التوقيع على وثائق<br>مع Node.js API"
description: "قم بتوقيع المستندات والصور الرقمية على أي نظام أساسي باستخدام واجهات برمجة التطبيقات المرنة والحلول القائمة على التطبيقات للمبرمجين والمستخدمين النهائيين."
words:
  for: "ل"

actions:
  main: "تحميل من NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "الترخيص"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "على استعداد للبدء؟"
  description: "جرب ميزات GroupDocs.Signature مجانًا أو اطلب ترخيصًا"

release:
  title: "تم إصدار الإصدار {0}."
  notes: "ترى ما هو الجديد"
  downloads: "التحميلات"

code:
  title: "توقيع ملفات PDF بواسطة Node.js"
  more: "مزيد من الأمثلة"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // حدد مستند PDF
    let signature = new Signature("sample.pdf");
    
    // تقديم النص
    let options = new TextSignOptions("John Smith");
    
    // ضبط اللون
    options.ForeColor = Color.Red;
    
    // قم بتوقيع الوثيقة وحفظها في ملف
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.نظرة عامة على التوقيع"
  description: "مكتبة توقيع المستندات الجاهزة للاستخدام في تطبيقات Node.js"
  features:
    # feature loop
    - title: "حل التوقيعات الرقمية لمستندات الأعمال باستخدام Node.js"
      content: "يقدم GroupDocs.Signature for Node.js via Java مجموعة شاملة من خيارات التوقيع الرقمي لملفات PDF ومستندات Office والصور. تتوفر النصوص والرموز الشريطية والصور والشهادات الرقمية والبيانات الوصفية. معالجة المستندات المبسطة تضمن الكفاءة."

    # feature loop
    - title: "التلاعب المتقدم بالوثائق الموقعة"
      content: "يمكّنك GroupDocs.Signature من معالجة المستندات الموقعة. البحث والتحقق من صحة التوقيعات باستخدام معايير مختلفة. بالإضافة إلى ذلك، يمكنك استخراج معلومات تفصيلية عن المستند أو إنشاء صور معاينة للصفحات."

    # feature loop
    - title: "تنسيقات الإخراج المتنوعة"
      content: "يوفر الحل الذي نقدمه تحكمًا شاملاً في تنسيق إخراج المستندات الموقعة. وضع التوقيعات بدقة على أي صفحة وتخصيص مظهرها. احفظ المستندات الموقعة بالعديد من التنسيقات المدعومة وقم بتأمينها اختياريًا بكلمات مرور."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلالية المنصة"
  description: "يقوم GroupDocs.Signature for Node.js via Java بمعالجة المستندات باستخدام أنظمة تشغيل مختلفة"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "تنسيقات الملفات المدعومة"
  description: |
    يسهل GroupDocs.Signature for Node.js via Java عمليات [تنسيقات الملفات الشائعة](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### تنسيقات مايكروسوفت أوفيس
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### الصور والتنسيقات الأخرى
        * **محمول:** PDF
        * **الصور:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **أشكال مكتبية أخرى:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### تنسيقات أخرى
        * **ويب:** HTML, MHTML
        * **أرشيف:** ZIP, TAR, 7Z
        * **الشهادات:** PFX

############################# Features ############################
features:
  enable: true
  title: "مميزات GroupDocs.Signature"
  description: "قم بتوقيع ملفات PDF ومستندات Office والصور باستخدام التوقيعات الرقمية"

  items:
    # feature loop
    - icon: "sign"
      title: "التوقيعات التجارية"
      content: "استخدم أنواع التوقيع المختلفة لتوقيع المستندات. ضع التوقيعات الرقمية بدقة على أي موقع بالصفحة."

    # feature loop
    - icon: "custom"
      title: "تخصيص مظهر التوقيع"
      content: "قم بتخصيص الجوانب المرئية للتوقيعات عن طريق ضبط اللون والخط والحدود والتدوير والمزيد لتحقيق النتيجة المرجوة."

    # feature loop
    - icon: "password"
      title: "المستندات المحمية بكلمة مرور"
      content: "بالنسبة للعديد من تنسيقات المستندات المدعومة، قم بحماية المستندات الموقعة بكلمة مرور لمزيد من الأمان."

    # feature loop
    - icon: "protect"
      title: "منع التعديلات غير المصرح بها"
      content: "قم بحماية مستندات الأعمال المهمة الموقعة بشهادات رقمية من التعديلات غير المصرح بها."

    # feature loop
    - icon: "convert"
      title: "تنسيقات الإخراج المطلوبة"
      content: "احصل بسهولة على المستندات الموقعة بأي تنسيق مدعوم. قم بتحويل مستندات MS Word إلى تنسيق PDF بسهولة."

    # feature loop
    - icon: "preview"
      title: "معاينة المستندات"
      content: "احفظ صفحات المستندات الفردية كصور لتلبية الاحتياجات المستقبلية."

    # feature loop
    - icon: "search"
      title: "بحث التوقيع"
      content: "استرجع معلومات حول التوقيعات المضافة مسبقًا داخل مستنداتك."

    # feature loop
    - icon: "validate"
      title: "التحقق من صحة الوثيقة"
      content: "التحقق من صحة التوقيعات المقدمة في أي وثيقة."

    # feature loop
    - icon: "update"
      title: "إدارة التوقيع"
      content: "حذف أو نقل أو تعديل أي توقيعات موضوعة على أي صفحة مستند."

############################# Code samples ############################
code_samples:
  enable: true
  title: "عينات التعليمات البرمجية"
  description: "أمثلة توضيحية تعرض عمليات GroupDocs.Signature for Node.js via Java النموذجية"
  items:
    # code sample loop
    - title: "قم بتمييز ملف PDF باستخدام رموز QR"
      content: |
        يمكن أن يؤدي دمج [الرموز الشريطية](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) في صفحات مستندات PDF محددة إلى تبسيط العمليات التجارية. يقدم هذا القسم مثالاً على إضافة رمز الاستجابة السريعة باستخدام GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="كيفية وضع رمز الاستجابة السريعة على PDF.">}}
        ```javascript {style=abap}
        // قم بتحميل المستند للتوقيع
        let signature = new Signature("file_to_sign.pdf");
        
        // قم بإنشاء خيارات رمز الاستجابة السريعة بنص محدد مسبقًا
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // قم بتكوين نوع ترميز رمز الاستجابة السريعة وموضعه على الصفحة
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // قم بتوقيع المستند واحفظه كملف النتيجة
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "حماية DOCX بالتوقيع الرقمي"
      content: |
        [حماية مستنداتك](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) من خلال التوقيعات المستندة إلى الشهادات الرقمية. يعمل التوقيع الرقمي على حماية مستندات عملك من تغيير المحتوى.
        {{< landing/code title="إليك كيفية ضمان سلامة المستند.">}}
        ```javascript {style=abap}   
        // قم بتحميل المستند ليتم توقيعه رقميًا
        let signature = new Signature("file_to_sign.docx");
        
        // حدد خيارات التوقيع الرقمي وقم بتوفير المسار إلى ملف الشهادة
        let options = new DigitalSignOptions("certificate.pfx");

        // قم بتعيين كلمة مرور الشهادة
        options.Password = "1234567890";

        // قم بتوقيع المستند وحفظه في المسار المطلوب
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
