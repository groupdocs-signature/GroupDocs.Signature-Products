---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Wmf
productName: .NET
lang: bg
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Wmf for C#

############################# Head ############################
head_title: "Създайте текстови електронни подписи към Wmf файл с C#"
head_description: "Поставете електронен подпис Text във файл Wmf за .NET, като използвате няколко реда код. Използвайте API на GroupDocs Document Signature, за да подписвате десетки файлови формати."

############################# Header ############################
title: "Подпишете Wmf файлове с Text подписи в C#"
description: "Как да добавите Text подпис с няколко реда код на .NET"
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
    title: "Относно API на GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) е популярен API за електронно подписване на цифрови документи. Налични са подписи като текстове, изображения, цифрови сертификати, баркодове, QR-кодове, печати или метаданни. Подписи могат да се поставят върху PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint, файлове на Adobe Photoshop и различни формати на изображения. Клиентите могат да подписват своя документ и да актуализират, търсят, проверяват, изтриват или визуализират електронни подписи, които са поставени върху тези документи. Освен това са предоставени много възможности за персонализиране на подписи.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Стъпки за подписване на Wmf с Text в C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) предоставя възможност за бързо и лесно подписване на Wmf документи с Text подписи.
        
        * Създайте екземпляр на клас подпис, предоставящ файл Wmf, който трябва да се подписва като път или поток от памет
        * Създайте клас SignOptions и задайте всички изисквани данни.
        * Извикване на метода Signature.Sign(), предаващ изходен файл Wmf или поток от памет

    title_right: " Системни изисквания"
    content_right: |
        GroupDocs.Signature for .NET се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Вземете най-новия GroupDocs.Signature for .NET от [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Wmf file
        string filePath = "input.wmf";
        // Set up output file
        string outputFilePath = "output.wmf";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Wmf document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписване на Wmf документи с Text Демо на живо"
    content: |
       Подпишете файл Wmf с различни подписи точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безплатна онлайн демонстрация ви очаква.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Други поддържани подписи Text за C#"
    content: |
        "Можете също да подпишете Wmf с други типове подписи. Моля, вижте списъка по-долу."
    format: 
       
       
back_to_top:
    enable: true
---