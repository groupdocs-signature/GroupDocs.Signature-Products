---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Dotx
productName: .NET
lang: ru
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Dotx with C#

############################# Head ############################
head_title: "Поиск подписей Metadata в файле Dotx в C#"
head_description: "Используйте .NET для поиска подписей Metadata в файлах Dotx с помощью нескольких строк кода."

############################# Header ############################
title: "Поиск подписей Metadata в файле Dotx"
description: "Собственный API .NET позволяет искать подписи Metadata в уже подписанных файлах Dotx. Выполните расширенный поиск электронной подписи в документах Dotx, используя несколько строк кода."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Об API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) предоставляет .NET API для обработки документов с использованием различных типов подписи, таких как тексты, изображения, цифровые сертификаты, штрих-коды, QR-коды, штампы или метаданные. Пользователи могут добавлять, удалять, обновлять, проверять или искать электронные подписи в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений с дополнительной поддержкой настройки свойств подписи по мере необходимости.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как искать подписи Metadata в Dotx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) упрощает разработчикам .NET поиск подписей Metadata в файлах Dotx из своих приложений, выполняя несколько простых шагов.
        
        * Создайте новый экземпляр класса Signature и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте экземпляр объекта SearchOptions в соответствии с вашими требованиями и укажите параметры поиска.
        * Вызовите метод Search экземпляра класса Signature и передайте ему SearchOptions.
        * Обрабатывайте результаты поиска в соответствии с вашими требованиями.

    title_right: "Системные Требования"
    content_right: |
        GroupDocs.Signature for .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Signature for .NET из [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Dotx file
        string filePath = "input.dotx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for Metadata signatures in Dotx document
                List<WordProcessingMetadataSignature> signatures = signature.Search<WordProcessingMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (WordProcessingMetadataSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание с помощью подписей Metadata Live Demo"
    content: |
       Добавьте различные электронные подписи к файлам Dotx прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Поиск других подписей Metadata с помощью C#"
    content: |
        "Поиск электронных подписей в различных документах. Найдите подписи одного из популярных форматов файлов, как показано ниже."
    format: 
           
       
back_to_top:
    enable: true
---