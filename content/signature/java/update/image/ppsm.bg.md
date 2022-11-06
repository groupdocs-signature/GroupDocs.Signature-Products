---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Ppsm
productName: Java
lang: bg
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Ppsm for Java

############################# Head ############################
head_title: "Актуализирайте Image подписи, поставени във Ppsm файлове с Java"
head_description: "Използвайте прост и лесен за разбиране код на Java за актуализиране на подписи на Image в подписани документи Ppsm."

############################# Header ############################
title: "Редактирайте и актуализирайте Image подписи, поставени във Ppsm файлове"
description: "API за Java предоставя функционалност за актуализиране на подписи на Image в документи на Ppsm. Актуализирайте електронните подписи във вашите Ppsm документи с няколко реда Java код бързо и лесно."
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
    title: "Научете за функциите на API на GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API функционалността съдържа богат избор от средства за обработка във формати на документи по заявка чрез използване на електронни подписи. Поддържат се широк спектър от електронни подписи като текстове, изображения, цифрови сертификати, баркодове, QR-кодове, печати или метаданни. Клиентите могат да добавят, премахват, редактират, валидират или търсят цифрови подписи в PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint, файлове на Adobe Photoshop и различни формати на изображения. Налични са множество полезни функции и настройки.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как да промените Image подписи във вашия Ppsm документ"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) включва полезни функции като актуализиране на Image подписи, поставени в Ppsm документи. Това прави възможно промяната на функциите на подписите без допълнителен код.
        
        * Като начало създайте обект Signature, предаващ като път на параметър на конструктор към документ, който трябва да бъде актуализиран.
        * След това създайте подходящ конкретен обект на подпис и настройте неговия идентификатор и свойства, които трябва да бъдат променени.
        * И накрая, извикайте метода за актуализиране на Signature, предавайки определен обект на подпис.
        * Процес на актуализиране на резултатите до ваше известие.

    title_right: "Системни изисквания"
    content_right: |
        GroupDocs.Signature for Java се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Изтеглете най-новата версия на GroupDocs.Signature for Java от [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ppsm file
        String filePath = "input.ppsm";
        // Set up output file
        String outputFilePath = "output.ppsm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Актуализиране на подписите Image на страниците на документа - Демо на живо"
    content: |
       Редактирайте различни електронни подписи на документа Ppsm точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Актуализирайте различни Image подписи чрез Java"
    content: |
        "Редактиране на цифрови подписи, които се поставят в различни формати на документи. Актуализирайте данните за подписи без допълнителен код."
    format: 
       
       
back_to_top:
    enable: true
---