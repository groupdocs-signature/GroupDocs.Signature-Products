---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Docm
productName: Java
lang: uk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Docm for Java

############################# Head ############################
head_title: "Документ eSign Docm зі штрих-кодом Interleaved2of5 у Java"
head_description: "Створіть підпис штрих-коду Interleaved2of5 і додайте його в документ Docm за допомогою Java за допомогою кількох рядків коду. Використовуйте API підпису документів GroupDocs для підпису різних форматів файлів."

############################# Header ############################
title: "Згенеруйте підпис штрих-коду Interleaved2of5 для документа Docm у Java"
description: "Електронно підписуйте свої ділові документи Docm штрих-кодом Interleaved2of5. Згенеруйте підпис штрих-коду швидко та легко за допомогою кількох рядків коду, щоб налаштувати параметри підпису."
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
    title_left: "Кроки для підпису Docm за допомогою Barcode у Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) надає можливість швидко та легко підписувати документи Docm за допомогою підписів Barcode.
        
        * Створіть екземпляр класу підпису, який надає файл Docm, який має бути підписаний як шлях або потік пам’яті
        * Створіть екземпляр класу SignOptions і встановіть усі потрібні дані.
        * Викликати метод Signature.Sign(), передаючи вихідний файл Docm або потік пам’яті

    title_right: " Системні вимоги"
    content_right: |
        GroupDocs.Signature for Java підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Отримайте останню версію GroupDocs.Signature for Java від [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";
        // Set up output file
        String outputFilePath = "output.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Interleaved2of5);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Docm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Підпис документів Docm за допомогою Barcode Live Demo"
    content: |
       Підпишіть файл Docm різними підписами просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безкоштовна онлайн-демоверсія чекає на вас.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) — це безперервний штриховий код двох ширин, що кодує цифри. Він комерційно використовується на плівці 135, для штрих-кодів ITF-14 і на коробках деяких продуктів, тоді як продукти всередині маркуються UPC або EAN.
          characterset: |
             Числові цифри (0-9).
          textcapacity: |
             Змінна довжина.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Інші підтримувані підписи Barcode для Java"
    content: |
        "Ви також можете підписати Docm іншими типами підписів. Перегляньте список нижче."
    format: 
        
       
back_to_top:
    enable: true
---