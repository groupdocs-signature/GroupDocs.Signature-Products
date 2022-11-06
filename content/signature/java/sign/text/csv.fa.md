---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Csv
productName: Java
lang: fa
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Csv for Java

############################# Head ############################
head_title: "ایجاد امضای الکترونیکی متنی در فایل Csv با Java"
head_description: "با استفاده از چند خط کد، Text eSignature را در فایل Csv برای Java قرار دهید. برای امضای ده ها فرمت فایل از GroupDocs Document Signature API استفاده کنید."

############################# Header ############################
title: "امضای فایل‌های Csv با امضاهای Text در Java"
description: "نحوه اضافه کردن امضای Text با چند خط کد Java"
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
    title: "درباره GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) یک API محبوب برای امضای الکترونیکی اسناد دیجیتال است. امضاهایی مانند متون، تصاویر، گواهی‌های دیجیتال، بارکدها، کدهای QR، تمبرها یا ابرداده‌ها در دسترس هستند. امضاها ممکن است روی فایل‌های PDF، اسناد MS Word، کتاب‌های کار MS Excel، ارائه‌های MS PowerPoint، فایل‌های Adobe Photoshop و فرمت‌های تصویر مختلف قرار داده شوند. مشتریان می توانند سند خود را امضا کنند و امضاهای الکترونیکی را که روی آن اسناد قرار داده شده است را به روز کنند، جستجو، تأیید، حذف یا پیش نمایش کنند. علاوه بر این، توانایی های زیادی برای سفارشی سازی امضا ارائه شده است.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "مراحل امضای Csv با Text در Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) امکان امضای اسناد Csv با امضاهای Text را سریع و آسان فراهم می‌کند.
        
        * یک نمونه از کلاس Signature ایجاد کنید که فایل Csv را به عنوان مسیر یا جریان حافظه امضا می کند.
        * کلاس SignOptions را راه اندازی کنید و تمام داده های درخواستی را تنظیم کنید.
        * فراخوانی متد Signature.Sign() برای ارسال خروجی Csv فایل یا جریان حافظه

    title_right: " سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for Java در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * آخرین GroupDocs.Signature for Java را از [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) دریافت کنید
         
    code: |
        ```java    
                
        // Set up input Csv file
        String filePath = "input.csv";
        // Set up output file
        String outputFilePath = "output.csv";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Csv document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "امضای اسناد Csv با نسخه نمایشی زنده Text"
    content: |
       با مراجعه به وب‌سایت [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) فایل Csv را با امضاهای مختلف در حال حاضر امضا کنید. نسخه ی نمایشی آنلاین رایگان در انتظار شماست.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "سایر امضاهای پشتیبانی شده Text برای Java"
    content: |
        "همچنین می‌توانید {{Format}} را با سایر انواع امضا امضا کنید. لطفا لیست زیر را ببینید."
    format: 
       
       
back_to_top:
    enable: true
---