---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: E A N14
fileformat: 7z
productName: Java
lang: uk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on 7z for Java

############################# Head ############################
head_title: "Документ eSign 7z зі штрих-кодом E A N14 у Java"
head_description: "Створіть підпис штрих-коду E A N14 і додайте його в документ 7z за допомогою Java за допомогою кількох рядків коду. Використовуйте API підпису документів GroupDocs для підпису різних форматів файлів."

############################# Header ############################
title: "Згенеруйте підпис штрих-коду E A N14 для документа 7z у Java"
description: "Електронно підписуйте свої ділові документи 7z штрих-кодом E A N14. Згенеруйте підпис штрих-коду швидко та легко за допомогою кількох рядків коду, щоб налаштувати параметри підпису."
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
    title: "Про API підписів штрих-кодів GroupDocs.Signature for Java."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) — це швидкий і простий API для керування електронним підписом цифрових документів за допомогою таких типів штрих-кодів, як UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 та багато інших. Клієнти можуть легко створювати штрих-коди з необхідним текстом і розміщувати їх у PDF, документах Microsoft Office Words, робочих книгах Microsoft Office Excel, презентаціях MS PowerPoint, файлах Adobe Photoshop і різних форматах зображень. Штрих-коди, розміщені в документах, можна оновлювати, шукати, перевіряти, видаляти або переглядати. Крім того, підтримується налаштування штрих-кодів.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Кроки для підпису 7z за допомогою Barcode у Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) надає можливість швидко та легко підписувати документи 7z за допомогою підписів Barcode.
        
        * Створіть екземпляр класу підпису, який надає файл 7z, який має бути підписаний як шлях або потік пам’яті
        * Створіть екземпляр класу SignOptions і встановіть усі потрібні дані.
        * Викликати метод Signature.Sign(), передаючи вихідний файл 7z або потік пам’яті

    title_right: " Системні вимоги"
    content_right: |
        GroupDocs.Signature for Java підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Отримайте останню версію GroupDocs.Signature for Java від [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input 7z file
        String filePath = "input.7z";
        // Set up output file
        String outputFilePath = "output.7z";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.E A N14);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign 7z document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Підпис документів 7z за допомогою Barcode Live Demo"
    content: |
       Підпишіть файл 7z різними підписами просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безкоштовна онлайн-демоверсія чекає на вас.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About E A N14 Barcode"
          content: |
            Європейський номер товару або EAN — це стандарт, що описує символіку штрих-коду та систему нумерації, яка використовується у світовій торгівлі для ідентифікації конкретного типу роздрібного продукту в певній конфігурації упаковки від конкретного виробника.
          characterset: |
             Цифри (0-9) і спеціальні символи.
          textcapacity: |
             Рівно 14 цифр.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Інші підтримувані підписи Barcode для Java"
    content: |
        "Ви також можете підписати 7z іншими типами підписів. Перегляньте список нижче."
    format: 
        
       
back_to_top:
    enable: true
---