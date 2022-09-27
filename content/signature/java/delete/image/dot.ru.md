---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Dot
productName: Java
lang: ru
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Dot for Java

############################# Head ############################
head_title: "Удалите подписи Image из Dot файлов с помощью Java"
head_description: "Удаление определенных подписей Image из подписанных документов Dot можно легко выполнить с помощью короткого кода Java."

############################# Header ############################
title: "Удалить подписи Image, размещенные в файлах Dot"
description: "Удалите различные подписи Image из Dot документов. Для удаления подписей Image требуется простой код Java."
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
    title: "Получить информацию о возможностях API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API предоставляет множество способов обработки ваших документов с помощью электронных подписей. Доступны цифровые подписи, такие как тексты, изображения, цифровые сертификаты, штрих-коды, QR-коды, штампы или метаданные. У клиентов есть возможность добавлять, удалять, обновлять, проверять или искать цифровые подписи в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений. Предусмотрено огромное количество полезных функций и настроек.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как удалить подписи Image из документа Dot"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) предоставляет полезную функцию для очистки документов Dot от подписей Image с помощью нескольких строк кода.
        
        * Во-первых, создайте путь передачи объекта Signature к вашему документу в качестве параметра конструктора.
        * Затем создайте соответствующий объект подписи и настройте его уникальный идентификатор.
        * После этого вызовите метод Delete, передав объект подписи, который необходимо удалить.
        * Наконец, обработайте результаты операции.

    title_right: "Системные Требования"
    content_right: |
        GroupDocs.Signature for Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Загрузите последнюю версию GroupDocs.Signature for Java из [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dot file
        String filePath = "input.dot";
        // Set up output file
        String outputFilePath = "output.dot";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

        // provide signature features to delete
        ImageSignature signatureToDelete = new ImageSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание с помощью подписей Image Live Demo"
    content: |
       Добавьте различные электронные подписи в файл Dot прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Удалите свои подписи Image с помощью Java"
    content: |
        "Удаление электронных подписей, которые были добавлены к различным форматам документов. Удаляйте подписи быстро без дополнительного кода."
    format: 
       
       
back_to_top:
    enable: true
---