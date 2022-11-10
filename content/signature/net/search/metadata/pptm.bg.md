---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Pptm
productName: .NET
lang: bg
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Pptm with C#

############################# Head ############################
head_title: "Търсене на подписи Metadata във файл Pptm в C#"
head_description: "Използвайте .NET за търсене на подписи Metadata във файлове Pptm, като използвате няколко реда код."

############################# Header ############################
title: "Търсене на подписи Metadata във файл Pptm"
description: "Нативният API на .NET позволява търсене на подписи на Metadata във вече подписани файлове на Pptm. Извършете разширено търсене с електронен подпис във вашите Pptm документи, като използвате няколко реда код."
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
    title: "Относно API на GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) предоставя .NET API за обработка на документи, използвайки различни типове подписи, като текстове, изображения, цифрови сертификати, баркодове, QR-кодове, печати или метаданни. Потребителите могат да добавят, изтриват, актуализират, проверяват или търсят електронни подписи в PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint, файлове на Adobe Photoshop и различни формати на изображения, с допълнителна поддръжка за персонализиране на свойствата на подписите, ако е необходимо.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как да търсите Metadata подписи във Pptm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) улеснява разработчиците на .NET да търсят подписи на Metadata във файловете на Pptm от техните приложения чрез прилагане на няколко лесни стъпки.
        
        * Създайте нов екземпляр на клас Signature и подайте пътя на изходния документ като параметър на конструктора.
        * Създайте екземпляр на обекта SearchOptions според вашите изисквания и задайте опции за търсене.
        * Извикайте метода Search на екземпляра на класа Signature и му предайте SearchOptions.
        * Обработвайте резултатите от търсенето според вашите изисквания.

    title_right: "Системни изисквания"
    content_right: |
        GroupDocs.Signature for .NET се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Изтеглете най-новата версия на GroupDocs.Signature for .NET от [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Pptm file
        string filePath = "input.pptm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for Metadata signatures in Pptm document
                List<PresentationMetadataSignature> signatures = signature.Search<PresentationMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (PresentationMetadataSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Търсете Metadata електронни подписи Демо на живо"
    content: |
       Потърсете в документа различни електронни подписи към Pptm файлове точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Търсене на други Metadata подписи с помощта на C#"
    content: |
        "Търсене на електронни подписи в различни документи. Намерете подписи от един от популярните файлови формати, както е показано по-долу."
    format: 
           
       
back_to_top:
    enable: true
---