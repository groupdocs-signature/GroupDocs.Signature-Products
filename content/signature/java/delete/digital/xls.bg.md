---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xls
productName: Java
lang: bg
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xls for Java

############################# Head ############################
head_title: "Изтрийте Digital подписи от Xls файлове чрез Java"
head_description: "Изтриването на конкретни Digital подписи от подписани Xls документи може да се извърши лесно с кратък Java код."

############################# Header ############################
title: "Премахнете Digital подписи, които са поставени във Xls файлове"
description: "Изтрийте различни подписи Digital от Xls документи. Премахването на подписи Digital изисква прост код Java."
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
    title: "Получете информация за функциите на API на GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API предоставя много начини за обработка на вашите документи с помощта на електронни подписи. Налични са цифрови подписи като текстове, изображения, цифрови сертификати, баркодове, QR-кодове, печати или метаданни. Клиентите имат възможност да добавят, изтриват, актуализират, проверяват или търсят цифрови подписи в PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint, файлове на Adobe Photoshop и различни формати на изображения. Предоставени са голям брой полезни функции и настройки.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как да премахнете подписи Digital от вашия Xls документ"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) предоставя полезна функция за изчистване на Xls документи от Digital подписи с няколко реда код.
        
        * Първо, инстанцирайте пътя за преминаване на обект на подпис към вашия документ като параметър на конструктора.
        * След това създайте подходящ обект за подпис и настройте неговия уникален идентификатор.
        * След това извикайте метода Delete, предавайки обект на подпис, който трябва да бъде изтрит.
        * И накрая, обработете резултатите от операцията.

    title_right: "Системни изисквания"
    content_right: |
        GroupDocs.Signature for Java се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Изтеглете най-новата версия на GroupDocs.Signature for Java от [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "a01e1940-997a-444b-89af-9309a2d559a5";

        // provide signature item to delete
        DigitalSignature signatureToDelete = new DigitalSignature(id);

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
    title: "Подписване с Digital подписи Демо на живо"
    content: |
       Добавете различни електронни подписи към файла Xls точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Изтрийте вашите Digital подписи с Java"
    content: |
        "Изтриване на електронни подписи, които са добавени към различни формати на документи. Премахнете подписите бързо без допълнителен код."
    format: 
       
       
back_to_top:
    enable: true
---