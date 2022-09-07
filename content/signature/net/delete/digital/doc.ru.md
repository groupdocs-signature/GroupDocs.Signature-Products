---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Doc
productName: .NET
lang: ru
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for C#

############################# Head ############################
head_title: "Удалите подписи Digital из Doc файлов с помощью C#"
head_description: "Удаление определенных подписей Digital из подписанных документов Doc можно легко выполнить с помощью короткого кода .NET."

############################# Header ############################
title: "Удалить подписи Digital, размещенные в файлах Doc"
description: "Удалите различные подписи Digital из Doc документов. Для удаления подписей Digital требуется простой код C#."
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
    title_left: "Как удалить подписи Digital из документа Doc"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) предоставляет полезную функцию для очистки документов Doc от подписей Digital с помощью нескольких строк кода.
        
        * Во-первых, создайте путь передачи объекта Signature к вашему документу в качестве параметра конструктора.
        * Затем создайте соответствующий объект подписи и настройте его уникальный идентификатор.
        * После этого вызовите метод Delete, передав объект подписи, который необходимо удалить.
        * Наконец, обработайте результаты операции.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Signature for .NET из [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

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
    title: "Подписание с помощью подписей Digital Live Demo"
    content: |
       Добавьте различные электронные подписи в файл Doc прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Удалите свои подписи Digital с помощью C#"
    content: |
        "Удаление электронных подписей, которые были добавлены к различным форматам документов. Удаляйте подписи быстро без дополнительного кода."
    format: 
       
       
back_to_top:
    enable: true
---