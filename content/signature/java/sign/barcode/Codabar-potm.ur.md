---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Codabar
fileformat: Potm
productName: Java
lang: ur
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Potm for Java

############################# Head ############################
head_title: "Java میں Codabar بارکوڈ کے ساتھ eSign Potm دستاویز"
head_description: "Codabar بارکوڈ دستخط بنائیں اور کوڈ کی دو سطروں کا استعمال کرتے ہوئے Java کے ساتھ Potm دستاویز پر رکھیں۔ مختلف فائل فارمیٹس پر دستخط کرنے کے لیے GroupDocs Document Signature API استعمال کریں۔"

############################# Header ############################
title: "Java میں Potm دستاویز کے لیے Codabar بارکوڈ دستخط بنائیں"
description: "اپنے Potm کاروباری دستاویزات پر Codabar بارکوڈ کے ساتھ دستخط کریں۔ دستخط کے اختیارات ترتیب دینے کے لیے کوڈ کی چند سطروں کے ساتھ بار کوڈ دستخط جلدی اور آسانی سے بنائیں۔"
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
    title_left: "Java میں Barcode کے ساتھ Potm پر دستخط کرنے کے مراحل"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) جلد اور آسانی سے Barcode دستخطوں کے ساتھ Potm دستاویزات پر دستخط کرنے کی صلاحیت فراہم کرتا ہے۔
        
        * دستخط کلاس کی ایک مثال بنائیں جو کہ Potm فائل کو پاتھ یا میموری اسٹریم کے طور پر دستخط کرنے کے لیے فراہم کرتی ہے۔
        * SignOptions کلاس کو فوری بنائیں اور تمام مطلوبہ ڈیٹا سیٹ کریں۔
        * Signature.Sign() طریقہ پاس کرنے کے آؤٹ پٹ Potm فائل یا میموری اسٹریم کو استعمال کریں

    title_right: " سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Signature for Java تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔

        * آپریٹنگ سسٹم: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        * ترقی کے ماحول: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * تازہ ترین GroupDocs.Signature for Java حاصل کریں [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) سے
         
    code: |
        ```java    
                
        // Set up input Potm file
        String filePath = "input.potm";
        // Set up output file
        String outputFilePath = "output.potm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Codabar);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Potm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode لائیو ڈیمو کے ساتھ Potm دستاویزات پر دستخط کرنا"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ویب سائٹ پر جا کر ابھی مختلف دستخطوں کے ساتھ Potm فائل پر دستخط کریں۔ مفت آن لائن ڈیمو آپ کا منتظر ہے۔

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Codabar Barcode"
          content: |
            کوڈابار ایک لکیری بارکوڈ علامت ہے جو کہ FedEx ایئر بلز اور بلڈ بینک فارم جیسے کثیر حصے کی شکلوں کے لیے ڈاٹ میٹرکس پرنٹرز پر پرنٹ ہونے پر بھی درست طریقے سے پڑھنے کے لیے ڈیزائن کیا گیا تھا۔
          characterset: |
             عددی ہندسے (0-9) اور خصوصی حروف $/-:+۔
          textcapacity: |
             کوئی خاص پابندیاں نہیں۔
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAD0AAABGCAYAAAB/h5zrAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAK2SURBVHhe7c9BagQBDAPB/f+nNxDQpUCOfc1MQx8khMGf7wN5n34K79NP4X36KYxPfz6fX0OyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2su48EiyyrZvWeXay7jwSLLKtm9Z5drLuPBIssq2b1nl2svfi3/I+/RTeJ9+Cg98+vv9AViQgD/8yuhqAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java کے لیے دیگر تعاون یافتہ Barcode دستخط"
    content: |
        "آپ دستخط کی دیگر اقسام کے ساتھ بھی Potm پر دستخط کر سکتے ہیں۔ براہ کرم نیچے دی گئی فہرست دیکھیں۔"
    format: 
        
       
back_to_top:
    enable: true
---