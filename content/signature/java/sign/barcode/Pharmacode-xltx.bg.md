---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Xltx
productName: Java
lang: bg
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Xltx for Java

############################# Head ############################
head_title: "eSign Xltx документ с Pharmacode баркод в Java"
head_description: "Създайте Pharmacode баркод подпис и го поставете в Xltx документ с Java, като използвате няколко реда код. Използвайте API на GroupDocs Document Signature за подписване на различни файлови формати."

############################# Header ############################
title: "Генерирайте Pharmacode баркод подпис за документ Xltx в Java"
description: "Електронно подпишете вашите Xltx бизнес документи с Pharmacode баркод. Генерирайте баркод подпис бързо и лесно с няколко реда код, за да зададете опции за подписване."
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
    title: "Относно API за подписи на баркодове на GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) е бърз и лесен API за управление на електронно подписване на цифрови документи с помощта на типове баркодове като UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 и много други. Клиентите могат лесно да създават баркодове, предоставящи необходимия текст, и да ги поставят в PDF, Microsoft Office Words документи, Microsoft Office Excel работни книги, MS PowerPoint презентации, Adobe Photoshop файлове и различни формати на изображения. Баркодовете, поставени в документи, могат да бъдат актуализирани, търсени, потвърдени, изтрити или визуализирани. Освен това се поддържа персонализиране на баркодове.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Стъпки за подписване на Xltx с Barcode в Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) предоставя възможност за бързо и лесно подписване на Xltx документи с Barcode подписи.
        
        * Създайте екземпляр на клас подпис, предоставящ файл Xltx, който трябва да се подписва като път или поток от памет
        * Създайте клас SignOptions и задайте всички изисквани данни.
        * Извикване на метода Signature.Sign(), предаващ изходен файл Xltx или поток от памет

    title_right: " Системни изисквания"
    content_right: |
        GroupDocs.Signature for Java се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Вземете най-новия GroupDocs.Signature for Java от [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltx file
        String filePath = "input.xltx";
        // Set up output file
        String outputFilePath = "output.xltx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Pharmacode);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Xltx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписване на Xltx документи с Barcode Демо на живо"
    content: |
       Подпишете файл Xltx с различни подписи точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безплатна онлайн демонстрация ви очаква.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode, известен също като Pharmaceutical Binary Code, е стандарт за баркод, използван във фармацевтичната индустрия като система за контрол на опаковката.
          characterset: |
             Цифри (0-9).
          textcapacity: |
             Представлява само едно цяло число от 3 до 131070.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Други поддържани подписи Barcode за Java"
    content: |
        "Можете също да подпишете Xltx с други типове подписи. Моля, вижте списъка по-долу."
    format: 
        
       
back_to_top:
    enable: true
---