---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Svg
productName: .NET
lang: ru
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Svg for C#

############################# Head ############################
head_title: "Добавление электронных подписей метаданных к документам Svg через C#"
head_description: "Используйте метаданные в качестве скрытых электронных подписей внутри ваших документов Svg, используя пару строк кода C#. Используйте API подписи документов GroupDocs для электронной подписи бизнес-документов и файлов с информацией о метаданных."

############################# Header ############################
title: "Электронные подписи метаданных для документа Svg через .NET просты и удобны в использовании!"
description: "Электронная подпись документов и контрактов Svg со скрытыми записями метаданных. Создавайте метаданные для PDF-файлов, документов MS Word, книг MS Excel, презентаций MS PowerPoint и различных форматов изображений без проблем и дополнительного кодирования."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Об API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) — популярный API для электронной подписи цифровых документов. Доступны подписи, такие как тексты, изображения, цифровые сертификаты, штрих-коды, QR-коды, штампы или метаданные. Подписи могут быть размещены в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений. Клиенты могут подписывать свои документы, а также обновлять, искать, проверять, удалять или просматривать электронные подписи, поставленные в этих документах. Кроме того, предусмотрено множество возможностей для настройки подписей.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Действия по подписанию Svg с помощью Metadata в C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) позволяет быстро и легко подписывать документы Svg с подписями Metadata.
        
        * Создайте экземпляр класса Signature, предоставляющий файл Svg, который должен быть подписан как путь или поток памяти.
        * Создайте экземпляр класса SignOptions и установите все требуемые данные.
        * Вызвать метод Signature.Sign(), передав выходной файл Svg или поток памяти

    title_right: "System Requirements"
    content_right: |
        Подписание документов с помощью GroupDocs.Signature for .NET можно выполнить всего за несколько простых шагов. Наши API поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Получите последнюю версию GroupDocs.Signature for .NET из [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Svg file
        string filePath = "input.svg";
        // Set up output file
        string outputFilePath = "output.svg";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                MetadataSignOptions options = new MetadataSignOptions();

                // Specify different Metadata Signatures and add them to options signature collection
                // set start id
                ushort imgsMetadataId = 41996;
                // setup int value
                ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
                options.Signatures.Add(mdSign_DocId);
                // setup Author property
                ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
                options.Signatures.Add(mdSign_Author);
                // setup data of sign date
                ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, DateTime.Now); // DateTime
                options.Signatures.Add(mdSign_Date);
                // setup double
                ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456M); //decimal value
                options.Signatures.Add(mdSign_Amnt);

                // sign Svg document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание Svg документов с помощью Metadata Live Demo"
    content: |
       Подпишите файл Svg с различными подписями прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Бесплатная онлайн-демонстрация ждет вас.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие поддерживаемые подписи Metadata для C#"
    content: |
        "Вы также можете подписать Svg другими типами подписи. См. список ниже."
    format: 
       
       
back_to_top:
    enable: true
---