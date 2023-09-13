---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:52
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET، Java، Cloud APIs اور آن لائن دستاویز دستخطی ایپس"
head_description: ".NET، Java اور کلاؤڈ بیسڈ ایپلی کیشنز کے لیے آل ان ون دستاویز کا ای دستخطی حل حاصل کریں۔ سادہ ڈریگ اینڈ ڈراپ فیچر کا استعمال کرتے ہوئے عام دستاویز کے فارمیٹس پر دستخط کریں۔"

############################# Header ############################
title: "دستاویزات پر دستخط کریں۔<br>.NET API کے ذریعے"
description: "پروگرامرز اور اختتامی صارفین کے لیے ہمارے لچکدار APIs اور ایپ پر مبنی حل کا استعمال کرتے ہوئے کسی بھی پلیٹ فارم پر ڈیجیٹل دستاویزات اور تصاویر پر دستخط کریں۔"
words:
  for: "کے لیے"

actions:
  main: "مفت نیو گیٹ ڈاؤن لوڈ"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "لائسنسنگ"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "شروع کرنے کے لیے تیار ہیں؟"
  description: "GroupDocs.Signature کی خصوصیات مفت میں آزمائیں یا لائسنس کی درخواست کریں۔"

release:
  title: "ورژن {0} جاری کیا گیا۔"
  notes: "دیکھیں کہ نیا کیا ہے۔"
  downloads: "ڈاؤن لوڈ"

code:
  title: "C# میں پی ڈی ایف فائلوں پر دستخط کریں"
  more: "مزید مثالیں۔"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // پی ڈی ایف دستاویز کو منتخب کریں۔
    using (Signature signature = new Signature("sample.pdf"))
    {
        // متن فراہم کریں۔
        var options = new TextSignOptions("John Smith")
        {
            // رنگ سیٹ کریں۔
            ForeColor = Color.Red
        };
        // دستاویز پر دستخط کریں اور فائل میں محفوظ کریں۔
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature کا جائزہ"
  description: ".NET ایپلی کیشنز میں دستاویز پر دستخط کرنے اور متعلقہ کارروائیوں کے لیے API"
  features:
    # feature loop
    - title: "C# میں کاروباری دستاویزات میں دستخط شامل کرنا"
      content: "دستاویزات پر دستخط کرنا: .NET کے لیے GroupDocs.Signature کے ساتھ، آپ پی ڈی ایف اور آفس دستاویزات میں متن، تصاویر، بارکوڈز، اور ڈیجیٹل سرٹیفکیٹس جیسے مختلف قسم کے دستخط شامل کر سکتے ہیں۔ یہ API آپ کو اپنے دستاویزات پر تقریباً کسی بھی قسم کے ڈیٹا کے ساتھ دستخط کرنے کی اجازت دیتا ہے، بشمول پوشیدہ میٹا ڈیٹا۔"

    # feature loop
    - title: "دستخط شدہ دستاویزات پر کارروائی ہو رہی ہے۔"
      content: "اضافی پروسیسنگ: آپ GroupDocs.Signature کا استعمال کرتے ہوئے دستخط شدہ دستاویزات پر طاقتور آپریشن کر سکتے ہیں۔ اس میں کاروباری دستاویزات میں موجودہ دستخطوں کی تلاش اور مخصوص معیارات کا استعمال کرتے ہوئے ان کی تصدیق کرنا شامل ہے۔ مزید برآں، آپ اس .NET API کے ذریعے دستاویز کی معلومات اور پیش نظارہ صفحات کو بازیافت کرسکتے ہیں۔"

    # feature loop
    - title: "نتائج کو حسب ضرورت بنانا"
      content: ".NET کے لیے GroupDocs.Signature حسب ضرورت کے وسیع اختیارات پیش کرتا ہے۔ آپ دستاویز کے صفحہ پر کہیں بھی دستخطوں کو درست طریقے سے رکھ سکتے ہیں اور مختلف ترتیبات کا استعمال کرتے ہوئے ان کی ظاہری شکل کو ایڈجسٹ کر سکتے ہیں۔ مزید برآں، یہ API پروسیس شدہ دستاویزات کو معاون فارمیٹس کی وسیع رینج میں محفوظ کرنے کی حمایت کرتا ہے۔"

############################# Platforms ############################
platforms:
  enable: true
  title: "پلیٹ فارم کی آزادی"
  description: ".NET کے لیے GroupDocs.Signature درج ذیل آپریٹنگ سسٹمز، فریم ورکس اور پیکیج مینیجرز کو سپورٹ کرتا ہے۔"
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
    .NET کے لیے GroupDocs.Signature درج ذیل [فائل فارمیٹس](https://docs.groupdocs.com/signature/net/supported-document-formats/) کے ساتھ کارروائیوں کی حمایت کرتا ہے۔
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
  description: "پی ڈی ایف، آفس دستاویزات، اور امیجز پر تیزی سے اور درست طریقے سے دستخط کرنا"

  items:
    # feature loop
    - icon: "merge"
      title: "دستاویز پر دستخط"
      content: "کاروباری دستاویزات پر کسی بھی مخصوص پوزیشن پر درست طریقے سے ایک یا متعدد معاون قسم کے دستخط شامل کریں۔"

    # feature loop
    - icon: "split"
      title: "دستخطوں کو حسب ضرورت بنائیں"
      content: "دستخطوں کی ظاہری شکل کو ترتیب دینے کے لیے رنگ، فونٹ، بارڈر، گردش وغیرہ جیسی خصوصیات کا استعمال کریں۔"

    # feature loop
    - icon: "move"
      title: "دستاویز پاس ورڈ کی حفاظت"
      content: "دستخط کرنے کے بعد پاس ورڈ ترتیب دے کر دستاویز کی مخصوص اقسام کو محفوظ کریں۔"

    # feature loop
    - icon: "remove"
      title: "تبدیلیوں سے تحفظ"
      content: "ڈیجیٹل سرٹیفکیٹ کے ساتھ دستخط شامل کرنے کے بعد اہم کاروباری دستاویزات میں تبدیلیوں کو روکیں۔"

    # feature loop
    - icon: "rotate"
      title: "دستخط شدہ فائلوں کو دوسرے فارمیٹس میں تبدیل کریں۔"
      content: "دستخط شدہ فائلوں کو مطلوبہ فارمیٹس میں تبدیل کریں، جیسے کہ ورڈ دستاویز کو پی ڈی ایف کے طور پر محفوظ کرنا۔"

    # feature loop
    - icon: "swap"
      title: "صفحہ پیش نظارہ نکالیں۔"
      content: "مستقبل کی پروسیسنگ کے لیے انفرادی تصاویر کے طور پر دستخط شدہ دستاویزات سے صفحات نکالیں۔"

    # feature loop
    - icon: "extract"
      title: "دستاویزات میں دستخط تلاش کریں۔"
      content: "مخصوص دستاویزات میں پہلے شامل کیے گئے دستخطوں کے بارے میں معلومات حاصل کریں۔"

    # feature loop
    - icon: "orientation"
      title: "دستخط شدہ دستاویزات کی توثیق کریں۔"
      content: "توثیق کی خصوصیات کا استعمال کرتے ہوئے دستاویزات پر صحیح دستخط کی تصدیق کریں۔"

    # feature loop
    - icon: "preview"
      title: "دستخطوں کو اپ ڈیٹ کریں یا حذف کریں۔"
      content: "کسی صفحہ پر مخصوص دستخطوں کو آسانی سے جگہ دیں، ان کے متن میں ترمیم کریں، یا بغیر کسی مسئلے کے انہیں حذف کریں۔"

############################# Code samples ############################
code_samples:
  enable: true
  title: "کوڈ کے نمونے"
  description: "کچھ .NET آپریشنز کے لیے مخصوص GroupDocs.Signature کے کیسز استعمال کرتے ہیں۔"
  items:
    # code sample loop
    - title: "پی ڈی ایف میں کیو آر کوڈ شامل کریں۔"
      content: |
        پی ڈی ایف دستاویزات کے مخصوص صفحات میں [QR-codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) شامل کرنا کاروباری عمل کو بڑھا سکتا ہے۔ ذیل میں GroupDocs.Signature کا استعمال کرتے ہوئے QR کوڈ شامل کرنے کے طریقے کی ایک مثال ہے۔
        {{< landing/code title="کیو آر کوڈ کو پی ڈی ایف میں کیسے ڈالیں۔">}}
        ```csharp {style=abap}
        // دستخط کرنے کے لیے دستاویز لوڈ کریں۔
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // پہلے سے طے شدہ متن کے ساتھ QR کوڈ کے اختیارات بنائیں
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // QR کوڈ انکوڈنگ کی قسم اور صفحہ پر پوزیشن کو ترتیب دیں۔
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // دستاویز پر دستخط کریں اور اسے رزلٹ فائل کے طور پر محفوظ کریں۔
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "ڈیجیٹل سرٹیفکیٹ کا استعمال کرتے ہوئے DOCX دستاویز کی حفاظت کرنا"
      content: |
        آپ ڈیجیٹل سرٹیفکیٹس کے بطور محفوظ کردہ ذاتی یا کارپوریٹ دستخطوں کا استعمال کرتے ہوئے [دستاویز کی حفاظت](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) کر سکتے ہیں۔ اس طرح کے محفوظ دستاویزات میں دستخط کو باطل کیے بغیر ترمیم نہیں کی جاسکتی ہے۔
        {{< landing/code title="دستاویز کی سالمیت کو یقینی بنانے کا طریقہ یہاں ہے۔">}}
        ```csharp {style=abap}   
        // ڈیجیٹل طور پر دستخط کرنے کے لیے دستاویز لوڈ کریں۔
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // ڈیجیٹل دستخط کرنے کے اختیارات کی وضاحت کریں اور سرٹیفکیٹ فائل کا راستہ فراہم کریں۔
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // سرٹیفکیٹ پاس ورڈ سیٹ کریں۔
                Password = "1234567890"
            };
            // دستاویز پر دستخط کریں اور اسے مطلوبہ راستے پر محفوظ کریں۔
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
