---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Barcode
fileformat: Xlsx
productName: Java
lang: bg
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Barcode signatures at Xlsx with Java

############################# Head ############################
head_title: "Търсене на подписи Barcode във файл Xlsx в Java"
head_description: "Използвайте Java за търсене на подписи Barcode във файлове Xlsx, като използвате няколко реда код."

############################# Header ############################
title: "Търсене на подписи Barcode във файл Xlsx"
description: "Нативният API на Java позволява търсене на подписи на Barcode във вече подписани файлове на Xlsx. Извършете разширено търсене с електронен подпис във вашите Xlsx документи, като използвате няколко реда код."
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
    title: "Относно API на GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) предоставя Java API за обработка на документи, използвайки различни типове подписи, като текстове, изображения, цифрови сертификати, баркодове, QR-кодове, печати или метаданни. Потребителите могат да добавят, изтриват, актуализират, проверяват или търсят електронни подписи в PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint, файлове на Adobe Photoshop и различни формати на изображения, с допълнителна поддръжка за персонализиране на свойствата на подписите, ако е необходимо.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как да търсите Barcode подписи във Xlsx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) улеснява разработчиците на Java да търсят подписи на Barcode във файловете на Xlsx от техните приложения чрез прилагане на няколко лесни стъпки.
        
        * Създайте нов екземпляр на клас Signature и подайте пътя на изходния документ като параметър на конструктора.
        * Създайте екземпляр на обекта SearchOptions според вашите изисквания и задайте опции за търсене.
        * Извикайте метода Search на екземпляра на класа Signature и му предайте SearchOptions.
        * Обработвайте резултатите от търсенето според вашите изисквания.

    title_right: "Системни изисквания"
    content_right: |
        GroupDocs.Signature for Java се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Изтеглете най-новата версия на GroupDocs.Signature for Java от [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Xlsx file
        String filePath = "input.xlsx";

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
                            
        // search for Barcode signatures in Xlsx document
        List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Търсете Barcode електронни подписи Демо на живо"
    content: |
       Потърсете в документа различни електронни подписи към Xlsx файлове точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Търсене на други Barcode подписи с помощта на Java"
    content: |
        "Търсене на електронни подписи в различни документи. Намерете подписи от един от популярните файлови формати, както е показано по-долу."
    format: 
           
       
back_to_top:
    enable: true
---