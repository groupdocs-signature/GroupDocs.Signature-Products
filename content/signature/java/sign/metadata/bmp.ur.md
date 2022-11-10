---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Bmp
productName: Java
lang: ur
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Bmp for Java

############################# Head ############################
head_title: "Java کے ذریعے Bmp دستاویزات میں میٹا ڈیٹا الیکٹرانک دستخط شامل کریں"
head_description: "Java کوڈ کی چند سطروں کا استعمال کرتے ہوئے اپنے Bmp دستاویزات کے اندر چھپے ہوئے الیکٹرانک دستخطوں کے طور پر میٹا ڈیٹا استعمال کریں۔ میٹا ڈیٹا کی معلومات کے ساتھ اپنے کاروباری دستاویزات اور فائلوں پر ای سائن کرنے کے لیے GroupDocs Document Signature API کا استعمال کریں۔"

############################# Header ############################
title: "Java کے ذریعے Bmp دستاویز کے لیے میٹا ڈیٹا الیکٹرانک دستخط سادہ اور استعمال میں آسان ہیں!"
description: "پوشیدہ میٹا ڈیٹا اندراجات کے ساتھ اپنے Bmp دستاویزات اور معاہدوں پر دستخط کریں۔ پی ڈی ایف، ایم ایس ورڈ دستاویزات، ایم ایس ایکسل ورک بک، ایم ایس پاورپوائنٹ پریزنٹیشنز اور مختلف امیج فارمیٹس کے لیے بغیر کسی پریشانی اور اضافی کوڈنگ کے میٹا ڈیٹا بنائیں۔"
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
    title: "GroupDocs.Signature for Java میٹا ڈیٹا دستخط API کے بارے میں"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ڈیجیٹل دستاویزات کے ای سائننگ کے لیے ایک مقبول API ہے۔ دستخط جیسے متن، تصاویر، ڈیجیٹل سرٹیفکیٹ، بارکوڈ، کیو آر کوڈ، ڈاک ٹکٹ یا میٹا ڈیٹا دستیاب ہیں۔ دستخط PDFs، MS Word دستاویزات، MS Excel ورک بک، MS پاورپوائنٹ پریزنٹیشنز، Adobe Photoshop فائلوں اور مختلف امیج فارمیٹس پر رکھے جا سکتے ہیں۔ صارفین اپنے دستاویز پر دستخط کر سکتے ہیں اور ان دستاویزات پر رکھے گئے ای دستخطوں کو اپ ڈیٹ، تلاش، تصدیق، حذف یا پیش نظارہ کر سکتے ہیں۔ مزید یہ کہ دستخطوں کی تخصیص کے لیے بہت ساری صلاحیتیں فراہم کی گئی ہیں۔
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java میں Metadata کے ساتھ Bmp پر دستخط کرنے کے مراحل"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) جلد اور آسانی سے Metadata دستخطوں کے ساتھ Bmp دستاویزات پر دستخط کرنے کی صلاحیت فراہم کرتا ہے۔
        
        * دستخط کلاس کی ایک مثال بنائیں جو کہ Bmp فائل کو پاتھ یا میموری اسٹریم کے طور پر دستخط کرنے کے لیے فراہم کرتی ہے۔
        * SignOptions کلاس کو فوری بنائیں اور تمام مطلوبہ ڈیٹا سیٹ کریں۔
        * Signature.Sign() طریقہ پاس کرنے کے آؤٹ پٹ Bmp فائل یا میموری اسٹریم کو استعمال کریں

    title_right: " سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Signature for Java تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔

        * آپریٹنگ سسٹم: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        * ترقی کے ماحول: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * تازہ ترین GroupDocs.Signature for Java حاصل کریں [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) سے
         
    code: |
        ```java    
                
        // Set up input Bmp file
        String filePath = "input.bmp";
        // Set up output file
        String outputFilePath = "output.bmp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // Specify different Metadata Signatures and add them to options signature collection
        // set start id
        int imgsMetadataId = 41996;
        // setup int value
        ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
        options.getSignatures().add(mdSign_DocId);
        // setup Author property
        ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
        options.getSignatures().add(mdSign_Author);
        // setup data of sign date
        ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, new Date()); // DateTime
        options.getSignatures().add(mdSign_Date);
        // setup double
        ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456); //decimal value
        options.getSignatures().add(mdSign_Amnt);

        // sign Bmp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Metadata لائیو ڈیمو کے ساتھ Bmp دستاویزات پر دستخط کرنا"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ویب سائٹ پر جا کر ابھی مختلف دستخطوں کے ساتھ Bmp فائل پر دستخط کریں۔ مفت آن لائن ڈیمو آپ کا منتظر ہے۔          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java کے لیے دیگر تعاون یافتہ Metadata دستخط"
    content: |
        "آپ دستخط کی دیگر اقسام کے ساتھ بھی Bmp پر دستخط کر سکتے ہیں۔ براہ کرم نیچے دی گئی فہرست دیکھیں۔"
    format: 
       
       
back_to_top:
    enable: true
---