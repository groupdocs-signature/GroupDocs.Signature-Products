---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Text
fileformat: Doc
productName: .NET
lang: bg
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Doc for C#

############################# Head ############################
head_title: "Проверка на Text подписи за Doc файлове чрез C#"
head_description: "Използвайте само няколко реда от кода на .NET, за да проверите документите Doc и техните подписи Text."

############################# Header ############################
title: "Text проверка на подписи за Doc файлове"
description: "API за .NET предоставя възможност за проверка на Text подписи в Doc документи. Проверката на електронните подписи във вашите Doc документи може да се извърши бързо и лесно."
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
    title: "Открийте нови функции на API на GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API предоставя широка гама от начини за обработка на множество формати на документи чрез използване на електронни подписи. Поддържат се много видове цифрови подписи като текстове, изображения, цифрови сертификати, баркодове, QR-кодове, печати или метаданни. Клиентите могат да добавят, премахват, редактират, валидират или търсят цифрови подписи в PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint, файлове на Adobe Photoshop и различни формати на изображения. Налични са удивителен брой допълнителни функции и настройки.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как да валидирате Text подписи във вашия Doc документ"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) включва полезни функции като проверка на подписи Text, поставени в Doc документи. Използвайте тази възможност без внедряване на допълнителен код.
        
        * Първо, създайте клас Signature, предоставящ като параметър на конструктора път към документ, който трябва да бъде проверен.
        * Второ, създайте нов обект VerifyOptions и настройте всички необходими свойства.
        * И накрая, извикайте метода Verify на обекта Signature, като предавате екземпляр VerifyOptions.
        * След това обработете резултатите от проверката.

    title_right: "Системни изисквания"
    content_right: |
        GroupDocs.Signature for .NET се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Изтеглете най-новата версия на GroupDocs.Signature for .NET от [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                TextVerifyOptions options = new TextVerifyOptions()
                {
                    // Process all pages 
                    AllPages = true,
                    // set up text match type
                    MatchType = TextMatchType.Exact,
                    // specify text pattern to search
                    Text = "Very important signature",
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
    title: "Подписване с Text подписи Демо на живо"
    content: |
       Добавете различни електронни подписи към файла Doc точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Проверете други Text подписи с помощта на C#"
    content: |
        "Проверка на електронни подписи, поставени в различни документи. Проверете качеството на подписите в популярните файлови формати, както е показано по-долу."
    format: 
       
       
back_to_top:
    enable: true
---