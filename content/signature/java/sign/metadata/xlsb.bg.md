---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xlsb
productName: Java
lang: bg
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xlsb for Java

############################# Head ############################
head_title: "Добавяне на електронни подписи с метаданни към Xlsb документи чрез Java"
head_description: "Използвайте метаданни като скрити електронни подписи във вашите Xlsb документи, като използвате няколко реда от Java код. Използвайте API за подписване на документи на GroupDocs, за да подпишете електронно вашите бизнес документи и файлове с информация за метаданни."

############################# Header ############################
title: "Електронните подписи с метаданни за документ Xlsb чрез Java са прости и лесни за използване!"
description: "Електронно подпишете вашите Xlsb документи и договори със скрити записи на метаданни. Генерирайте метаданни за PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint и различни формати на изображения без проблеми и допълнително кодиране."
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
    title: "Относно API за подписи на метаданни на GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) е популярен API за електронно подписване на цифрови документи. Налични са подписи като текстове, изображения, цифрови сертификати, баркодове, QR-кодове, печати или метаданни. Подписи могат да се поставят върху PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint, файлове на Adobe Photoshop и различни формати на изображения. Клиентите могат да подписват своя документ и да актуализират, търсят, проверяват, изтриват или визуализират електронни подписи, които са поставени върху тези документи. Освен това са предоставени много възможности за персонализиране на подписи.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Стъпки за подписване на Xlsb с Metadata в Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) предоставя възможност за бързо и лесно подписване на Xlsb документи с Metadata подписи.
        
        * Създайте екземпляр на клас подпис, предоставящ файл Xlsb, който трябва да се подписва като път или поток от памет
        * Създайте клас SignOptions и задайте всички изисквани данни.
        * Извикване на метода Signature.Sign(), предаващ изходен файл Xlsb или поток от памет

    title_right: " Системни изисквания"
    content_right: |
        GroupDocs.Signature for Java се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Вземете най-новия GroupDocs.Signature for Java от [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsb file
        String filePath = "input.xlsb";
        // Set up output file
        String outputFilePath = "output.xlsb";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Xlsb document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписване на Xlsb документи с Metadata Демо на живо"
    content: |
       Подпишете файл Xlsb с различни подписи точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безплатна онлайн демонстрация ви очаква.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Други поддържани подписи Metadata за Java"
    content: |
        "Можете също да подпишете Xlsb с други типове подписи. Моля, вижте списъка по-долу."
    format: 
       
       
back_to_top:
    enable: true
---