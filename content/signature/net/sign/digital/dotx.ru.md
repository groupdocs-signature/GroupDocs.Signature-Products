---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dotx
productName: .NET
lang: ru
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dotx for C#

############################# Head ############################
head_title: "Добавление цифровых электронных подписей в файл Dotx с C#"
head_description: "Поместите цифровую подпись в файл Dotx для .NET, используя несколько строк кода. Используйте API подписи документов GroupDocs для подписи десятков форматов файлов."

############################# Header ############################
title: "eSign Dotx файлов с подписями Digital в C#"
description: "Как добавить подпись Digital с помощью нескольких строк кода .NET"
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
    title: "Об API цифровых подписей GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) — популярный API для оформления документов с помощью цифровых электронных подписей и цифровых сертификатов. Для API цифровых подписей используются файлы сертификатов PFX для создания документа с защищенными паролем закрытыми и открытыми ключами. Цифровые подписи могут использоваться для сертификации деловых документов с помощью eSign PDF на определенной странице, для сертификации целых документов Microsoft Office, таких как файлы Word, Excel, Powerpoint и документы Open Office. Клиенты могут легко манипулировать подписями, например редактировать их, удалять или корректировать. API предоставляет способ поиска и проверки подписей. Кроме того, предусмотрено множество возможностей для настройки подписей.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Действия по подписанию Dotx с помощью Digital в C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) позволяет быстро и легко подписывать документы Dotx с подписями Digital.
        
        * Создайте экземпляр класса Signature, предоставляющий файл Dotx, который должен быть подписан как путь или поток памяти.
        * Создайте экземпляр класса SignOptions и установите все требуемые данные.
        * Вызвать метод Signature.Sign(), передав выходной файл Dotx или поток памяти

    title_right: " Системные Требования"
    content_right: |
        GroupDocs.Signature for .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Получите последнюю версию GroupDocs.Signature for .NET из [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotx file
        string filePath = "input.dotx";
        // Set up output file
        string outputFilePath = "output.dotx";
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

                // sign Dotx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание Dotx документов с помощью Digital Live Demo"
    content: |
       Подпишите файл Dotx с различными подписями прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Бесплатная онлайн-демонстрация ждет вас.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие поддерживаемые подписи Digital для C#"
    content: |
        "Вы также можете подписать Dotx другими типами подписи. См. список ниже."
    format: 
       
       
back_to_top:
    enable: true
---