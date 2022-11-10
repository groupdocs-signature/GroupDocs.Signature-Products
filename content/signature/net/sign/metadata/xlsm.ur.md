---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xlsm
productName: .NET
lang: ur
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xlsm for C#

############################# Head ############################
head_title: "C# کے ذریعے Xlsm دستاویزات میں میٹا ڈیٹا الیکٹرانک دستخط شامل کریں"
head_description: "C# کوڈ کی چند سطروں کا استعمال کرتے ہوئے اپنے Xlsm دستاویزات کے اندر چھپے ہوئے الیکٹرانک دستخطوں کے طور پر میٹا ڈیٹا استعمال کریں۔ میٹا ڈیٹا کی معلومات کے ساتھ اپنے کاروباری دستاویزات اور فائلوں پر ای سائن کرنے کے لیے GroupDocs Document Signature API کا استعمال کریں۔"

############################# Header ############################
title: ".NET کے ذریعے Xlsm دستاویز کے لیے میٹا ڈیٹا الیکٹرانک دستخط سادہ اور استعمال میں آسان ہیں!"
description: "پوشیدہ میٹا ڈیٹا اندراجات کے ساتھ اپنے Xlsm دستاویزات اور معاہدوں پر دستخط کریں۔ پی ڈی ایف، ایم ایس ورڈ دستاویزات، ایم ایس ایکسل ورک بک، ایم ایس پاورپوائنٹ پریزنٹیشنز اور مختلف امیج فارمیٹس کے لیے بغیر کسی پریشانی اور اضافی کوڈنگ کے میٹا ڈیٹا بنائیں۔"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET میٹا ڈیٹا دستخط API کے بارے میں"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ڈیجیٹل دستاویزات کے ای سائننگ کے لیے ایک مقبول API ہے۔ دستخط جیسے متن، تصاویر، ڈیجیٹل سرٹیفکیٹ، بارکوڈ، کیو آر کوڈ، ڈاک ٹکٹ یا میٹا ڈیٹا دستیاب ہیں۔ دستخط PDFs، MS Word دستاویزات، MS Excel ورک بک، MS پاورپوائنٹ پریزنٹیشنز، Adobe Photoshop فائلوں اور مختلف امیج فارمیٹس پر رکھے جا سکتے ہیں۔ صارفین اپنے دستاویز پر دستخط کر سکتے ہیں اور ان دستاویزات پر رکھے گئے ای دستخطوں کو اپ ڈیٹ، تلاش، تصدیق، حذف یا پیش نظارہ کر سکتے ہیں۔ مزید یہ کہ دستخطوں کی تخصیص کے لیے بہت ساری صلاحیتیں فراہم کی گئی ہیں۔
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# میں Metadata کے ساتھ Xlsm پر دستخط کرنے کے مراحل"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) جلد اور آسانی سے Metadata دستخطوں کے ساتھ Xlsm دستاویزات پر دستخط کرنے کی صلاحیت فراہم کرتا ہے۔
        
        * دستخط کلاس کی ایک مثال بنائیں جو کہ Xlsm فائل کو پاتھ یا میموری اسٹریم کے طور پر دستخط کرنے کے لیے فراہم کرتی ہے۔
        * SignOptions کلاس کو فوری بنائیں اور تمام مطلوبہ ڈیٹا سیٹ کریں۔
        * Signature.Sign() طریقہ پاس کرنے کے آؤٹ پٹ Xlsm فائل یا میموری اسٹریم کو استعمال کریں

    title_right: " سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Signature for .NET تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔

        * آپریٹنگ سسٹم: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        * ترقی کے ماحول: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * تازہ ترین GroupDocs.Signature for .NET حاصل کریں [Nuget](https://www.nuget.org/packages/groupdocs.signature) سے
         
    code: |
        ```csharp    
        
        // Set up input Xlsm file
        string filePath = "input.xlsm";
        // Set up output file
        string outputFilePath = "output.xlsm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Xlsm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Metadata لائیو ڈیمو کے ساتھ Xlsm دستاویزات پر دستخط کرنا"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ویب سائٹ پر جا کر ابھی مختلف دستخطوں کے ساتھ Xlsm فائل پر دستخط کریں۔ مفت آن لائن ڈیمو آپ کا منتظر ہے۔          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# کے لیے دیگر تعاون یافتہ Metadata دستخط"
    content: |
        "آپ دستخط کی دیگر اقسام کے ساتھ بھی Xlsm پر دستخط کر سکتے ہیں۔ براہ کرم نیچے دی گئی فہرست دیکھیں۔"
    format: 
       
       
back_to_top:
    enable: true
---