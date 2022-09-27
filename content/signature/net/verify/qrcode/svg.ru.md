---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Svg
productName: .NET
lang: ru
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Svg for C#

############################# Head ############################
head_title: "Проверка подписей Qrcode для файлов Svg с помощью C#"
head_description: "Используйте всего несколько строк кода .NET для проверки документов Svg и их подписей Qrcode."

############################# Header ############################
title: "Проверка подписей Qrcode для Svg файлов"
description: "API для .NET предоставляет возможность проверять подписи Qrcode в документах Svg. Проверка электронных подписей внутри ваших документов Svg может быть выполнена быстро и легко."
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
    title: "Откройте для себя новые функции GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API предоставляет широкий спектр способов обработки различных форматов документов с использованием электронных подписей. Поддерживаются многие типы цифровых подписей, такие как тексты, изображения, цифровые сертификаты, штрих-коды, QR-коды, штампы или метаданные. Клиенты могут добавлять, удалять, редактировать, проверять или искать цифровые подписи в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений. Доступно невероятное количество дополнительных функций и настроек.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как проверить подписи Qrcode в документе Svg"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) содержит полезные функции, такие как проверка подписей Qrcode, размещенных в документах Svg. Используйте эту возможность, не внедряя дополнительный код.
        
        * Во-первых, создайте экземпляр класса Signature, указав в качестве параметра конструктора путь к документу, который должен быть проверен.
        * Во-вторых, создайте новый объект VerifyOptions и настройте все необходимые свойства.
        * Наконец, вызовите метод Verify объекта Signature, передав экземпляр VerifyOptions.
        * Затем обработайте результаты проверки.

    title_right: "Системные Требования"
    content_right: |
        GroupDocs.Signature for .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Signature for .NET из [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Svg file
        string filePath = "input.svg";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание с помощью подписей Qrcode Live Demo"
    content: |
       Добавьте различные электронные подписи в файл Svg прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Проверьте другие подписи Qrcode, используя C#"
    content: |
        "Проверка электронных подписей, размещенных в различных документах. Проверьте качество подписей в популярных форматах файлов, как показано ниже."
    format: 
       
       
back_to_top:
    enable: true
---