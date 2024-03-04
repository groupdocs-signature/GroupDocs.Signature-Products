---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ur
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
head_title: ".NET، Java، Cloud APIs اور آن لائن دستاویز دستخطی ایپس"
head_description: ".NET، Java اور کلاؤڈ بیسڈ ایپلی کیشنز کے لیے آل ان ون دستاویز کا ای دستخطی حل حاصل کریں۔ سادہ ڈریگ اینڈ ڈراپ فیچر کا استعمال کرتے ہوئے عام دستاویز کے فارمیٹس پر دستخط کریں۔"

############################# Header ############################
title: "دستاویزات پر دستخط کریں۔<br>Node.js API کے ساتھ"
description: "پروگرامرز اور اختتامی صارفین کے لیے ہمارے لچکدار APIs اور ایپ پر مبنی حل کا استعمال کرتے ہوئے کسی بھی پلیٹ فارم پر ڈیجیٹل دستاویزات اور تصاویر پر دستخط کریں۔"
words:
  for: "کے لیے"

actions:
  main: "NPM سے ڈاؤن لوڈ کریں۔"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "لائسنسنگ"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "شروع کرنے کے لیے تیار ہیں؟"
  description: "GroupDocs.Signature کی خصوصیات مفت میں آزمائیں یا لائسنس کی درخواست کریں۔"

release:
  title: "ورژن {0} جاری کیا گیا۔"
  notes: "دیکھیں کہ نیا کیا ہے۔"
  downloads: "ڈاؤن لوڈ"

code:
  title: "Node.js کے ذریعے پی ڈی ایف پر دستخط کرنا"
  more: "مزید مثالیں۔"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // پی ڈی ایف دستاویز کو منتخب کریں۔
    let signature = new Signature("sample.pdf");
    
    // متن فراہم کریں۔
    let options = new TextSignOptions("John Smith");
    
    // رنگ سیٹ کریں۔
    options.ForeColor = Color.Red;
    
    // دستاویز پر دستخط کریں اور فائل میں محفوظ کریں۔
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature کا جائزہ"
  description: "دستاویزات پر دستخط کرنے والی لائبریری جو Node.js ایپلی کیشنز میں استعمال کے لیے تیار ہے۔"
  features:
    # feature loop
    - title: "Node.js کے ساتھ کاروباری دستاویزات کے لیے ڈیجیٹل دستخطوں کا حل"
      content: "GroupDocs.Signature for Node.js via Java PDF، آفس دستاویزات اور تصاویر کے لیے ڈیجیٹل دستخطی اختیارات کا ایک جامع سیٹ پیش کرتا ہے۔ متن، بارکوڈ، تصاویر، ڈیجیٹل سرٹیفکیٹ اور میٹا ڈیٹا دستیاب ہیں۔ ہموار دستاویز کی پروسیسنگ کارکردگی کو یقینی بناتی ہے۔"

    # feature loop
    - title: "دستخط شدہ دستاویزات کی اعلی درجے کی ہیرا پھیری"
      content: "GroupDocs.Signature آپ کو دستخط شدہ دستاویزات پر کارروائی کرنے کا اختیار دیتا ہے۔ مختلف معیارات کا استعمال کرتے ہوئے دستخطوں کی تلاش اور توثیق کریں۔ مزید برآں، تفصیلی دستاویز کی معلومات نکالیں یا صفحات کی پیش نظارہ تصاویر بنائیں۔"

    # feature loop
    - title: "متنوع آؤٹ پٹ فارمیٹس"
      content: "ہمارا حل دستخط شدہ دستاویزات کے آؤٹ پٹ فارمیٹ پر وسیع کنٹرول فراہم کرتا ہے۔ کسی بھی صفحہ پر دستخطوں کو درست طریقے سے رکھیں اور ان کی ظاہری شکل کو حسب ضرورت بنائیں۔ دستخط شدہ دستاویزات کو متعدد معاون فارمیٹس میں محفوظ کریں اور اختیاری طور پر پاس ورڈز کے ساتھ محفوظ کریں۔"

############################# Platforms ############################
platforms:
  enable: true
  title: "پلیٹ فارم کی آزادی"
  description: "GroupDocs.Signature for Node.js via Java مختلف آپریٹنگ سسٹمز کے ساتھ دستاویز پر کارروائی کرتا ہے۔"
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
  title: "تائید شدہ فائل فارمیٹس"
  description: |
    GroupDocs.Signature for Node.js via Java [مقبول فائل فارمیٹس](https://docs.groupdocs.com/signature/java/supported-document-formats/) کے لیے آپریشنز کی سہولت فراہم کرتا ہے۔
  groups:
    # group loop
    - color: "green"
      content: |
        ### مائیکروسافٹ آفس فارمیٹس
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### امیجز اور دیگر فارمیٹس
        * **پورٹیبل:** PDF
        * **امیجز:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **دیگر دفتری فارمیٹس:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### دیگر فارمیٹس
        * **ویب:** HTML, MHTML
        * **آرکائیوز:** ZIP, TAR, 7Z
        * **سرٹیفکیٹس:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature کی خصوصیات"
  description: "ڈیجیٹل دستخطوں کے ساتھ پی ڈی ایف، آفس دستاویزات، اور تصاویر پر دستخط کریں۔"

  items:
    # feature loop
    - icon: "sign"
      title: "کاروباری دستخط"
      content: "دستاویزات پر دستخط کرنے کے لیے مختلف قسم کے دستخط استعمال کریں۔ کسی بھی صفحہ کی جگہ پر ڈیجیٹل دستخط بالکل ٹھیک رکھیں۔"

    # feature loop
    - icon: "custom"
      title: "دستخط کی ظاہری شکل کو حسب ضرورت بنانا"
      content: "اپنے مطلوبہ نتائج کو حاصل کرنے کے لیے رنگ، فونٹ، بارڈرز، گردش اور مزید کو ایڈجسٹ کرکے دستخطوں کے بصری پہلوؤں کو تیار کریں۔"

    # feature loop
    - icon: "password"
      title: "پاس ورڈ سے محفوظ دستاویزات"
      content: "بہت سے معاون دستاویز فارمیٹس کے لیے، اضافی سیکیورٹی کے لیے پاس ورڈ کے ساتھ دستخط شدہ دستاویزات کی حفاظت کریں۔"

    # feature loop
    - icon: "protect"
      title: "غیر مجاز ترمیم کو روکنا"
      content: "ڈیجیٹل سرٹیفکیٹس کے ساتھ دستخط شدہ اہم کاروباری دستاویزات کو غیر مجاز تبدیلیوں سے محفوظ رکھیں۔"

    # feature loop
    - icon: "convert"
      title: "مطلوبہ آؤٹ پٹ فارمیٹس"
      content: "کسی بھی معاون فارمیٹ میں آسانی سے دستخط شدہ دستاویزات حاصل کریں۔ ایم ایس ورڈ دستاویزات کو آسانی سے پی ڈی ایف فارمیٹ میں تبدیل کریں۔"

    # feature loop
    - icon: "preview"
      title: "دستاویزات کا پیش نظارہ"
      content: "مستقبل کی ضروریات کے لیے انفرادی دستاویز کے صفحات کو بطور تصویر محفوظ کریں۔"

    # feature loop
    - icon: "search"
      title: "دستخط کی تلاش"
      content: "اپنے دستاویزات میں پہلے شامل کیے گئے دستخطوں کے بارے میں معلومات حاصل کریں۔"

    # feature loop
    - icon: "validate"
      title: "دستاویز کی توثیق"
      content: "کسی بھی دستاویز میں پیش کیے گئے دستخطوں کی صداقت کی تصدیق کریں۔"

    # feature loop
    - icon: "update"
      title: "دستخط کا انتظام"
      content: "کسی بھی دستاویز کے صفحے پر رکھے گئے دستخطوں کو حذف کریں، منتقل کریں، یا اس میں ترمیم کریں۔"

############################# Code samples ############################
code_samples:
  enable: true
  title: "کوڈ کے نمونے"
  description: "مثالی مثالیں عام GroupDocs.Signature for Node.js via Java آپریشنز کو ظاہر کرتی ہیں۔"
  items:
    # code sample loop
    - title: "کیو آر کوڈز کے ساتھ پی ڈی ایف کو نشان زد کریں۔"
      content: |
        پی ڈی ایف دستاویز کے مخصوص صفحات میں [بار کوڈز](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) کو شامل کرنا کاروباری عمل کو ہموار کر سکتا ہے۔ یہ سیکشن GroupDocs.Signature for Node.js via Java کا استعمال کرتے ہوئے QR کوڈ شامل کرنے کی ایک مثال فراہم کرتا ہے۔
        {{< landing/code title="کیو آر کوڈ کو پی ڈی ایف میں کیسے ڈالیں۔">}}
        ```javascript {style=abap}
        // دستخط کرنے کے لیے دستاویز لوڈ کریں۔
        let signature = new Signature("file_to_sign.pdf");
        
        // پہلے سے طے شدہ متن کے ساتھ QR کوڈ کے اختیارات بنائیں
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // QR کوڈ انکوڈنگ کی قسم اور صفحہ پر پوزیشن کو ترتیب دیں۔
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // دستاویز پر دستخط کریں اور اسے رزلٹ فائل کے طور پر محفوظ کریں۔
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "ڈیجیٹل دستخط کے ساتھ DOCX کی حفاظت کرنا"
      content: |
        ڈیجیٹل سرٹیفکیٹس پر مبنی دستخطوں کے ذریعے [اپنے دستاویزات کی حفاظت کریں](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/)۔ ڈیجیٹل دستخط مواد کی تبدیلی سے آپ کے کاروباری دستاویزات کی حفاظت کرتے ہیں۔
        {{< landing/code title="دستاویز کی سالمیت کو یقینی بنانے کا طریقہ یہاں ہے۔">}}
        ```javascript {style=abap}   
        // ڈیجیٹل طور پر دستخط کرنے کے لیے دستاویز لوڈ کریں۔
        let signature = new Signature("file_to_sign.pdf");
        
        // ڈیجیٹل دستخط کرنے کے اختیارات کی وضاحت کریں اور سرٹیفکیٹ فائل کا راستہ فراہم کریں۔
        let options = new DigitalSignOptions("certificate.pfx");

        // سرٹیفکیٹ پاس ورڈ سیٹ کریں۔
        options.Password = "1234567890";

        // دستاویز پر دستخط کریں اور اسے مطلوبہ راستے پر محفوظ کریں۔
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
