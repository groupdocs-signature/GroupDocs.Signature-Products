---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Webp
productName: .NET
lang: bg
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Webp for C#

############################# Head ############################
head_title: "Проверка на Qrcode подписи за Webp файлове чрез C#"
head_description: "Използвайте само няколко реда от кода на .NET, за да проверите документите Webp и техните подписи Qrcode."

############################# Header ############################
title: "Qrcode проверка на подписи за Webp файлове"
description: "API за .NET предоставя възможност за проверка на Qrcode подписи в Webp документи. Проверката на електронните подписи във вашите Webp документи може да се извърши бързо и лесно."
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
    title_left: "Как да валидирате Qrcode подписи във вашия Webp документ"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) включва полезни функции като проверка на подписи Qrcode, поставени в Webp документи. Използвайте тази възможност без внедряване на допълнителен код.
        
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
                
        // Set up input Webp file
        string filePath = "input.webp";

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
    title: "Подписване с Qrcode подписи Демо на живо"
    content: |
       Добавете различни електронни подписи към файла Webp точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Проверете други Qrcode подписи с помощта на C#"
    content: |
        "Проверка на електронни подписи, поставени в различни документи. Проверете качеството на подписите в популярните файлови формати, както е показано по-долу."
    format: 
       
       
back_to_top:
    enable: true
---