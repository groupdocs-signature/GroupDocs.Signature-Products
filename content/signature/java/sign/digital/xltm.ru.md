---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xltm
productName: Java
lang: ru
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xltm for Java

############################# Head ############################
head_title: "Добавление цифровых электронных подписей в файл Xltm с Java"
head_description: "Поместите цифровую подпись в файл Xltm для Java, используя несколько строк кода. Используйте API подписи документов GroupDocs для подписи десятков форматов файлов."

############################# Header ############################
title: "eSign Xltm файлов с подписями Digital в Java"
description: "Как добавить подпись Digital с помощью нескольких строк кода Java"
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
    title: "Об API цифровых подписей GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) — популярный API для оформления документов с помощью цифровых электронных подписей и цифровых сертификатов. Для API цифровых подписей используются файлы сертификатов PFX для создания документа с защищенными паролем закрытыми и открытыми ключами. Цифровые подписи могут использоваться для сертификации деловых документов с помощью eSign PDF на определенной странице, для сертификации целых документов Microsoft Office, таких как файлы Word, Excel, Powerpoint и документы Open Office. Клиенты могут легко манипулировать подписями, например редактировать их, удалять или корректировать. API предоставляет способ поиска и проверки подписей. Кроме того, предусмотрено множество возможностей для настройки подписей.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Действия по подписанию Xltm с помощью Digital в Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) позволяет быстро и легко подписывать документы Xltm с подписями Digital.
        
        * Создайте экземпляр класса Signature, предоставляющий файл Xltm, который должен быть подписан как путь или поток памяти.
        * Создайте экземпляр класса SignOptions и установите все требуемые данные.
        * Вызвать метод Signature.Sign(), передав выходной файл Xltm или поток памяти

    title_right: " Системные Требования"
    content_right: |
        GroupDocs.Signature for Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Получите последнюю версию GroupDocs.Signature for Java из [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltm file
        String filePath = "input.xltm";
        // Set up output file
        String outputFilePath = "output.xltm";
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

        // sign Xltm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание Xltm документов с помощью Digital Live Demo"
    content: |
       Подпишите файл Xltm с различными подписями прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Бесплатная онлайн-демонстрация ждет вас.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие поддерживаемые подписи Digital для Java"
    content: |
        "Вы также можете подписать Xltm другими типами подписи. См. список ниже."
    format: 
       
       
back_to_top:
    enable: true
---