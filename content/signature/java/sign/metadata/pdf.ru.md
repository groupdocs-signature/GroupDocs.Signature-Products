---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Pdf
productName: Java
lang: ru
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Pdf for Java

############################# Head ############################
head_title: "Добавление электронных подписей метаданных к документам Pdf через Java"
head_description: "Используйте метаданные в качестве скрытых электронных подписей внутри ваших документов Pdf, используя пару строк кода Java. Используйте API подписи документов GroupDocs для электронной подписи бизнес-документов и файлов с информацией о метаданных."

############################# Header ############################
title: "Электронные подписи метаданных для документа Pdf через Java просты и удобны в использовании!"
description: "Электронная подпись документов и контрактов Pdf со скрытыми записями метаданных. Создавайте метаданные для PDF-файлов, документов MS Word, книг MS Excel, презентаций MS PowerPoint и различных форматов изображений без проблем и дополнительного кодирования."
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
    title: "Об API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) — популярный API для электронной подписи цифровых документов. Доступны подписи, такие как тексты, изображения, цифровые сертификаты, штрих-коды, QR-коды, штампы или метаданные. Подписи могут быть размещены в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений. Клиенты могут подписывать свои документы, а также обновлять, искать, проверять, удалять или просматривать электронные подписи, поставленные в этих документах. Кроме того, предусмотрено множество возможностей для настройки подписей.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Действия по подписанию Pdf с помощью Metadata в Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) позволяет быстро и легко подписывать документы Pdf с подписями Metadata.
        
        * Создайте экземпляр класса Signature, предоставляющий файл Pdf, который должен быть подписан как путь или поток памяти.
        * Создайте экземпляр класса SignOptions и установите все требуемые данные.
        * Вызвать метод Signature.Sign(), передав выходной файл Pdf или поток памяти

    title_right: "System Requirements"
    content_right: |
        Подписание документов с помощью GroupDocs.Signature for Java можно выполнить всего за несколько простых шагов. Наши API поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Получите последнюю версию GroupDocs.Signature for Java из [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pdf file
        String filePath = "input.pdf";
        // Set up output file
        String outputFilePath = "output.pdf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        PdfMetadataSignature mdSign_Author = new PdfMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        PdfMetadataSignature mdSign_DocData = new PdfMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        PdfMetadataSignature mdSign_DocId = new PdfMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Pdf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание Pdf документов с помощью Metadata Live Demo"
    content: |
       Подпишите файл Pdf с различными подписями прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Бесплатная онлайн-демонстрация ждет вас.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие поддерживаемые подписи Metadata для Java"
    content: |
        "Вы также можете подписать Pdf другими типами подписи. См. список ниже."
    format: 
       
       
back_to_top:
    enable: true
---