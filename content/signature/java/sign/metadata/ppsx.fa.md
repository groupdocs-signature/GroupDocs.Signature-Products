---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Ppsx
productName: Java
lang: fa
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Ppsx for Java

############################# Head ############################
head_title: "از طریق Java امضاهای الکترونیکی فراداده را به اسناد Ppsx اضافه کنید"
head_description: "با استفاده از چند خط کد Java از فراداده به عنوان امضای الکترونیکی پنهان در اسناد Ppsx خود استفاده کنید. از GroupDocs Document Signature API برای امضای الکترونیکی اسناد و فایل‌های تجاری خود با اطلاعات فراداده استفاده کنید."

############################# Header ############################
title: "امضاهای الکترونیکی فراداده برای سند Ppsx از طریق Java ساده و آسان برای استفاده هستند!"
description: "اسناد و قراردادهای Ppsx خود را با ورودی‌های فراداده پنهان امضا کنید. فراداده برای فایل‌های PDF، اسناد MS Word، کتاب‌های کار MS Excel، ارائه‌های MS PowerPoint و فرمت‌های تصویری مختلف بدون مشکل و کدنویسی اضافی ایجاد کنید."
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
    title: "درباره GroupDocs.Signature for Java API امضاهای فراداده"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) یک API محبوب برای امضای الکترونیکی اسناد دیجیتال است. امضاهایی مانند متون، تصاویر، گواهی‌های دیجیتال، بارکدها، کدهای QR، تمبرها یا ابرداده‌ها در دسترس هستند. امضاها ممکن است روی فایل‌های PDF، اسناد MS Word، کتاب‌های کار MS Excel، ارائه‌های MS PowerPoint، فایل‌های Adobe Photoshop و فرمت‌های تصویر مختلف قرار داده شوند. مشتریان می توانند سند خود را امضا کنند و امضاهای الکترونیکی را که روی آن اسناد قرار داده شده است را به روز کنند، جستجو، تأیید، حذف یا پیش نمایش کنند. علاوه بر این، توانایی های زیادی برای سفارشی سازی امضا ارائه شده است.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "مراحل امضای Ppsx با Metadata در Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) امکان امضای اسناد Ppsx با امضاهای Metadata را سریع و آسان فراهم می‌کند.
        
        * یک نمونه از کلاس Signature ایجاد کنید که فایل Ppsx را به عنوان مسیر یا جریان حافظه امضا می کند.
        * کلاس SignOptions را راه اندازی کنید و تمام داده های درخواستی را تنظیم کنید.
        * فراخوانی متد Signature.Sign() برای ارسال خروجی Ppsx فایل یا جریان حافظه

    title_right: " سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for Java در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * آخرین GroupDocs.Signature for Java را از [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) دریافت کنید
         
    code: |
        ```java    
                
        // Set up input Ppsx file
        String filePath = "input.ppsx";
        // Set up output file
        String outputFilePath = "output.ppsx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Ppsx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "امضای اسناد Ppsx با نسخه نمایشی زنده Metadata"
    content: |
       با مراجعه به وب‌سایت [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) فایل Ppsx را با امضاهای مختلف در حال حاضر امضا کنید. نسخه ی نمایشی آنلاین رایگان در انتظار شماست.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "سایر امضاهای پشتیبانی شده Metadata برای Java"
    content: |
        "همچنین می‌توانید Ppsx را با سایر انواع امضا امضا کنید. لطفا لیست زیر را ببینید."
    format: 
       
       
back_to_top:
    enable: true
---