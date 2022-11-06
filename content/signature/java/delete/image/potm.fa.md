---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Potm
productName: Java
lang: fa
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Potm for Java

############################# Head ############################
head_title: "حذف امضاهای Image از فایل‌های Potm از طریق Java"
head_description: "حذف امضاهای خاص Image از اسناد امضا شده Potm ممکن است به راحتی با کد کوتاه Java انجام شود."

############################# Header ############################
title: "حذف Image امضاهایی که در فایل‌های Potm قرار گرفته‌اند."
description: "امضاهای مختلف Image را از اسناد Potm حذف کنید. حذف امضاهای Image به کد Java ساده نیاز دارد."
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
    title: "اطلاعاتی درباره ویژگی‌های API GroupDocs.Signature for Java دریافت کنید"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API راه های زیادی برای پردازش اسناد شما با استفاده از امضای الکترونیکی ارائه می دهد. امضاهای دیجیتال مانند متون، تصاویر، گواهی های دیجیتال، بارکدها، کدهای QR، تمبر یا ابرداده در دسترس هستند. مشتریان امکان افزودن، حذف، به روز رسانی، تأیید یا جستجوی امضاهای دیجیتال را در فایل های PDF، اسناد MS Word، کتاب های کار MS Excel، ارائه های MS PowerPoint، فایل های Adobe Photoshop و فرمت های تصویری مختلف دارند. تعداد زیادی از ویژگی ها و تنظیمات مفید ارائه شده است.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "نحوه حذف امضاهای Image از سند Potm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ویژگی مفیدی را برای پاک کردن اسناد Potm از امضاهای Image با چند خط کد ارائه می‌کند.
        
        * ابتدا، مسیر عبور شی Signature به سند خود را به عنوان پارامتر سازنده نمونه سازی کنید.
        * سپس، یک شی امضای مناسب ایجاد کنید و شناسه منحصر به فرد آن را تنظیم کنید.
        * پس از آن، متد Delete را فراخوانی کنید که شی امضا را ارسال می کند که باید حذف شود.
        * در نهایت، نتایج عملیات را پردازش کنید.

    title_right: "سیستم مورد نیاز"
    content_right: |
        GroupDocs.Signature for Java در تمام سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.

        * سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        * محیط های توسعه: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * آخرین نسخه GroupDocs.Signature for Java را از [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) دانلود کنید
         
    code: |
        ```java    
                
        // Set up input Potm file
        String filePath = "input.potm";
        // Set up output file
        String outputFilePath = "output.potm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

        // provide signature features to delete
        ImageSignature signatureToDelete = new ImageSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "امضا کردن با امضاهای Image نمایش زنده"
    content: |
       با مراجعه به وب‌سایت [GroupDocs.Signature App](https://products.groupdocs.app/signature/family)، همین حالا امضاهای الکترونیکی مختلف را به فایل Potm اضافه کنید.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "امضاهای Image خود را با Java حذف کنید"
    content: |
        "حذف امضاهای الکترونیکی که به فرمت های مختلف اسناد اضافه شده اند. امضاها را به سرعت بدون کد اضافی حذف کنید."
    format: 
       
       
back_to_top:
    enable: true
---