---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Gif
productName: Java
lang: bg
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Gif for Java

############################# Head ############################
head_title: "Проверка на Qrcode подписи за Gif файлове чрез Java"
head_description: "Използвайте само няколко реда от кода на Java, за да проверите документите Gif и техните подписи Qrcode."

############################# Header ############################
title: "Qrcode проверка на подписи за Gif файлове"
description: "API за Java предоставя възможност за проверка на Qrcode подписи в Gif документи. Проверката на електронните подписи във вашите Gif документи може да се извърши бързо и лесно."
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
    title: "Открийте нови функции на API на GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API предоставя широка гама от начини за обработка на множество формати на документи чрез използване на електронни подписи. Поддържат се много видове цифрови подписи като текстове, изображения, цифрови сертификати, баркодове, QR-кодове, печати или метаданни. Клиентите могат да добавят, премахват, редактират, валидират или търсят цифрови подписи в PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint, файлове на Adobe Photoshop и различни формати на изображения. Налични са удивителен брой допълнителни функции и настройки.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как да валидирате Qrcode подписи във вашия Gif документ"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) включва полезни функции като проверка на подписи Qrcode, поставени в Gif документи. Използвайте тази възможност без внедряване на допълнителен код.
        
        * Първо, създайте клас Signature, предоставящ като параметър на конструктора път към документ, който трябва да бъде проверен.
        * Второ, създайте нов обект VerifyOptions и настройте всички необходими свойства.
        * И накрая, извикайте метода Verify на обекта Signature, като предавате екземпляр VerifyOptions.
        * След това обработете резултатите от проверката.

    title_right: "Системни изисквания"
    content_right: |
        GroupDocs.Signature for Java се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Изтеглете най-новата версия на GroupDocs.Signature for Java от [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Gif file
        String filePath = "input.gif";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписване с Qrcode подписи Демо на живо"
    content: |
       Добавете различни електронни подписи към файла Gif точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Проверете други Qrcode подписи с помощта на Java"
    content: |
        "Проверка на електронни подписи, поставени в различни документи. Проверете качеството на подписите в популярните файлови формати, както е показано по-долу."
    format: 
       
       
back_to_top:
    enable: true
---