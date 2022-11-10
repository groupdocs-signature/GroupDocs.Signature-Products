---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Otp
productName: .NET
lang: ur
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Otp for C#

############################# Head ############################
head_title: "C# کے ذریعے Otp فائلوں سے Image دستخطوں کو حذف کریں"
head_description: "دستخط شدہ Otp دستاویزات سے مخصوص Image دستخطوں کو حذف کرنا مختصر .NET کوڈ کے ساتھ آسانی سے انجام دیا جا سکتا ہے۔"

############################# Header ############################
title: "Image دستخطوں کو ہٹا دیں جو Otp فائلوں میں رکھے گئے ہیں"
description: "Otp دستاویزات سے مختلف Image دستخطوں کو حذف کریں۔ Image دستخطوں کو ہٹانے کے لیے سادہ C# کوڈ کی ضرورت ہے۔"
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
    title: "GroupDocs.Signature for .NET API خصوصیات کے بارے میں معلومات حاصل کریں۔"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API الیکٹرانک دستخطوں کا استعمال کرتے ہوئے آپ کے دستاویزات پر کارروائی کرنے کے بہت سے طریقے فراہم کرتا ہے۔ ڈیجیٹل دستخط جیسے متن، تصاویر، ڈیجیٹل سرٹیفکیٹ، بارکوڈ، QR-کوڈ، ڈاک ٹکٹ یا میٹا ڈیٹا دستیاب ہیں۔ صارفین کے پاس پی ڈی ایف، ایم ایس ورڈ دستاویزات، ایم ایس ایکسل ورک بک، ایم ایس پاورپوائنٹ پریزنٹیشنز، ایڈوب فوٹوشاپ فائلز اور مختلف امیج فارمیٹس پر ڈیجیٹل دستخط شامل کرنے، حذف کرنے، اپ ڈیٹ کرنے، تصدیق کرنے یا تلاش کرنے کا امکان ہے۔ مفید خصوصیات اور ترتیبات کی ایک بڑی تعداد فراہم کی گئی ہے۔
    

############################# Steps ############################
steps:
    enable: true
    title_left: "اپنے Otp دستاویز سے Image دستخطوں کو کیسے ہٹایا جائے۔"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) کوڈ کی چند سطروں کے ساتھ Image دستخطوں کی Otp دستاویزات کو صاف کرنے کے لیے مفید خصوصیت فراہم کرتا ہے۔
        
        * سب سے پہلے، کنسٹرکٹر پیرامیٹر کے طور پر اپنے دستاویز میں دستخطی آبجیکٹ گزرنے کا راستہ فوری بنائیں۔
        * پھر، ایک مناسب دستخطی آبجیکٹ بنائیں اور اس کا منفرد شناخت کنندہ ترتیب دیں۔
        * اس کے بعد، دستخطی آبجیکٹ کو پاس کرنے والے ڈیلیٹ طریقہ کی درخواست کریں جسے حذف کرنا ضروری ہے۔
        * آخر میں، عمل کے آپریشن کے نتائج.

    title_right: "سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Signature for .NET تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔

        * آپریٹنگ سسٹم: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        * ترقی کے ماحول: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * GroupDocs.Signature for .NET کا تازہ ترین ورژن [Nuget](https://www.nuget.org/packages/groupdocs.signature) سے ڈاؤن لوڈ کریں۔
         
    code: |
        ```csharp    
                
        // Set up input Otp file
        string filePath = "input.otp";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

                // provide signature features to delete
                // set up particular signature id
                ImageSignature signatureToDelete = new ImageSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Image کے ساتھ دستخط کرنا لائیو ڈیمو"
    content: |
       ابھی [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ویب سائٹ پر جا کر Otp فائل میں مختلف الیکٹرانک دستخط شامل کریں۔          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# کے ساتھ اپنے Image دستخطوں کو حذف کریں"
    content: |
        "ای دستخطوں کو حذف کرنا جو مختلف دستاویز کی شکلوں میں شامل کیے گئے تھے۔ اضافی کوڈ کے بغیر دستخطوں کو جلدی سے ہٹا دیں۔"
    format: 
       
       
back_to_top:
    enable: true
---