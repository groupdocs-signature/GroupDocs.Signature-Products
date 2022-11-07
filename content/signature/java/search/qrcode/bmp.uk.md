---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Bmp
productName: Java
lang: uk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Bmp with Java

############################# Head ############################
head_title: "Шукайте підписи Qrcode у файлі Bmp у Java"
head_description: "Використовуйте Java для пошуку підписів Qrcode у файлах Bmp за допомогою кількох рядків коду."

############################# Header ############################
title: "Шукайте підписи Qrcode у файлі Bmp"
description: "Власний API Java дозволяє шукати підписи Qrcode у вже підписаних файлах Bmp. Виконайте розширений пошук електронного підпису в документах Bmp за допомогою кількох рядків коду."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Про API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) надає API Java для обробки документів з використанням різних типів підписів, таких як тексти, зображення, цифрові сертифікати, штрих-коди, QR-коди, штампи або метадані. Користувачі можуть додавати, видаляти, оновлювати, перевіряти або шукати електронні підписи в PDF-файлах, документах MS Word, робочих книгах MS Excel, презентаціях MS PowerPoint, файлах Adobe Photoshop і різних форматах зображень, з додатковою підтримкою налаштування властивостей підписів за потреби.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Як шукати підписи Qrcode у Bmp"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) полегшує розробникам Java пошук підписів Qrcode у файлах Bmp у їхніх програмах, виконавши кілька простих кроків.
        
        * Створіть новий екземпляр класу підпису та передайте шлях до вихідного документа як параметр конструктора.
        * Створіть екземпляр об’єкта SearchOptions відповідно до ваших вимог і вкажіть параметри пошуку.
        * Викличте метод Search екземпляра класу Signature і передайте йому SearchOptions.
        * Обробляйте результати пошуку відповідно до ваших вимог.

    title_right: "Системні вимоги"
    content_right: |
        GroupDocs.Signature for Java підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Завантажте останню версію GroupDocs.Signature for Java з [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Bmp file
        String filePath = "input.bmp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Bmp document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Шукайте електронні підписи Qrcode Демонстрація в реальному часі"
    content: |
       Знайдіть у документі різні електронні підписи до файлів Bmp просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Шукайте інші підписи Qrcode за допомогою Java"
    content: |
        "Пошук електронних підписів у різних документах. Знайдіть підписи в одному з популярних форматів файлів, як показано нижче."
    format: 
           
       
back_to_top:
    enable: true
---