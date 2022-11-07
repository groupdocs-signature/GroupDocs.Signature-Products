---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Ods
productName: Java
lang: uk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Ods for Java

############################# Head ############################
head_title: "Додавання підписів Image до файлу Ods за допомогою Java"
head_description: "Додайте підпис Image до файлу Ods для Java за допомогою кількох рядків коду. Використовуйте API підпису документів GroupDocs, щоб підписувати десятки форматів файлів."

############################# Header ############################
title: "Підпишіть файли Ods підписами Image у Java"
description: "Як додати підпис Image із кількома рядками коду Java"
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
    title: "Про API підписів зображень GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) — популярний API для електронного підпису цифрових документів. Доступні такі підписи, як тексти, зображення, цифрові сертифікати, штрих-коди, QR-коди, штампи або метадані. Підписи можна розміщувати на PDF-файлах, документах MS Word, робочих книгах MS Excel, презентаціях MS PowerPoint, файлах Adobe Photoshop і різних форматах зображень. Клієнти можуть підписувати свій документ і оновлювати, шукати, перевіряти, видаляти або переглядати електронні підписи, які були розміщені на цих документах. Крім того, передбачено безліч можливостей для налаштування підписів.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Кроки для підпису Ods за допомогою Image у Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) надає можливість швидко та легко підписувати документи Ods за допомогою підписів Image.
        
        * Створіть екземпляр класу підпису, який надає файл Ods, який має бути підписаний як шлях або потік пам’яті
        * Створіть екземпляр класу SignOptions і встановіть усі потрібні дані.
        * Викликати метод Signature.Sign(), передаючи вихідний файл Ods або потік пам’яті

    title_right: " Системні вимоги"
    content_right: |
        GroupDocs.Signature for Java підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Отримайте останню версію GroupDocs.Signature for Java від [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";
        // Set up output file
        String outputFilePath = "output.ods";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Ods document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Підпис документів Ods за допомогою Image Live Demo"
    content: |
       Підпишіть файл Ods різними підписами просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безкоштовна онлайн-демоверсія чекає на вас.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Інші підтримувані підписи Image для Java"
    content: |
        "Ви також можете підписати Ods іншими типами підписів. Перегляньте список нижче."
    format: 
       
       
back_to_top:
    enable: true
---