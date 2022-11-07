---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Csv
productName: .NET
lang: ur
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Csv with C#

############################# Head ############################
head_title: "C# میں Csv فائل میں Image دستخط تلاش کریں۔"
head_description: "کوڈ کی چند سطروں کا استعمال کرتے ہوئے Csv فائلوں میں Image دستخط تلاش کرنے کے لیے .NET استعمال کریں۔"

############################# Header ############################
title: "Csv فائل میں Image دستخط تلاش کریں۔"
description: ".NET مقامی API پہلے سے دستخط شدہ Csv فائلوں میں Image دستخطوں کو تلاش کرنے کی اجازت دیتا ہے۔ کوڈ کی چند سطروں کا استعمال کرتے ہوئے اپنے Csv دستاویزات کے اندر اعلی درجے کی ای دستخط تلاش کریں۔"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET API کے بارے میں"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) مختلف دستخطی اقسام جیسے متن، تصاویر، ڈیجیٹل سرٹیفیکیٹس، بارکوڈز، QR-کوڈز، ڈاک ٹکٹ یا میٹا ڈیٹا کا استعمال کرتے ہوئے دستاویزات پر کارروائی کرنے کے لیے .NET API فراہم کرتا ہے۔ صارفین پی ڈی ایف، ایم ایس ورڈ دستاویزات، ایم ایس ایکسل ورک بک، ایم ایس پاورپوائنٹ پریزنٹیشنز، ایڈوب فوٹوشاپ فائلز اور مختلف امیج فارمیٹس میں الیکٹرانک دستخط شامل، حذف، اپ ڈیٹ، تصدیق یا تلاش کرسکتے ہیں، ضرورت کے مطابق دستخط کی خصوصیات کو حسب ضرورت بنانے کے لیے اضافی تعاون کے ساتھ۔
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Csv میں Image دستخط کیسے تلاش کریں"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) .NET ڈویلپرز کے لیے چند آسان اقدامات کو لاگو کرکے اپنی ایپلی کیشنز سے Image فائلوں میں Image دستخط تلاش کرنا آسان بناتا ہے۔
        
        * سگنیچر کلاس کی ایک نئی مثال بنائیں اور کنسٹرکٹر پیرامیٹر کے بطور سورس دستاویز کا راستہ پاس کریں۔
        * اپنی ضروریات کے مطابق SearchOptions آبجیکٹ کو فوری بنائیں اور تلاش کے اختیارات کی وضاحت کریں۔
        * سگنیچر کلاس مثال کے سرچ طریقہ کو کال کریں اور اس میں Search Options پاس کریں۔
        * اپنے مطالبات کے مطابق تلاش کے نتائج پر کارروائی کریں۔

    title_right: "سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Signature for .NET تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔

        * آپریٹنگ سسٹم: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        * ترقی کے ماحول: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * GroupDocs.Signature for .NET کا تازہ ترین ورژن [Nuget](https://www.nuget.org/packages/groupdocs.signature) سے ڈاؤن لوڈ کریں۔
         
    code: |
        ```csharp    
                
        // Set up input Csv file
        string filePath = "input.csv";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  Image images for processing
                    ReturnContent = true,
                    // set up type of returned  Image images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for Image signatures in Csv document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Image الیکٹرانک دستخطوں کا لائیو ڈیمو تلاش کریں۔"
    content: |
       ابھی [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ویب سائٹ پر جا کر Csv فائلوں پر مختلف الیکٹرانک دستخطوں کے لیے دستاویز تلاش کریں۔

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "C# کا استعمال کرتے ہوئے دیگر Image دستخط تلاش کریں۔"
    content: |
        "الیکٹرانک دستخط مختلف دستاویزات میں تلاش کرتے ہیں۔ ذیل میں دکھائے گئے مقبول فائل فارمیٹس میں سے ایک سے دستخط تلاش کریں۔"
    format: 
           
       
back_to_top:
    enable: true
---