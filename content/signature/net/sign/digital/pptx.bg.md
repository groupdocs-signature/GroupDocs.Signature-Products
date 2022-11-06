---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Pptx
productName: .NET
lang: bg
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pptx for C#

############################# Head ############################
head_title: "Добавяне на цифрови електронни подписи към файл Pptx с C#"
head_description: "Поставете цифров подпис на файл Pptx за .NET, като използвате няколко реда код. Използвайте API на GroupDocs Document Signature, за да подписвате десетки файлови формати."

############################# Header ############################
title: "eSign Pptx файлове с Digital подписи в C#"
description: "Как да добавите подпис Digital с няколко реда код на .NET"
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
    title: "Относно API за цифрови подписи на GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) е популярен API за създаване на документи с цифрови електронни подписи, с цифрови сертификати. За цифровите подписи API използва PFX сертификатни файлове, за да подпише документ със защитени с парола частни и публични ключове. Цифровите подписи могат да се използват за сертифициране на бизнес документи с конкретна страница eSign PDF, за сертифициране на цели документи на Microsoft Office като Words, Excel, Powerpoint файлове и документи на Open Office. Клиентите могат лесно да манипулират подписите, като ги редактират, премахват или коригират. API предоставя начин за търсене и проверка на подписи. Освен това са предоставени много възможности за персонализиране на подписи.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Стъпки за подписване на Pptx с Digital в C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) предоставя възможност за бързо и лесно подписване на Pptx документи с Digital подписи.
        
        * Създайте екземпляр на клас подпис, предоставящ файл Pptx, който трябва да се подписва като път или поток от памет
        * Създайте клас SignOptions и задайте всички изисквани данни.
        * Извикване на метода Signature.Sign(), предаващ изходен файл Pptx или поток от памет

    title_right: " Системни изисквания"
    content_right: |
        GroupDocs.Signature for .NET се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Вземете най-новия GroupDocs.Signature for .NET от [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pptx file
        string filePath = "input.pptx";
        // Set up output file
        string outputFilePath = "output.pptx";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Pptx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписване на Pptx документи с Digital Демо на живо"
    content: |
       Подпишете файл Pptx с различни подписи точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безплатна онлайн демонстрация ви очаква.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Други поддържани подписи Digital за C#"
    content: |
        "Можете също да подпишете Pptx с други типове подписи. Моля, вижте списъка по-долу."
    format: 
       
       
back_to_top:
    enable: true
---