---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Xltx
productName: Java
lang: ur
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Xltx for Java

############################# Head ############################
head_title: "Java میں Pharmacode بارکوڈ کے ساتھ eSign Xltx دستاویز"
head_description: "Pharmacode بارکوڈ دستخط بنائیں اور کوڈ کی دو سطروں کا استعمال کرتے ہوئے Java کے ساتھ Xltx دستاویز پر رکھیں۔ مختلف فائل فارمیٹس پر دستخط کرنے کے لیے GroupDocs Document Signature API استعمال کریں۔"

############################# Header ############################
title: "Java میں Xltx دستاویز کے لیے Pharmacode بارکوڈ دستخط بنائیں"
description: "اپنے Xltx کاروباری دستاویزات پر Pharmacode بارکوڈ کے ساتھ دستخط کریں۔ دستخط کے اختیارات ترتیب دینے کے لیے کوڈ کی چند سطروں کے ساتھ بار کوڈ دستخط جلدی اور آسانی سے بنائیں۔"
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
        options.setEncodeType(BarcodeTypes.Pharmacode);

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
          title: "About Pharmacode Barcode"
          content: |
            فارما کوڈ، جسے فارماسیوٹیکل بائنری کوڈ کے نام سے بھی جانا جاتا ہے، ایک بارکوڈ معیار ہے، جو فارماسیوٹیکل انڈسٹری میں پیکنگ کنٹرول سسٹم کے طور پر استعمال ہوتا ہے۔
          characterset: |
             عددی ہندسے (0-9)۔
          textcapacity: |
             3 سے 131070 تک صرف ایک عدد عدد کی نمائندگی کرتا ہے۔
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

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