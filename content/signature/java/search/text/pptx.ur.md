---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Pptx
productName: Java
lang: ur
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Pptx with Java

############################# Head ############################
head_title: "Java میں Pptx فائل میں Text دستخط تلاش کریں۔"
head_description: "کوڈ کی چند سطروں کا استعمال کرتے ہوئے Pptx فائلوں میں Text دستخط تلاش کرنے کے لیے Java استعمال کریں۔"

############################# Header ############################
title: "Pptx فائل میں Text دستخط تلاش کریں۔"
description: "Java مقامی API پہلے سے دستخط شدہ Pptx فائلوں میں Text دستخطوں کو تلاش کرنے کی اجازت دیتا ہے۔ کوڈ کی چند سطروں کا استعمال کرتے ہوئے اپنے Pptx دستاویزات کے اندر اعلی درجے کی ای دستخط تلاش کریں۔"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java API کے بارے میں"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) مختلف دستخطی اقسام جیسے متن، تصاویر، ڈیجیٹل سرٹیفیکیٹس، بارکوڈز، QR-کوڈز، ڈاک ٹکٹ یا میٹا ڈیٹا کا استعمال کرتے ہوئے دستاویزات پر کارروائی کرنے کے لیے Java API فراہم کرتا ہے۔ صارفین پی ڈی ایف، ایم ایس ورڈ دستاویزات، ایم ایس ایکسل ورک بک، ایم ایس پاورپوائنٹ پریزنٹیشنز، ایڈوب فوٹوشاپ فائلز اور مختلف امیج فارمیٹس میں الیکٹرانک دستخط شامل، حذف، اپ ڈیٹ، تصدیق یا تلاش کرسکتے ہیں، ضرورت کے مطابق دستخط کی خصوصیات کو حسب ضرورت بنانے کے لیے اضافی تعاون کے ساتھ۔
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Pptx میں Text دستخط کیسے تلاش کریں"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) Java ڈویلپرز کے لیے چند آسان اقدامات کو لاگو کرکے اپنی ایپلی کیشنز سے Text فائلوں میں Text دستخط تلاش کرنا آسان بناتا ہے۔
        
        * سگنیچر کلاس کی ایک نئی مثال بنائیں اور کنسٹرکٹر پیرامیٹر کے بطور سورس دستاویز کا راستہ پاس کریں۔
        * اپنی ضروریات کے مطابق SearchOptions آبجیکٹ کو فوری بنائیں اور تلاش کے اختیارات کی وضاحت کریں۔
        * سگنیچر کلاس مثال کے سرچ طریقہ کو کال کریں اور اس میں Search Options پاس کریں۔
        * اپنے مطالبات کے مطابق تلاش کے نتائج پر کارروائی کریں۔

    title_right: "سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Signature for Java تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔

        * آپریٹنگ سسٹم: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        * ترقی کے ماحول: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * GroupDocs.Signature for Java کا تازہ ترین ورژن [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) سے ڈاؤن لوڈ کریں۔
         
    code: |
        ```java    
                
        // Set up input Pptx file
        String filePath = "input.pptx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        TextSearchOptions options = new TextSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
                            
        // search for Text signatures in Pptx document
        List<TextSignature> signatures = signature.search(TextSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Text الیکٹرانک دستخطوں کا لائیو ڈیمو تلاش کریں۔"
    content: |
       ابھی [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) ویب سائٹ پر جا کر Pptx فائلوں پر مختلف الیکٹرانک دستخطوں کے لیے دستاویز تلاش کریں۔

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Java کا استعمال کرتے ہوئے دیگر Text دستخط تلاش کریں۔"
    content: |
        "الیکٹرانک دستخط مختلف دستاویزات میں تلاش کرتے ہیں۔ ذیل میں دکھائے گئے مقبول فائل فارمیٹس میں سے ایک سے دستخط تلاش کریں۔"
    format: 
           
       
back_to_top:
    enable: true
---