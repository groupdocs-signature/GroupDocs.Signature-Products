---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Tar
productName: .NET
lang: ur
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Tar for C#

############################# Head ############################
head_title: "C# کے ذریعے Tar فائلوں کے لیے Digital دستخطوں کی تصدیق"
head_description: "Tar دستاویزات اور ان کے Digital دستخطوں کی تصدیق کے لیے .NET کوڈ کی صرف چند سطریں استعمال کریں۔"

############################# Header ############################
title: "Digital Tar فائلوں کے لیے دستخطوں کی تصدیق"
description: "API برائے .NET Tar دستاویزات پر Digital دستخطوں کی تصدیق کرنے کا موقع فراہم کرتا ہے۔ آپ کے Tar دستاویزات کے اندر ای دستخطوں کی تصدیق جلد اور آسانی سے کی جا سکتی ہے۔"
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
    title: "نئی GroupDocs.Signature for .NET API خصوصیات دریافت کریں۔"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API الیکٹرانک دستخطوں کا استعمال کرتے ہوئے متعدد دستاویزات کے فارمیٹس پر کارروائی کرنے کے وسیع طریقے فراہم کرتا ہے۔ متن، تصاویر، ڈیجیٹل سرٹیفکیٹ، بارکوڈ، QR-کوڈز، ڈاک ٹکٹ یا میٹا ڈیٹا کے طور پر ڈیجیٹل دستخطوں کی بہت سی قسمیں معاون ہیں۔ صارفین پی ڈی ایف، ایم ایس ورڈ دستاویزات، ایم ایس ایکسل ورک بک، ایم ایس پاورپوائنٹ پریزنٹیشنز، ایڈوب فوٹوشاپ فائلز اور مختلف امیج فارمیٹس پر ڈیجیٹل دستخط شامل، ہٹا سکتے، ترمیم، توثیق یا تلاش کرسکتے ہیں۔ اضافی خصوصیات اور ترتیبات کی حیرت انگیز تعداد دستیاب ہے۔
    

############################# Steps ############################
steps:
    enable: true
    title_left: "اپنے Tar دستاویز میں Digital دستخطوں کی تصدیق کیسے کریں"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) میں مفید خصوصیات شامل ہیں جیسے Tar دستاویزات پر رکھے گئے Digital دستخطوں کی تصدیق۔ اضافی کوڈ کو لاگو کیے بغیر اس موقع کا استعمال کریں۔
        
        * سب سے پہلے، ایک دستاویز کو کنسٹرکٹر پیرامیٹر کے راستے کے طور پر فراہم کرنے والے دستخط کی کلاس کو فوری طور پر فراہم کرنا جس کی تصدیق کی جانی چاہئے۔
        * دوم، ایک نیا VerifyOptions آبجیکٹ بنائیں اور تمام مطلوبہ خصوصیات کو ترتیب دیں۔
        * آخر میں، VerifyOptions مثال سے گزرتے ہوئے Signature کے آبجیکٹ کی تصدیق کا طریقہ استعمال کریں۔
        * پھر تصدیقی نتائج پر کارروائی کریں۔

    title_right: "سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Signature for .NET تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔

        * آپریٹنگ سسٹم: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        * ترقی کے ماحول: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * GroupDocs.Signature for .NET کا تازہ ترین ورژن [Nuget](https://www.nuget.org/packages/groupdocs.signature) سے ڈاؤن لوڈ کریں۔
         
    code: |
        ```csharp    
                
        // Set up input Tar file
        string filePath = "input.tar";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                DigitalVerifyOptions options = new DigitalVerifyOptions()
                {
                    // Digital signature comment
                    Comments = "Approved by co-owner",
                    // specify period of signatures
                    SignDateTimeFrom = new DateTime(year: 2021, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2022, month: 12, day: 31)
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital کے ساتھ دستخط کرنا لائیو ڈیمو"
    content: |
       ابھی [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ویب سائٹ پر جا کر Tar فائل میں مختلف الیکٹرانک دستخط شامل کریں۔          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# کا استعمال کرتے ہوئے دیگر Digital دستخطوں کی تصدیق کریں"
    content: |
        "مختلف دستاویزات میں رکھے گئے الیکٹرانک دستخطوں کی تصدیق۔ مشہور فائل فارمیٹس میں دستخطوں کا معیار چیک کریں جیسا کہ ذیل میں بتایا گیا ہے۔"
    format: 
       
       
back_to_top:
    enable: true
---