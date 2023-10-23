---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Zip
productName: .NET
lang: bg
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Zip with C#

############################# Head ############################
head_title: "Търсене на подписи Digital във файл Zip в C#"
head_description: "Използвайте .NET за търсене на подписи Digital във файлове Zip, като използвате няколко реда код."

############################# Header ############################
title: "Търсене на подписи Digital във файл Zip"
description: "Нативният API на .NET позволява търсене на подписи на Digital във вече подписани файлове на Zip. Извършете разширено търсене с електронен подпис във вашите Zip документи, като използвате няколко реда код."
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
    title_left: "Как да търсите Digital подписи във Zip"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) улеснява разработчиците на .NET да търсят подписи на Digital във файловете на Zip от техните приложения чрез прилагане на няколко лесни стъпки.
        
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
                
        // Set up input Zip file
        string filePath = "input.zip";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                DigitalSearchOptions options = new DigitalSearchOptions()
                {
                    // specify special search criteria
                    Comments = "Approved",
                    // specify date range period of signature
                    SignDateTimeFrom = new DateTime(year: 2020, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2020, month: 12, day: 31)
                };

                // search for Digital signatures in Zip document
                List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

                // process signatures which were found                
                foreach (DigitalSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Търсете Digital електронни подписи Демо на живо"
    content: |
       Потърсете в документа различни електронни подписи към Zip файлове точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Търсене на други Digital подписи с помощта на C#"
    content: |
        "Търсене на електронни подписи в различни документи. Намерете подписи от един от популярните файлови формати, както е показано по-долу."
    format: 
           
       
back_to_top:
    enable: true
---