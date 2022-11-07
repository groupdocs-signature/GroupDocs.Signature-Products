---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dotx
productName: Java
lang: uk
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dotx for Java

############################# Head ############################
head_title: "Додавання цифрових електронних підписів до файлу Dotx за допомогою Java"
head_description: "Помістіть цифровий підпис у файл Dotx для Java за допомогою кількох рядків коду. Використовуйте API підпису документів GroupDocs, щоб підписувати десятки форматів файлів."

############################# Header ############################
title: "Файли eSign Dotx із підписами Digital у Java"
description: "Як додати підпис Digital за допомогою кількох рядків коду Java"
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
    title: "Про API цифрових підписів GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) — це популярний API для оформлення документів за допомогою цифрових електронних підписів із цифровими сертифікатами. API цифрових підписів використовує файли сертифікатів PFX для підписання документів із захищеними паролем закритими та відкритими ключами. Цифрові підписи можна використовувати для сертифікації бізнес-документів за допомогою окремої сторінки eSign PDF, сертифікації цілих документів Microsoft Office, таких як Words, Excel, файли Powerpoint і документи Open Office. Клієнти можуть легко маніпулювати підписами, наприклад редагувати їх, видаляти або коригувати. API надає спосіб пошуку та перевірки підписів. Крім того, передбачено безліч можливостей для налаштування підписів.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Кроки для підпису Dotx за допомогою Digital у Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) надає можливість швидко та легко підписувати документи Dotx за допомогою підписів Digital.
        
        * Створіть екземпляр класу підпису, який надає файл Dotx, який має бути підписаний як шлях або потік пам’яті
        * Створіть екземпляр класу SignOptions і встановіть усі потрібні дані.
        * Викликати метод Signature.Sign(), передаючи вихідний файл Dotx або потік пам’яті

    title_right: " Системні вимоги"
    content_right: |
        GroupDocs.Signature for Java підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Отримайте останню версію GroupDocs.Signature for Java від [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";
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

        // sign Dotx document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Підпис документів Dotx за допомогою Digital Live Demo"
    content: |
       Підпишіть файл Dotx різними підписами просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безкоштовна онлайн-демоверсія чекає на вас.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Інші підтримувані підписи Digital для Java"
    content: |
        "Ви також можете підписати Dotx іншими типами підписів. Перегляньте список нижче."
    format: 
       
       
back_to_top:
    enable: true
---