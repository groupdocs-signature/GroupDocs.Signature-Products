---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Xlsb
productName: Java
lang: ur
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Xlsb for Java

############################# Head ############################
head_title: "Java کے ساتھ Xlsb فائل میں Image دستخط شامل کرنا"
head_description: "کوڈ کی چند سطروں کا استعمال کرتے ہوئے Java کے لیے Xlsb فائل پر Image دستخط لگائیں۔ درجنوں فائل فارمیٹس پر دستخط کرنے کے لیے GroupDocs Document Signature API کا استعمال کریں۔"

############################# Header ############################
title: "Java میں Xlsb فائلوں پر Image دستخطوں کے ساتھ دستخط کریں"
description: "Java کوڈ کی چند سطروں کے ساتھ Image دستخط کیسے شامل کریں"
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
    title: "GroupDocs.Signature for Java تصویری دستخط API کے بارے میں"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ڈیجیٹل دستاویزات کے ای سائننگ کے لیے ایک مقبول API ہے۔ دستخط جیسے متن، تصاویر، ڈیجیٹل سرٹیفکیٹ، بارکوڈ، کیو آر کوڈ، ڈاک ٹکٹ یا میٹا ڈیٹا دستیاب ہیں۔ دستخط PDFs، MS Word دستاویزات، MS Excel ورک بک، MS پاورپوائنٹ پریزنٹیشنز، Adobe Photoshop فائلوں اور مختلف امیج فارمیٹس پر رکھے جا سکتے ہیں۔ صارفین اپنے دستاویز پر دستخط کر سکتے ہیں اور ان دستاویزات پر رکھے گئے ای دستخطوں کو اپ ڈیٹ، تلاش، تصدیق، حذف یا پیش نظارہ کر سکتے ہیں۔ مزید یہ کہ دستخطوں کی تخصیص کے لیے بہت ساری صلاحیتیں فراہم کی گئی ہیں۔
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java میں Image کے ساتھ Xlsb پر دستخط کرنے کے مراحل"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) جلد اور آسانی سے Image دستخطوں کے ساتھ Xlsb دستاویزات پر دستخط کرنے کی صلاحیت فراہم کرتا ہے۔
        
        * دستخط کلاس کی ایک مثال بنائیں جو کہ Xlsb فائل کو پاتھ یا میموری اسٹریم کے طور پر دستخط کرنے کے لیے فراہم کرتی ہے۔
        * SignOptions کلاس کو فوری بنائیں اور تمام مطلوبہ ڈیٹا سیٹ کریں۔
        * Signature.Sign() طریقہ پاس کرنے کے آؤٹ پٹ Xlsb فائل یا میموری اسٹریم کو استعمال کریں

    title_right: " سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Signature for Java تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔

        * آپریٹنگ سسٹم: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        * ترقی کے ماحول: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * تازہ ترین GroupDocs.Signature for Java حاصل کریں [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) سے
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";
        // Set up output file
        String outputFilePath = "output.xlsb";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Xlsb document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Image لائیو ڈیمو کے ساتھ Xlsb دستاویزات پر دستخط کرنا"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ویب سائٹ پر جا کر ابھی مختلف دستخطوں کے ساتھ Xlsb فائل پر دستخط کریں۔ مفت آن لائن ڈیمو آپ کا منتظر ہے۔          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java کے لیے دیگر تعاون یافتہ Image دستخط"
    content: |
        "آپ دستخط کی دیگر اقسام کے ساتھ بھی Xlsb پر دستخط کر سکتے ہیں۔ براہ کرم نیچے دی گئی فہرست دیکھیں۔"
    format: 
       
       
back_to_top:
    enable: true
---