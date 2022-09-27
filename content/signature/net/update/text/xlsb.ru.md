---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Xlsb
productName: .NET
lang: ru
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Xlsb for C#

############################# Head ############################
head_title: "Обновите подписи Text, размещенные в файлах Xlsb, с помощью C#"
head_description: "Используйте простой и понятный код .NET для обновления подписей Text в подписанных документах Xlsb."

############################# Header ############################
title: "Редактировать и обновлять подписи Text, размещенные в файлах Xlsb"
description: "API для .NET предоставляет функциональные возможности для обновления подписей Text в документах Xlsb. Быстро и легко обновляйте электронные подписи внутри ваших документов Xlsb с помощью пары строк кода C#."
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
    title: "Узнайте о возможностях API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) Функциональность API содержит широкий выбор средств для обработки востребованных форматов документов с использованием электронных подписей. Поддерживается широкий спектр электронных подписей, таких как тексты, изображения, цифровые сертификаты, штрих-коды, QR-коды, штампы или метаданные. Клиенты могут добавлять, удалять, редактировать, проверять или искать цифровые подписи в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений. Доступны многочисленные полезные функции и настройки.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как изменить подписи Text в документе Xlsb"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) содержит полезные функции, такие как обновление подписей Text, размещенных в документах Xlsb. Это позволяет изменять функции подписи без дополнительного кода.
        
        * Для начала создайте объект Signature, передав в качестве параметра конструктора путь к документу, который предполагается обновить.
        * Затем создайте экземпляр соответствующего конкретного объекта подписи и настройте его идентификатор и свойства, которые необходимо изменить.
        * Наконец, вызовите метод Update подписи, передав конкретный объект подписи.
        * Обработайте результаты обновления до вашего уведомления.

    title_right: "Системные Требования"
    content_right: |
        GroupDocs.Signature for .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Signature for .NET из [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsb file
        string filePath = "input.xlsb";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                TextSignature signatureToUpdate = new TextSignature(id)
                {
                    // specify signature width
                    Width = 130,
                    // specify signature height
                    Height = 20,
                    // set left position
                    Left = 40,
                    // set top position
                    Top = 50,
                    // set up new text
                    Text = "Mr. John Smith"
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание с помощью подписей Text Live Demo"
    content: |
       Добавьте различные электронные подписи в файл Xlsb прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Обновите различные подписи Text через C#"
    content: |
        "Редактирование цифровых подписей, размещенных в различных форматах документов. Обновление данных подписей без дополнительного кода."
    format: 
       
       
back_to_top:
    enable: true
---