---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pdf
productName: Java
lang: fa
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pdf for Java

############################# Head ############################
head_title: "افزودن امضای الکترونیکی دیجیتال به فایل Pdf با Java"
head_description: "با استفاده از چند خط کد، امضای دیجیتال را روی فایل Pdf برای Java قرار دهید. برای امضای ده ها فرمت فایل از GroupDocs Document Signature API استفاده کنید."

############################# Header ############################
title: "eSign فایلهای Pdf با امضاهای Digital در Java"
description: "نحوه اضافه کردن امضای Digital با چند خط کد Java"
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
    title: "درباره GroupDocs.Signature for Java API امضای دیجیتال"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) یک API محبوب برای ثبت اسناد با امضای الکترونیکی دیجیتال، با گواهی‌های دیجیتال است. برای امضای دیجیتال API از فایل های گواهی PFX برای تنظیم سند با کلیدهای خصوصی و عمومی محافظت شده با رمز عبور استفاده می کند. امضاهای دیجیتال ممکن است برای تأیید اسناد تجاری با صفحه خاص eSign PDF، تأیید کل اسناد Microsoft Office مانند Words، Excel، فایل‌های Powerpoint و اسناد Open Office استفاده شوند. مشتریان به راحتی می توانند امضاها را مانند ویرایش، حذف یا تنظیم آن ها دستکاری کنند. API راهی برای جستجو و تأیید امضاها فراهم می کند. علاوه بر این، توانایی های زیادی برای سفارشی سازی امضا ارائه شده است.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "مراحل امضای Pdf با Digital در Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) امکان امضای اسناد Pdf با امضاهای Digital را سریع و آسان فراهم می‌کند.
        
        * یک نمونه از کلاس Signature ایجاد کنید که فایل Pdf را به عنوان مسیر یا جریان حافظه امضا می کند.
        * کلاس SignOptions را راه اندازی کنید و تمام داده های درخواستی را تنظیم کنید.
        * فراخوانی متد Signature.Sign() برای ارسال خروجی Pdf فایل یا جریان حافظه

    title_right: " سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for Java در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * آخرین GroupDocs.Signature for Java را از [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) دریافت کنید
         
    code: |
        ```java    
                
        // Set up input Pdf file
        String filePath = "input.pdf";
        // Set up output file
        String outputFilePath = "output.pdf";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Pdf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "امضای اسناد Pdf با نسخه نمایشی زنده Digital"
    content: |
       با مراجعه به وب‌سایت [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) فایل Pdf را با امضاهای مختلف در حال حاضر امضا کنید. نسخه ی نمایشی آنلاین رایگان در انتظار شماست.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "سایر امضاهای پشتیبانی شده Digital برای Java"
    content: |
        "همچنین می‌توانید Pdf را با سایر انواع امضا امضا کنید. لطفا لیست زیر را ببینید."
    format: 
       
       
back_to_top:
    enable: true
---