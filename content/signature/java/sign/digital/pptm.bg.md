---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pptm
productName: Java
lang: bg
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pptm for Java

############################# Head ############################
head_title: "Добавяне на цифрови електронни подписи към файл Pptm с Java"
head_description: "Поставете цифров подпис на файл Pptm за Java, като използвате няколко реда код. Използвайте API на GroupDocs Document Signature, за да подписвате десетки файлови формати."

############################# Header ############################
title: "eSign Pptm файлове с Digital подписи в Java"
description: "Как да добавите подпис Digital с няколко реда код на Java"
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
    title: "Относно API за цифрови подписи на GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) е популярен API за създаване на документи с цифрови електронни подписи, с цифрови сертификати. За цифровите подписи API използва PFX сертификатни файлове, за да подпише документ със защитени с парола частни и публични ключове. Цифровите подписи могат да се използват за сертифициране на бизнес документи с конкретна страница eSign PDF, за сертифициране на цели документи на Microsoft Office като Words, Excel, Powerpoint файлове и документи на Open Office. Клиентите могат лесно да манипулират подписите, като ги редактират, премахват или коригират. API предоставя начин за търсене и проверка на подписи. Освен това са предоставени много възможности за персонализиране на подписи.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Стъпки за подписване на Pptm с Digital в Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) предоставя възможност за бързо и лесно подписване на Pptm документи с Digital подписи.
        
        * Създайте екземпляр на клас подпис, предоставящ файл Pptm, който трябва да се подписва като път или поток от памет
        * Създайте клас SignOptions и задайте всички изисквани данни.
        * Извикване на метода Signature.Sign(), предаващ изходен файл Pptm или поток от памет

    title_right: " Системни изисквания"
    content_right: |
        GroupDocs.Signature for Java се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Вземете най-новия GroupDocs.Signature for Java от [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pptm file
        String filePath = "input.pptm";
        // Set up output file
        String outputFilePath = "output.pptm";
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

        // sign Pptm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписване на Pptm документи с Digital Демо на живо"
    content: |
       Подпишете файл Pptm с различни подписи точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безплатна онлайн демонстрация ви очаква.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Други поддържани подписи Digital за Java"
    content: |
        "Можете също да подпишете Pptm с други типове подписи. Моля, вижте списъка по-долу."
    format: 
       
       
back_to_top:
    enable: true
---