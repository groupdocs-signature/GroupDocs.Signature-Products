---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xlsx
productName: Java
lang: uk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xlsx for Java

############################# Head ############################
head_title: "Додайте електронні підписи метаданих до документів Xlsx за допомогою Java"
head_description: "Використовуйте метадані як приховані електронні підписи у своїх документах Xlsx за допомогою кількох рядків коду Java. Використовуйте API підпису документів GroupDocs, щоб електронно підписувати свої бізнес-документи та файли з інформацією метаданих."

############################# Header ############################
title: "Електронні підписи метаданих для документа Xlsx через Java прості та легкі у використанні!"
description: "Електронно підписуйте свої Xlsx документи та контракти за допомогою прихованих записів метаданих. Створюйте метадані для PDF-файлів, документів MS Word, робочих книг MS Excel, презентацій MS PowerPoint і різних форматів зображень без проблем і додаткового кодування."
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
    title: "Про API підписів метаданих GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) — популярний API для електронного підпису цифрових документів. Доступні такі підписи, як тексти, зображення, цифрові сертифікати, штрих-коди, QR-коди, штампи або метадані. Підписи можна розміщувати на PDF-файлах, документах MS Word, робочих книгах MS Excel, презентаціях MS PowerPoint, файлах Adobe Photoshop і різних форматах зображень. Клієнти можуть підписувати свій документ і оновлювати, шукати, перевіряти, видаляти або переглядати електронні підписи, які були розміщені на цих документах. Крім того, передбачено безліч можливостей для налаштування підписів.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Кроки для підпису Xlsx за допомогою Metadata у Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) надає можливість швидко та легко підписувати документи Xlsx за допомогою підписів Metadata.
        
        * Створіть екземпляр класу підпису, який надає файл Xlsx, який має бути підписаний як шлях або потік пам’яті
        * Створіть екземпляр класу SignOptions і встановіть усі потрібні дані.
        * Викликати метод Signature.Sign(), передаючи вихідний файл Xlsx або потік пам’яті

    title_right: " Системні вимоги"
    content_right: |
        GroupDocs.Signature for Java підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Отримайте останню версію GroupDocs.Signature for Java від [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsx file
        String filePath = "input.xlsx";
        // Set up output file
        String outputFilePath = "output.xlsx";

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

        // sign Xlsx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Підпис документів Xlsx за допомогою Metadata Live Demo"
    content: |
       Підпишіть файл Xlsx різними підписами просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безкоштовна онлайн-демоверсія чекає на вас.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Інші підтримувані підписи Metadata для Java"
    content: |
        "Ви також можете підписати Xlsx іншими типами підписів. Перегляньте список нижче."
    format: 
       
       
back_to_top:
    enable: true
---