---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Pptx
productName: .NET
lang: uk
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Pptx for C#

############################# Head ############################
head_title: "Додайте електронні підписи метаданих до документів Pptx за допомогою C#"
head_description: "Використовуйте метадані як приховані електронні підписи у своїх документах Pptx за допомогою кількох рядків коду C#. Використовуйте API підпису документів GroupDocs, щоб електронно підписувати свої бізнес-документи та файли з інформацією метаданих."

############################# Header ############################
title: "Електронні підписи метаданих для документа Pptx через .NET прості та легкі у використанні!"
description: "Електронно підписуйте свої Pptx документи та контракти за допомогою прихованих записів метаданих. Створюйте метадані для PDF-файлів, документів MS Word, робочих книг MS Excel, презентацій MS PowerPoint і різних форматів зображень без проблем і додаткового кодування."
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
    title: "Про API підписів метаданих GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) — популярний API для електронного підпису цифрових документів. Доступні такі підписи, як тексти, зображення, цифрові сертифікати, штрих-коди, QR-коди, штампи або метадані. Підписи можна розміщувати на PDF-файлах, документах MS Word, робочих книгах MS Excel, презентаціях MS PowerPoint, файлах Adobe Photoshop і різних форматах зображень. Клієнти можуть підписувати свій документ і оновлювати, шукати, перевіряти, видаляти або переглядати електронні підписи, які були розміщені на цих документах. Крім того, передбачено безліч можливостей для налаштування підписів.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Кроки для підпису Pptx за допомогою Metadata у C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) надає можливість швидко та легко підписувати документи Pptx за допомогою підписів Metadata.
        
        * Створіть екземпляр класу підпису, який надає файл Pptx, який має бути підписаний як шлях або потік пам’яті
        * Створіть екземпляр класу SignOptions і встановіть усі потрібні дані.
        * Викликати метод Signature.Sign(), передаючи вихідний файл Pptx або потік пам’яті

    title_right: " Системні вимоги"
    content_right: |
        GroupDocs.Signature for .NET підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Отримайте останню версію GroupDocs.Signature for .NET від [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Pptx file
        string filePath = "input.pptx";
        // Set up output file
        string outputFilePath = "output.pptx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Pptx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Підпис документів Pptx за допомогою Metadata Live Demo"
    content: |
       Підпишіть файл Pptx різними підписами просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безкоштовна онлайн-демоверсія чекає на вас.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Інші підтримувані підписи Metadata для C#"
    content: |
        "Ви також можете підписати Pptx іншими типами підписів. Перегляньте список нижче."
    format: 
       
       
back_to_top:
    enable: true
---