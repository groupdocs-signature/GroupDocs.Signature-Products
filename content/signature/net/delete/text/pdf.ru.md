---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Pdf
productName: .NET
lang: ru
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Pdf for C#

############################# Head ############################
head_title: "Удалите подписи Text из Pdf файлов с помощью C#"
head_description: "Удаление определенных подписей Text из подписанных документов Pdf можно легко выполнить с помощью короткого кода .NET."

############################# Header ############################
title: "Удалить подписи Text, размещенные в файлах Pdf"
description: "Удалите различные подписи Text из Pdf документов. Для удаления подписей Text требуется простой код C#."
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
    title: "Получить информацию о возможностях API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API предоставляет множество способов обработки ваших документов с помощью электронных подписей. Доступны цифровые подписи, такие как тексты, изображения, цифровые сертификаты, штрих-коды, QR-коды, штампы или метаданные. У клиентов есть возможность добавлять, удалять, обновлять, проверять или искать цифровые подписи в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений. Предусмотрено огромное количество полезных функций и настроек.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как удалить подписи Text из документа Pdf"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) предоставляет полезную функцию для очистки документов Pdf от подписей Text с помощью нескольких строк кода.
        
        * Во-первых, создайте путь передачи объекта Signature к вашему документу в качестве параметра конструктора.
        * Затем создайте соответствующий объект подписи и настройте его уникальный идентификатор.
        * После этого вызовите метод Delete, передав объект подписи, который необходимо удалить.
        * Наконец, обработайте результаты операции.

    title_right: "Системные Требования"
    content_right: |
        GroupDocs.Signature for .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Signature for .NET из [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pdf file
        string filePath = "input.pdf";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to delete
                // set up particular signature id
                TextSignature signatureToDelete = new TextSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание с помощью подписей Text Live Demo"
    content: |
       Добавьте различные электронные подписи в файл Pdf прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Удалите свои подписи Text с помощью C#"
    content: |
        "Удаление электронных подписей, которые были добавлены к различным форматам документов. Удаляйте подписи быстро без дополнительного кода."
    format: 
       
       
back_to_top:
    enable: true
---