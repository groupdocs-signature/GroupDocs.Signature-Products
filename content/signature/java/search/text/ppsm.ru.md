---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Ppsm
productName: Java
lang: ru
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Ppsm with Java

############################# Head ############################
head_title: "Поиск подписей Text в файле Ppsm в Java"
head_description: "Используйте Java для поиска подписей Text в файлах Ppsm с помощью нескольких строк кода."

############################# Header ############################
title: "Поиск подписей Text в файле Ppsm"
description: "Собственный API Java позволяет искать подписи Text в уже подписанных файлах Ppsm. Выполните расширенный поиск электронной подписи в документах Ppsm, используя несколько строк кода."
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
    title_left: "Как искать подписи Text в Ppsm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) упрощает разработчикам Java поиск подписей Text в файлах Ppsm из своих приложений, выполняя несколько простых шагов.
        
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
                
        // Set up input Ppsm file
        String filePath = "input.ppsm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        TextSearchOptions options = new TextSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
                            
        // search for Text signatures in Ppsm document
        List<TextSignature> signatures = signature.search(TextSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Поиск электронных подписей Text Live Demo"
    content: |
       Найдите в документе различные электронные подписи к Ppsm файлам прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Поиск других подписей Text с помощью Java"
    content: |
        "Поиск электронных подписей в различных документах. Найдите подписи одного из популярных форматов файлов, как показано ниже."
    format: 
           
       
back_to_top:
    enable: true
---