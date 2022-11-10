---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Code39
fileformat: Xltx
productName: Java
lang: ur
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Xltx for Java

############################# Head ############################
head_title: "Java میں Code39 بارکوڈ کے ساتھ eSign Xltx دستاویز"
head_description: "Code39 بارکوڈ دستخط بنائیں اور کوڈ کی دو سطروں کا استعمال کرتے ہوئے Java کے ساتھ Xltx دستاویز پر رکھیں۔ مختلف فائل فارمیٹس پر دستخط کرنے کے لیے GroupDocs Document Signature API استعمال کریں۔"

############################# Header ############################
title: "Java میں Xltx دستاویز کے لیے Code39 بارکوڈ دستخط بنائیں"
description: "اپنے Xltx کاروباری دستاویزات پر Code39 بارکوڈ کے ساتھ دستخط کریں۔ دستخط کے اختیارات ترتیب دینے کے لیے کوڈ کی چند سطروں کے ساتھ بار کوڈ دستخط جلدی اور آسانی سے بنائیں۔"
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
    title: "GroupDocs.Signature for Java بارکوڈ دستخط API کے بارے میں۔"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) بارکوڈ کی اقسام جیسے UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN کا استعمال کرتے ہوئے ڈیجیٹل دستاویزات کے ای-سائننگ کا انتظام کرنے کے لیے ایک تیز اور آسان API ہے۔ ، ITF14 اور بہت سے دوسرے۔ صارفین آسانی سے مطلوبہ متن فراہم کرنے والے بارکوڈز بنا سکتے ہیں اور انہیں پی ڈی ایف، مائیکروسافٹ آفس ورڈز ڈاکومنٹس، مائیکروسافٹ آفس ایکسل ورک بک، ایم ایس پاورپوائنٹ پریزنٹیشنز، ایڈوب فوٹوشاپ فائلز اور مختلف امیج فارمیٹس پر لگا سکتے ہیں۔ دستاویزات میں رکھے گئے بارکوڈز کو اپ ڈیٹ، تلاش، تصدیق، حذف یا پیش نظارہ کیا جا سکتا ہے۔ مزید یہ کہ بارکوڈز کی تخصیص کی حمایت کی جاتی ہے۔
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java میں Barcode کے ساتھ Xltx پر دستخط کرنے کے مراحل"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) جلد اور آسانی سے Barcode دستخطوں کے ساتھ Xltx دستاویزات پر دستخط کرنے کی صلاحیت فراہم کرتا ہے۔
        
        * دستخط کلاس کی ایک مثال بنائیں جو کہ Xltx فائل کو پاتھ یا میموری اسٹریم کے طور پر دستخط کرنے کے لیے فراہم کرتی ہے۔
        * SignOptions کلاس کو فوری بنائیں اور تمام مطلوبہ ڈیٹا سیٹ کریں۔
        * Signature.Sign() طریقہ پاس کرنے کے آؤٹ پٹ Xltx فائل یا میموری اسٹریم کو استعمال کریں

    title_right: " سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Signature for Java تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔

        * آپریٹنگ سسٹم: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        * ترقی کے ماحول: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * تازہ ترین GroupDocs.Signature for Java حاصل کریں [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) سے
         
    code: |
        ```java    
                
        // Set up input Xltx file
        String filePath = "input.xltx";
        // Set up output file
        String outputFilePath = "output.xltx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Code39);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Xltx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode لائیو ڈیمو کے ساتھ Xltx دستاویزات پر دستخط کرنا"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ویب سائٹ پر جا کر ابھی مختلف دستخطوں کے ساتھ Xltx فائل پر دستخط کریں۔ مفت آن لائن ڈیمو آپ کا منتظر ہے۔

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Code39 Barcode"
          content: |
            کوڈ 39 (جسے الفا39، کوڈ 3 آف 9، کوڈ 3/9، ٹائپ 39، یو ایس ایس کوڈ 39، یا USD-3 بھی کہا جاتا ہے) ایک متغیر لمبائی، مجرد بارکوڈ علامت ہے۔
          characterset: |
             عددی ہندسے (0-9) اور بڑے حروف (A-Z) اور متعدد خصوصی حروف (-، .، $، /، +، %، اور space)۔
          textcapacity: |
             کوئی خاص پابندیاں نہیں۔
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java کے لیے دیگر تعاون یافتہ Barcode دستخط"
    content: |
        "آپ دستخط کی دیگر اقسام کے ساتھ بھی Xltx پر دستخط کر سکتے ہیں۔ براہ کرم نیچے دی گئی فہرست دیکھیں۔"
    format: 
        
       
back_to_top:
    enable: true
---