---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Ods
productName: Java
lang: ru
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ods for Java

############################# Head ############################
head_title: "Проверка подписей Digital для файлов Ods с помощью Java"
head_description: "Используйте всего несколько строк кода Java для проверки документов Ods и их подписей Digital."

############################# Header ############################
title: "Проверка подписей Digital для Ods файлов"
description: "API для Java предоставляет возможность проверять подписи Digital в документах Ods. Проверка электронных подписей внутри ваших документов Ods может быть выполнена быстро и легко."
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
    title: "Откройте для себя новые функции GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API предоставляет широкий спектр способов обработки различных форматов документов с использованием электронных подписей. Поддерживаются многие типы цифровых подписей, такие как тексты, изображения, цифровые сертификаты, штрих-коды, QR-коды, штампы или метаданные. Клиенты могут добавлять, удалять, редактировать, проверять или искать цифровые подписи в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений. Доступно невероятное количество дополнительных функций и настроек.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как проверить подписи Digital в документе Ods"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) содержит полезные функции, такие как проверка подписей Digital, размещенных в документах Ods. Используйте эту возможность, не внедряя дополнительный код.
        
        * Во-первых, создайте экземпляр класса Signature, указав в качестве параметра конструктора путь к документу, который должен быть проверен.
        * Во-вторых, создайте новый объект VerifyOptions и настройте все необходимые свойства.
        * Наконец, вызовите метод Verify объекта Signature, передав экземпляр VerifyOptions.
        * Затем обработайте результаты проверки.

    title_right: "Системные Требования"
    content_right: |
        GroupDocs.Signature for Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Загрузите последнюю версию GroupDocs.Signature for Java из [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ods file
        String filePath = "input.ods";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание с помощью подписей Digital Live Demo"
    content: |
       Добавьте различные электронные подписи в файл Ods прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Проверьте другие подписи Digital, используя Java"
    content: |
        "Проверка электронных подписей, размещенных в различных документах. Проверьте качество подписей в популярных форматах файлов, как показано ниже."
    format: 
       
       
back_to_top:
    enable: true
---