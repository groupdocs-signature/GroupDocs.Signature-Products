---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:51
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: "NET و Java و Cloud APIs وتطبيقات توقيع المستندات عبر الإنترنت"
head_description: "احصل على حل التوقيع الإلكتروني الشامل للمستند للتطبيقات المستندة إلى .NET و Java والتطبيقات المستندة إلى السحابة. قم بتوقيع تنسيقات المستندات الشائعة عبر الإنترنت باستخدام ميزة السحب والإفلات البسيطة"

############################# Header ############################
title: "التوقيع على وثائق<br>عبر .NET API"
description: "قم بتوقيع المستندات والصور الرقمية على أي نظام أساسي باستخدام واجهات برمجة التطبيقات المرنة والحلول القائمة على التطبيقات للمبرمجين والمستخدمين النهائيين."
words:
  for: "ل"

actions:
  main: "تحميل نوجيت مجانا"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "الترخيص"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "على استعداد للبدء؟"
  description: "جرب ميزات GroupDocs.Signature مجانًا أو اطلب ترخيصًا"

release:
  title: "تم إصدار الإصدار {0}."
  notes: "ترى ما هو الجديد"
  downloads: "التحميلات"

code:
  title: "تسجيل ملفات PDF في C#"
  more: "مزيد من الأمثلة"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // حدد مستند PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // تقديم النص
        var options = new TextSignOptions("John Smith")
        {
            // ضبط اللون
            ForeColor = Color.Red
        };
        // قم بتوقيع الوثيقة وحفظها في ملف
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.نظرة عامة على التوقيع"
  description: "واجهة برمجة التطبيقات (API) لتنفيذ توقيع المستندات والعمليات ذات الصلة في تطبيقات .NET"
  features:
    # feature loop
    - title: "إضافة التوقيعات إلى مستندات العمل في C#"
      content: "توقيع المستندات: باستخدام GroupDocs.Signature for .NET، يمكنك إضافة أنواع مختلفة من التوقيعات، مثل النصوص والصور والرموز الشريطية والشهادات الرقمية، إلى مستندات PDF وOffice. تسمح لك واجهة برمجة التطبيقات (API) هذه بتوقيع مستنداتك باستخدام أي نوع بيانات تقريبًا، بما في ذلك البيانات التعريفية المخفية."

    # feature loop
    - title: "معالجة المستندات الموقعة"
      content: "معالجة إضافية: يمكنك إجراء عمليات قوية على المستندات الموقعة باستخدام GroupDocs.Signature. يتضمن ذلك البحث عن التوقيعات الموجودة ضمن مستندات الأعمال والتحقق منها باستخدام معايير محددة. بالإضافة إلى ذلك، يمكنك استرداد معلومات المستند ومعاينة الصفحات من خلال .NET API."

    # feature loop
    - title: "تخصيص النتائج"
      content: "يوفر GroupDocs.Signature for .NET خيارات تخصيص واسعة النطاق. يمكنك وضع التوقيعات بدقة في أي مكان على صفحة المستند وضبط مظهرها باستخدام مجموعة متنوعة من الإعدادات. علاوة على ذلك، تدعم واجهة برمجة التطبيقات هذه حفظ المستندات التي تمت معالجتها في مجموعة واسعة من التنسيقات المدعومة."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلالية المنصة"
  description: "يدعم GroupDocs.Signature for .NET أنظمة التشغيل وأطر العمل ومديري الحزم التالية"
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
    يدعم GroupDocs.Signature for .NET العمليات باستخدام [تنسيقات الملفات] التالية (https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "توقيع ملفات PDF ومستندات Office والصور بسرعة ودقة"

  items:
    # feature loop
    - icon: "merge"
      title: "توقيع الوثيقة"
      content: "أضف واحدًا أو أكثر من أنواع التوقيعات المدعومة بدقة في أي موضع محدد في مستندات العمل."

    # feature loop
    - icon: "split"
      title: "تخصيص التوقيعات"
      content: "استخدم ميزات مثل اللون والخط والحدود والتدوير وما إلى ذلك لتكوين مظهر التوقيعات."

    # feature loop
    - icon: "move"
      title: "حماية كلمة المرور للوثيقة"
      content: "تأمين أنواع معينة من المستندات عن طريق تعيين كلمة مرور بعد التوقيع."

    # feature loop
    - icon: "remove"
      title: "الحماية من التغييرات"
      content: "منع إجراء تغييرات على مستندات العمل المهمة بعد إلحاق توقيع بشهادة رقمية."

    # feature loop
    - icon: "rotate"
      title: "تحويل الملفات الموقعة إلى صيغ أخرى"
      content: "تحويل الملفات الموقعة إلى التنسيقات المطلوبة، مثل حفظ مستند Word كملف PDF."

    # feature loop
    - icon: "swap"
      title: "استخراج معاينات الصفحة"
      content: "استخرج الصفحات من المستندات الموقعة كصور فردية للمعالجة المستقبلية."

    # feature loop
    - icon: "extract"
      title: "البحث عن التوقيع في المستندات"
      content: "استرجاع المعلومات حول التوقيعات المضافة مسبقًا في مستندات محددة."

    # feature loop
    - icon: "orientation"
      title: "التحقق من صحة الوثائق الموقعة"
      content: "تحقق من التوقيع الصحيح للمستندات باستخدام ميزات التحقق من الصحة."

    # feature loop
    - icon: "preview"
      title: "تحديث أو حذف التوقيعات"
      content: "يمكنك بسهولة تغيير موضع توقيعات محددة على الصفحة، أو تعديل نصها، أو حذفها دون أي مشاكل."

############################# Code samples ############################
code_samples:
  enable: true
  title: "عينات التعليمات البرمجية"
  description: "تستخدم بعض حالات GroupDocs.Signature النموذجية لعمليات .NET"
  items:
    # code sample loop
    - title: "إضافة رمز الاستجابة السريعة إلى PDF"
      content: |
        يمكن أن تؤدي إضافة [رموز QR](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) إلى صفحات محددة من مستندات PDF إلى تحسين العمليات التجارية. فيما يلي مثال لكيفية إضافة رمز الاستجابة السريعة باستخدام GroupDocs.Signature.
        {{< landing/code title="كيفية وضع رمز الاستجابة السريعة على PDF.">}}
        ```csharp {style=abap}
        // قم بتحميل المستند للتوقيع
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // قم بإنشاء خيارات رمز الاستجابة السريعة بنص محدد مسبقًا
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // قم بتكوين نوع ترميز رمز الاستجابة السريعة وموضعه على الصفحة
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // قم بتوقيع المستند واحفظه كملف النتيجة
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "حماية مستند DOCX باستخدام شهادة رقمية"
      content: |
        يمكنك [حماية مستند](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) باستخدام التوقيعات الشخصية أو توقيعات الشركة المخزنة كشهادات رقمية. ولا يمكن تعديل هذه المستندات المحمية دون إبطال التوقيع.
        {{< landing/code title="إليك كيفية ضمان سلامة المستند.">}}
        ```csharp {style=abap}   
        // قم بتحميل المستند ليتم توقيعه رقميًا
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // حدد خيارات التوقيع الرقمي وقم بتوفير المسار إلى ملف الشهادة
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // قم بتعيين كلمة مرور الشهادة
                Password = "1234567890"
            };
            // قم بتوقيع المستند وحفظه في المسار المطلوب
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

############################# Reviews ############################
# reviews:
# enable: true
# title: "{reviews.title}"
# description: "{reviews.description}"

# items:
#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_1.content}"
#     author: "{reviews.review_1.author}"
#     company: "{reviews.review_1.company}"

#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_2.content}"
#     author: "{reviews.review_2.author}"
#     company: "{reviews.review_2.company}"
---
