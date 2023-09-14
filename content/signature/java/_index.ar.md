---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:21
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ar
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "NET و Java و Cloud APIs وتطبيقات توقيع المستندات عبر الإنترنت"
head_description: "احصل على حل التوقيع الإلكتروني الشامل للمستند للتطبيقات المستندة إلى .NET و Java والتطبيقات المستندة إلى السحابة. قم بتوقيع تنسيقات المستندات الشائعة عبر الإنترنت باستخدام ميزة السحب والإفلات البسيطة"

############################# Header ############################
title: "التوقيع على وثائق<br>عبر جافا API"
description: "قم بتوقيع المستندات والصور الرقمية على أي نظام أساسي باستخدام واجهات برمجة التطبيقات المرنة والحلول القائمة على التطبيقات للمبرمجين والمستخدمين النهائيين."
words:
  for: "ل"

actions:
  main: "تحميل مافن مجانا"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "الترخيص"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "على استعداد للبدء؟"
  description: "جرب ميزات GroupDocs.Signature مجانًا أو اطلب ترخيصًا"

release:
  title: "تم إصدار الإصدار {0}."
  notes: "ترى ما هو الجديد"
  downloads: "التحميلات"

code:
  title: "تسجيل ملفات PDF في جافا"
  more: "مزيد من الأمثلة"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // حدد مستند PDF
    Signature signature = new Signature("sample.pdf");
    
    // تقديم النص
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // قم بتوقيع الوثيقة وحفظها في ملف
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.نظرة عامة على التوقيع"
  description: "واجهة برمجة التطبيقات (API) لتنفيذ توقيع المستندات والعمليات ذات الصلة في تطبيقات Java"
  features:
    # feature loop
    - title: "تحسين مستندات الأعمال باستخدام التوقيعات الرقمية في Java"
      content: "التوقيع السريع والقابل للتخصيص: يقدم GroupDocs.Signature for Java مجموعة واسعة من خيارات التوقيع الرقمي لملفات PDF والصور ومستندات Office. يمكنك استخدام النصوص أو الرموز الشريطية أو رموز QR أو الشهادات الرقمية أو الصور أو البيانات الوصفية المخفية. معالجة المستندات سريعة وفعالة."

    # feature loop
    - title: "التلاعب بالوثائق الموقعة"
      content: "تتضمن المعالجة المتقدمة للمستندات عمليات قوية على المستندات الموقعة باستخدام GroupDocs.Signature لـ Java. يمكنك البحث عن التوقيعات التي تمت إضافتها إلى مستندات الأعمال والتحقق من صحتها باستخدام معايير مفيدة متعددة. بالإضافة إلى ذلك، يمكنك الوصول إلى معلومات تفصيلية حول المستند أو الحصول على صور معاينة لصفحاته."

    # feature loop
    - title: "مجموعة متنوعة من خيارات الإخراج"
      content: "تتيح لك خيارات التوقيع القوية تخصيص مخرجات المستندات الموقعة باستخدام GroupDocs.Signature for Java. يمكنك وضع أي توقيع بدقة على أي صفحة مستند وتكوين مظهره بطرق مختلفة. تدعم Java API حفظ مستندات الأعمال الموقعة في العديد من التنسيقات المدعومة وتوفر خيارات لتأمينها بكلمات مرور."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلالية المنصة"
  description: "يدعم GroupDocs.Signature for Java أنظمة التشغيل وأطر العمل ومديري الحزم التالية"
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "تنسيقات الملفات المدعومة"
  description: |
    يدعم GroupDocs.Signature for Java تنسيقات الملفات [التالية](https://docs.groupdocs.com/signature/java/supported-document-formats/) العمليات باستخدام.
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
  title: "ميزات GroupDocs.Signature"
  description: "توقيع ملفات PDF ومستندات Office والصور بالتوقيعات الرقمية"

  items:
    # feature loop
    - icon: "sign"
      title: "إضافة التوقيعات"
      content: "قم بتوقيع مستند باستخدام أنواع التوقيع المدعومة المختلفة عن طريق وضع التوقيع الرقمي بدقة في أي موضع على أي صفحة."

    # feature loop
    - icon: "custom"
      title: "تخصيص النتائج"
      content: "قم بتخصيص مظهر التوقيع عن طريق ضبط اللون والخط والحدود والتدوير والميزات الأخرى لتحقيق النتيجة المرجوة."

    # feature loop
    - icon: "password"
      title: "تأمين المستندات بكلمة مرور"
      content: "بالنسبة للعديد من أنواع المستندات المدعومة، يمكنك حماية المستند الموقع بكلمة مرور."

    # feature loop
    - icon: "protect"
      title: "منع التغييرات غير المصرح بها"
      content: "حماية مستندات العمل المهمة الموقعة بشهادة رقمية من التعديلات غير المصرح بها."

    # feature loop
    - icon: "convert"
      title: "الحصول على النتائج بالصيغ المطلوبة"
      content: "يمكنك بسهولة الحصول على ملفات النتائج الموقعة بأي تنسيق مدعوم. يمكنك أيضًا تحويل مستندات MS Word إلى PDF بسهولة."

    # feature loop
    - icon: "preview"
      title: "معاينة الوثيقة"
      content: "احفظ أي صفحة من المستند كصورة للمعالجة المستقبلية."

    # feature loop
    - icon: "search"
      title: "البحث عن التوقيعات"
      content: "من الممكن الحصول على معلومات حول التوقيعات المضافة مسبقًا في مستندات محددة."

    # feature loop
    - icon: "validate"
      title: "التحقق من صحة الوثائق"
      content: "التحقق من صحة التوقيعات على أي وثيقة موقعة."

    # feature loop
    - icon: "update"
      title: "إدارة التوقيعات"
      content: "بمجرد وضع التوقيع على صفحة المستند، يمكن حذفه أو نقله أو تحديثه حسب الحاجة."

############################# Code samples ############################
code_samples:
  enable: true
  title: "عينات التعليمات البرمجية"
  description: "تستخدم بعض حالات GroupDocs.Signature النموذجية لعمليات Java"
  items:
    # code sample loop
    - title: "Enchance وثيقة PDF مع رمز الاستجابة السريعة"
      content: |
        يمكن أن يكون تحسين العمليات التجارية عن طريق إضافة [رموز QR](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) إلى صفحات محددة من مستندات PDF أمرًا ذا قيمة. يوجد مثال لكيفية إضافة رمز QR باستخدام GroupDocs.Signature لـ Java.
        {{< landing/code title="Enchance وثيقة PDF مع رمز الاستجابة السريعة">}}
        ```java {style=abap}
        // قم بتحميل المستند للتوقيع
        Signature signature = new Signature("file_to_sign.pdf");
        
        // قم بإنشاء خيارات رمز الاستجابة السريعة بنص محدد مسبقًا
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // قم بتكوين نوع ترميز رمز الاستجابة السريعة وموضعه على الصفحة
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // قم بتوقيع المستند واحفظه كملف النتيجة
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "استخدم التوقيع الرقمي لحماية DOCX"
      content: |
        يمكنك [حماية مستند](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) باستخدام التوقيعات الشخصية أو توقيعات الشركة المخزنة كشهادات رقمية. لا يمكن تغيير المستندات المؤمنة بالشهادة دون إبطال التوقيع.
        {{< landing/code title="استخدم التوقيع الرقمي لحماية DOCX">}}
        ```java {style=abap}   
        // قم بتحميل المستند ليتم توقيعه رقميًا
        Signature signature = new Signature("file_to_sign.pdf");
        
        // حدد خيارات التوقيع الرقمي وقم بتوفير المسار إلى ملف الشهادة
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // قم بتعيين كلمة مرور الشهادة
        options.setPassword("1234567890");

        // قم بتوقيع المستند وحفظه في المسار المطلوب
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
