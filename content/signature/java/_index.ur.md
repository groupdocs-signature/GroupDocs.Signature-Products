---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:06
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ur
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

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
title: "دستاویزات پر دستخط کریں۔<br>جاوا API کے ذریعے"
description: "پروگرامرز اور اختتامی صارفین کے لیے ہمارے لچکدار APIs اور ایپ پر مبنی حل کا استعمال کرتے ہوئے کسی بھی پلیٹ فارم پر ڈیجیٹل دستاویزات اور تصاویر پر دستخط کریں۔"
words:
  for: "کے لیے"

actions:
  main: "مفت ماون ڈاؤن لوڈ کریں۔"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "لائسنسنگ"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "شروع کرنے کے لیے تیار ہیں؟"
  description: "GroupDocs.Signature کی خصوصیات مفت میں آزمائیں یا لائسنس کی درخواست کریں۔"

release:
  title: "ورژن {0} جاری کیا گیا۔"
  notes: "دیکھیں کہ نیا کیا ہے۔"
  downloads: "ڈاؤن لوڈ"

code:
  title: "جاوا میں پی ڈی ایف فائلوں پر دستخط کریں۔"
  more: "مزید مثالیں۔"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // پی ڈی ایف دستاویز کو منتخب کریں۔
    Signature signature = new Signature("sample.pdf");
    
    // متن فراہم کریں۔
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // دستاویز پر دستخط کریں اور فائل میں محفوظ کریں۔
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature کا جائزہ"
  description: "جاوا ایپلیکیشنز میں دستاویز پر دستخط کرنے اور متعلقہ کارروائیوں کے لیے API"
  features:
    # feature loop
    - title: "جاوا میں ڈیجیٹل دستخطوں کے ساتھ بہتر کاروباری دستاویزات"
      content: "تیز اور حسب ضرورت دستخط: GroupDocs.Signature for Java PDFs، تصاویر اور آفس دستاویزات کے لیے ڈیجیٹل دستخطی اختیارات کی ایک وسیع رینج پیش کرتا ہے۔ آپ ٹیکسٹ، بارکوڈز، کیو آر کوڈز، ڈیجیٹل سرٹیفکیٹ، تصاویر، یا پوشیدہ میٹا ڈیٹا استعمال کر سکتے ہیں۔ دستاویز کی پروسیسنگ تیز اور موثر ہے۔"

    # feature loop
    - title: "دستخط شدہ دستاویزات میں ہیرا پھیری"
      content: "اعلی درجے کی دستاویز کی پروسیسنگ میں جاوا کے لیے GroupDocs.Signature کا استعمال کرتے ہوئے دستخط شدہ دستاویزات پر طاقتور آپریشن شامل ہیں۔ آپ مختلف مفید معیارات کا استعمال کرتے ہوئے کاروباری دستاویزات میں شامل کیے گئے دستخطوں کو تلاش اور ان کی تصدیق کر سکتے ہیں۔ مزید برآں، آپ دستاویز کے بارے میں تفصیلی معلومات تک رسائی حاصل کرسکتے ہیں یا اس کے صفحات کی پیش نظارہ تصاویر حاصل کرسکتے ہیں۔"

    # feature loop
    - title: "مختلف قسم کے آؤٹ پٹ انتخاب"
      content: "مضبوط دستخط کے اختیارات آپ کو جاوا کے لیے GroupDocs.Signature کے ساتھ دستخط شدہ دستاویزات کے لیے آؤٹ پٹ کو اپنی مرضی کے مطابق کرنے کی اجازت دیتے ہیں۔ آپ کسی بھی دستاویز کے صفحہ پر کسی بھی دستخط کو درست طریقے سے پوزیشن میں رکھ سکتے ہیں اور اس کی ظاہری شکل کو مختلف طریقوں سے ترتیب دے سکتے ہیں۔ Java API دستخط شدہ کاروباری دستاویزات کو متعدد معاون فارمیٹس میں محفوظ کرنے کی حمایت کرتا ہے اور انہیں پاس ورڈ کے ساتھ محفوظ کرنے کے اختیارات فراہم کرتا ہے۔"

############################# Platforms ############################
platforms:
  enable: true
  title: "پلیٹ فارم کی آزادی"
  description: "GroupDocs.Signature for Java درج ذیل آپریٹنگ سسٹمز، فریم ورکس اور پیکیج مینیجرز کو سپورٹ کرتا ہے۔"
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
  title: "تائید شدہ فائل فارمیٹس"
  description: |
    جاوا کے لیے GroupDocs.Signature درج ذیل [فائل فارمیٹس](https://docs.groupdocs.com/signature/java/supported-document-formats/) کے ساتھ کارروائیوں کی حمایت کرتا ہے۔
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
  description: "ڈیجیٹل دستخطوں کے ساتھ PDFs، آفس دستاویزات، اور تصاویر پر دستخط کرنا"

  items:
    # feature loop
    - icon: "sign"
      title: "دستخط شامل کرنا"
      content: "کسی بھی صفحہ پر کسی بھی پوزیشن پر ٹھیک ٹھیک ڈیجیٹل دستخط رکھ کر مختلف معاون دستخطی اقسام کا استعمال کرتے ہوئے دستاویز پر دستخط کریں۔"

    # feature loop
    - icon: "custom"
      title: "نتائج کو حسب ضرورت بنانا"
      content: "مطلوبہ نتیجہ حاصل کرنے کے لیے رنگ، فونٹ، بارڈر، گردش اور دیگر خصوصیات کو ایڈجسٹ کرکے دستخط کی ظاہری شکل کو اپنی مرضی کے مطابق بنائیں۔"

    # feature loop
    - icon: "password"
      title: "پاس ورڈ کے ساتھ دستاویزات کو محفوظ کرنا"
      content: "متعدد معاون دستاویز کی اقسام کے لیے، آپ پاس ورڈ کے ساتھ دستخط شدہ دستاویز کی حفاظت کر سکتے ہیں۔"

    # feature loop
    - icon: "protect"
      title: "غیر مجاز تبدیلیوں کو روکنا"
      content: "ڈیجیٹل سرٹیفکیٹ کے ساتھ دستخط شدہ اہم کاروباری دستاویزات کو غیر مجاز ترمیم سے محفوظ رکھیں۔"

    # feature loop
    - icon: "convert"
      title: "مطلوبہ فارمیٹس میں نتائج حاصل کرنا"
      content: "کسی بھی معاون فارمیٹ میں دستخط شدہ نتائج کی فائلیں آسانی سے حاصل کریں۔ آپ ایم ایس ورڈ دستاویزات کو آسانی سے پی ڈی ایف میں بھی تبدیل کر سکتے ہیں۔"

    # feature loop
    - icon: "preview"
      title: "دستاویز کا پیش نظارہ"
      content: "کسی دستاویز کے کسی بھی صفحے کو مستقبل کی پروسیسنگ کے لیے بطور تصویر محفوظ کریں۔"

    # feature loop
    - icon: "search"
      title: "دستخطوں کی تلاش"
      content: "مخصوص دستاویزات میں پہلے شامل کیے گئے دستخطوں کے بارے میں معلومات حاصل کرنا ممکن ہے۔"

    # feature loop
    - icon: "validate"
      title: "دستاویزات کی تصدیق کرنا"
      content: "کسی بھی دستخط شدہ دستاویز پر دستخطوں کی درستگی کی توثیق کریں۔"

    # feature loop
    - icon: "update"
      title: "دستخطوں کا انتظام کرنا"
      content: "ایک بار جب دستخط کسی دستاویز کے صفحے پر رکھے جاتے ہیں، تو اسے ضرورت کے مطابق حذف، منتقل یا اپ ڈیٹ کیا جا سکتا ہے۔"

############################# Code samples ############################
code_samples:
  enable: true
  title: "کوڈ کے نمونے"
  description: "کچھ جاوا آپریشنز کے لیے مخصوص GroupDocs.Signature کے کیسز استعمال کرتے ہیں۔"
  items:
    # code sample loop
    - title: "QR-code کے ساتھ PDF دستاویز کو بہتر بنائیں"
      content: |
        پی ڈی ایف دستاویزات کے مخصوص صفحات میں [QR-codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) شامل کرکے کاروباری عمل کو بہتر بنانا قیمتی ہوسکتا ہے۔ جاوا کے لیے GroupDocs.Signature کا استعمال کرتے ہوئے QR کوڈ شامل کرنے کے طریقے کی ایک مثال موجود ہے۔
        {{< landing/code title="QR-code کے ساتھ PDF دستاویز کو بہتر بنائیں">}}
        ```java {style=abap}
        // دستخط کرنے کے لیے دستاویز لوڈ کریں۔
        Signature signature = new Signature("file_to_sign.pdf");
        
        // پہلے سے طے شدہ متن کے ساتھ QR کوڈ کے اختیارات بنائیں
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // QR کوڈ انکوڈنگ کی قسم اور صفحہ پر پوزیشن کو ترتیب دیں۔
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // دستاویز پر دستخط کریں اور اسے رزلٹ فائل کے طور پر محفوظ کریں۔
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX کی حفاظت کے لیے ڈیجیٹل دستخط استعمال کریں۔"
      content: |
        آپ ڈیجیٹل سرٹیفکیٹس کے بطور محفوظ کردہ ذاتی یا کارپوریٹ دستخطوں کا استعمال کرتے ہوئے [دستاویز کی حفاظت](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) کر سکتے ہیں۔ سرٹیفکیٹ کے ساتھ محفوظ دستاویزات کو دستخط کو باطل کیے بغیر تبدیل نہیں کیا جاسکتا۔
        {{< landing/code title="DOCX کی حفاظت کے لیے ڈیجیٹل دستخط استعمال کریں۔">}}
        ```java {style=abap}   
        // ڈیجیٹل طور پر دستخط کرنے کے لیے دستاویز لوڈ کریں۔
        Signature signature = new Signature("file_to_sign.pdf");
        
        // ڈیجیٹل دستخط کرنے کے اختیارات کی وضاحت کریں اور سرٹیفکیٹ فائل کا راستہ فراہم کریں۔
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // سرٹیفکیٹ پاس ورڈ سیٹ کریں۔
        options.setPassword("1234567890");

        // دستاویز پر دستخط کریں اور اسے مطلوبہ راستے پر محفوظ کریں۔
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
