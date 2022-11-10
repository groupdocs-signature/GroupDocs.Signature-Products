---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Docx
productName: .NET
lang: ur
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docx for C#

############################# Head ############################
head_title: "C# کے ساتھ Docx فائل میں ڈیجیٹل الیکٹرانک دستخط شامل کرنا"
head_description: "کوڈ کی چند سطروں کا استعمال کرتے ہوئے .NET کے لیے Docx فائل پر ڈیجیٹل دستخط لگائیں۔ درجنوں فائل فارمیٹس پر دستخط کرنے کے لیے GroupDocs Document Signature API کا استعمال کریں۔"

############################# Header ############################
title: "C# میں Digital دستخطوں کے ساتھ eSign Docx فائلیں"
description: ".NET کوڈ کی چند سطروں کے ساتھ Digital دستخط کیسے شامل کریں"
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
    title: "GroupDocs.Signature for .NET ڈیجیٹل دستخط API کے بارے میں"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ڈیجیٹل الیکٹرانک دستخطوں کے ساتھ، ڈیجیٹل سرٹیفکیٹس کے ساتھ دستاویزات پر دستخط کرنے کے لیے ایک مقبول API ہے۔ ڈیجیٹل دستخطوں کے لیے API PFX سرٹیفکیٹ فائلوں کو پاس ورڈ سے محفوظ نجی اور عوامی کلیدوں کے ساتھ دستاویز پر دستخط کرنے کے لیے استعمال کرتا ہے۔ ڈیجیٹل دستخطوں کا استعمال کاروباری دستاویزات کو eSign PDF مخصوص صفحہ کے ساتھ تصدیق کرنے، Microsoft Office کے تمام دستاویزات جیسے Words، Excel، PowerPoint فائلوں، اور Open Office دستاویزات کی تصدیق کے لیے کیا جا سکتا ہے۔ صارفین آسانی سے دستخطوں کو جوڑ سکتے ہیں جیسے ان میں ترمیم کرنا، ہٹانا یا ایڈجسٹ کرنا۔ API دستخطوں کو تلاش اور تصدیق کرنے کا ایک طریقہ فراہم کرتا ہے۔ مزید یہ کہ دستخطوں کی تخصیص کے لیے بہت ساری صلاحیتیں فراہم کی گئی ہیں۔
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# میں Digital کے ساتھ Docx پر دستخط کرنے کے مراحل"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) جلد اور آسانی سے Digital دستخطوں کے ساتھ Docx دستاویزات پر دستخط کرنے کی صلاحیت فراہم کرتا ہے۔
        
        * دستخط کلاس کی ایک مثال بنائیں جو کہ Docx فائل کو پاتھ یا میموری اسٹریم کے طور پر دستخط کرنے کے لیے فراہم کرتی ہے۔
        * SignOptions کلاس کو فوری بنائیں اور تمام مطلوبہ ڈیٹا سیٹ کریں۔
        * Signature.Sign() طریقہ پاس کرنے کے آؤٹ پٹ Docx فائل یا میموری اسٹریم کو استعمال کریں

    title_right: " سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Signature for .NET تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔

        * آپریٹنگ سسٹم: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        * ترقی کے ماحول: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * تازہ ترین GroupDocs.Signature for .NET حاصل کریں [Nuget](https://www.nuget.org/packages/groupdocs.signature) سے
         
    code: |
        ```csharp    
                
        // Set up input Docx file
        string filePath = "input.docx";
        // Set up output file
        string outputFilePath = "output.docx";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Docx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital لائیو ڈیمو کے ساتھ Docx دستاویزات پر دستخط کرنا"
    content: |
       [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ویب سائٹ پر جا کر ابھی مختلف دستخطوں کے ساتھ Docx فائل پر دستخط کریں۔ مفت آن لائن ڈیمو آپ کا منتظر ہے۔          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# کے لیے دیگر تعاون یافتہ Digital دستخط"
    content: |
        "آپ دستخط کی دیگر اقسام کے ساتھ بھی Docx پر دستخط کر سکتے ہیں۔ براہ کرم نیچے دی گئی فہرست دیکھیں۔"
    format: 
       
       
back_to_top:
    enable: true
---