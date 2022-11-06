---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Docm
productName: Java
lang: bg
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Docm for Java

############################# Head ############################
head_title: "Добавяне на подписи Image към файл Docm с Java"
head_description: "Поставете подпис Image върху файл Docm за Java, като използвате няколко реда код. Използвайте API на GroupDocs Document Signature, за да подписвате десетки файлови формати."

############################# Header ############################
title: "Подпишете Docm файлове с Image подписи в Java"
description: "Как да добавите Image подпис с няколко реда код на Java"
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
    title: "Относно API за подписи на изображения на GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) е популярен API за електронно подписване на цифрови документи. Налични са подписи като текстове, изображения, цифрови сертификати, баркодове, QR-кодове, печати или метаданни. Подписи могат да се поставят върху PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint, файлове на Adobe Photoshop и различни формати на изображения. Клиентите могат да подписват своя документ и да актуализират, търсят, проверяват, изтриват или визуализират електронни подписи, които са поставени върху тези документи. Освен това са предоставени много възможности за персонализиране на подписи.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Стъпки за подписване на Docm с Image в Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) предоставя възможност за бързо и лесно подписване на Docm документи с Image подписи.
        
        * Създайте екземпляр на клас подпис, предоставящ файл Docm, който трябва да се подписва като път или поток от памет
        * Създайте клас SignOptions и задайте всички изисквани данни.
        * Извикване на метода Signature.Sign(), предаващ изходен файл Docm или поток от памет

    title_right: " Системни изисквания"
    content_right: |
        GroupDocs.Signature for Java се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Вземете най-новия GroupDocs.Signature for Java от [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";
        // Set up output file
        String outputFilePath = "output.docm";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Docm document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписване на Docm документи с Image Демо на живо"
    content: |
       Подпишете файл Docm с различни подписи точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безплатна онлайн демонстрация ви очаква.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Други поддържани подписи Image за Java"
    content: |
        "Можете също да подпишете Docm с други типове подписи. Моля, вижте списъка по-долу."
    format: 
       
       
back_to_top:
    enable: true
---