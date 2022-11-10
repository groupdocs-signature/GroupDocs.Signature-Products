---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Odt
productName: .NET
lang: uk
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Odt for C#

############################# Head ############################
head_title: "Додавання цифрових електронних підписів до файлу Odt за допомогою C#"
head_description: "Помістіть цифровий підпис у файл Odt для .NET за допомогою кількох рядків коду. Використовуйте API підпису документів GroupDocs, щоб підписувати десятки форматів файлів."

############################# Header ############################
title: "Файли eSign Odt із підписами Digital у C#"
description: "Як додати підпис Digital за допомогою кількох рядків коду .NET"
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
    title: "Про API цифрових підписів GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) — це популярний API для оформлення документів за допомогою цифрових електронних підписів із цифровими сертифікатами. API цифрових підписів використовує файли сертифікатів PFX для підписання документів із захищеними паролем закритими та відкритими ключами. Цифрові підписи можна використовувати для сертифікації бізнес-документів за допомогою окремої сторінки eSign PDF, сертифікації цілих документів Microsoft Office, таких як Words, Excel, файли Powerpoint і документи Open Office. Клієнти можуть легко маніпулювати підписами, наприклад редагувати їх, видаляти або коригувати. API надає спосіб пошуку та перевірки підписів. Крім того, передбачено безліч можливостей для налаштування підписів.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Кроки для підпису Odt за допомогою Digital у C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) надає можливість швидко та легко підписувати документи Odt за допомогою підписів Digital.
        
        * Створіть екземпляр класу підпису, який надає файл Odt, який має бути підписаний як шлях або потік пам’яті
        * Створіть екземпляр класу SignOptions і встановіть усі потрібні дані.
        * Викликати метод Signature.Sign(), передаючи вихідний файл Odt або потік пам’яті

    title_right: " Системні вимоги"
    content_right: |
        GroupDocs.Signature for .NET підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Отримайте останню версію GroupDocs.Signature for .NET від [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Odt file
        string filePath = "input.odt";
        // Set up output file
        string outputFilePath = "output.odt";
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

                // sign Odt document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Підпис документів Odt за допомогою Digital Live Demo"
    content: |
       Підпишіть файл Odt різними підписами просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безкоштовна онлайн-демоверсія чекає на вас.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Інші підтримувані підписи Digital для C#"
    content: |
        "Ви також можете підписати Odt іншими типами підписів. Перегляньте список нижче."
    format: 
       
       
back_to_top:
    enable: true
---