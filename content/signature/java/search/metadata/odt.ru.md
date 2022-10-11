---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Odt
productName: Java
lang: ru
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Odt with Java

############################# Head ############################
head_title: "Поиск подписей Metadata в файле Odt в Java"
head_description: "Используйте Java для поиска подписей Metadata в файлах Odt с помощью нескольких строк кода."

############################# Header ############################
title: "Поиск подписей Metadata в файле Odt"
description: "Собственный API Java позволяет искать подписи Metadata в уже подписанных файлах Odt. Выполните расширенный поиск электронной подписи в документах Odt, используя несколько строк кода."
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
    title: "Об API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) предоставляет Java API для обработки документов с использованием различных типов подписи, таких как тексты, изображения, цифровые сертификаты, штрих-коды, QR-коды, штампы или метаданные. Пользователи могут добавлять, удалять, обновлять, проверять или искать электронные подписи в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений с дополнительной поддержкой настройки свойств подписи по мере необходимости.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как искать подписи Metadata в Odt"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) упрощает разработчикам Java поиск подписей Metadata в файлах Odt из своих приложений, выполняя несколько простых шагов.
        
        * Создайте новый экземпляр класса Signature и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте экземпляр объекта SearchOptions в соответствии с вашими требованиями и укажите параметры поиска.
        * Вызовите метод Search экземпляра класса Signature и передайте ему SearchOptions.
        * Обрабатывайте результаты поиска в соответствии с вашими требованиями.

    title_right: "Системные Требования"
    content_right: |
        GroupDocs.Signature for Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Загрузите последнюю версию GroupDocs.Signature for Java из [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Odt file
        String filePath = "input.odt";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // search for Metadata signatures in Odt document
        List<WordProcessingMetadataSignature> signatures = signature.search(WordProcessingMetadataSignature.class, SignatureType.Metadata);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));


        ```

############################# Demos ############################
demos:
    enable: true
    title: "Поиск электронных подписей Metadata Live Demo"
    content: |
       Найдите в документе различные электронные подписи к Odt файлам прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Поиск других подписей Metadata с помощью Java"
    content: |
        "Поиск электронных подписей в различных документах. Найдите подписи одного из популярных форматов файлов, как показано ниже."
    format: 
           
       
back_to_top:
    enable: true
---