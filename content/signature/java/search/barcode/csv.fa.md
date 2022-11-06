---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Csv
productName: Java
lang: fa
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Csv with Java

############################# Head ############################
head_title: "جستجوی امضاهای Barcode در فایل Csv در Java"
head_description: "از Java برای جستجوی امضاهای Barcode در فایل های Csv با استفاده از چند خط کد استفاده کنید."

############################# Header ############################
title: "امضاهای Barcode را در فایل Csv جستجو کنید"
description: "API بومی Java امکان جستجوی امضاهای Barcode را در فایل‌های Csv از قبل امضا شده می‌دهد. با استفاده از چند خط کد، جستجوی پیشرفته امضای الکترونیکی را در اسناد Csv خود انجام دهید."
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
    title: "درباره GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API Java را برای پردازش اسناد با استفاده از انواع مختلف امضا مانند متون، تصاویر، گواهی‌های دیجیتال، بارکد، کدهای QR، تمبر یا ابرداده ارائه می‌کند. کاربران می‌توانند امضاهای الکترونیکی را در فایل‌های PDF، اسناد MS Word، کتاب‌های کار MS Excel، ارائه‌های MS PowerPoint، فایل‌های Adobe Photoshop و فرمت‌های تصویر مختلف با پشتیبانی اضافی برای سفارشی‌سازی ویژگی‌های امضا در صورت لزوم اضافه، حذف، به‌روزرسانی، تأیید یا جستجو کنند.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "نحوه جستجوی امضاهای Barcode در Csv"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) با اجرای چند مرحله آسان، جستجوی امضاهای Barcode در فایل‌های Csv را برای توسعه‌دهندگان Java آسان‌تر می‌کند.
        
        * یک نمونه جدید از کلاس Signature ایجاد کنید و مسیر سند منبع را به عنوان پارامتر سازنده ارسال کنید.
        * شی SearchOptions را مطابق با نیاز خود نمونه سازی کنید و گزینه های جستجو را مشخص کنید.
        * متد Search نمونه کلاس Signature را فراخوانی کنید و SearchOptions را به آن ارسال کنید.
        * نتایج جستجو را بر اساس خواسته های خود پردازش کنید.

    title_right: "سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for Java در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * آخرین نسخه GroupDocs.Signature for Java را از [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) دانلود کنید
         
    code: |
        ```java    
        
        // Set up input Csv file
        String filePath = "input.csv";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        BarcodeSearchOptions options = new BarcodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Barcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Barcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Barcode signatures in Csv document
        List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode امضای الکترونیکی نسخه نمایشی زنده را جستجو کنید"
    content: |
       اکنون با مراجعه به وب‌سایت [GroupDocs.Signature App] (https://products.groupdocs.app/signature/family)، سند را برای امضاهای الکترونیکی مختلف در فایل‌های Csv جستجو کنید.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "جستجوی امضاهای دیگر Barcode با استفاده از Java"
    content: |
        "جستجوی امضای الکترونیکی در اسناد مختلف. همانطور که در زیر نشان داده شده است، امضاها را از یکی از فرمت های فایل محبوب پیدا کنید."
    format: 
           
       
back_to_top:
    enable: true
---