---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Docm
productName: .NET
lang: uk
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Docm for C#

############################# Head ############################
head_title: "Оновіть підписи Image у файлах Docm за допомогою C#"
head_description: "Використовуйте простий і легкий для розуміння код .NET для оновлення підписів Image у підписаних документах Docm."

############################# Header ############################
title: "Редагувати та оновлювати підписи Image, розміщені у файлах Docm"
description: "API для .NET забезпечує функціональність для оновлення підписів Image у документах Docm. Швидко й легко оновлюйте електронні підписи у своїх документах Docm за допомогою кількох рядків коду C#."
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
    title: "Дізнайтеся про функції API GroupDocs.Signature for .NET"
    content: |
        Функціональність API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) містить широкий вибір засобів для обробки у форматах документів на вимогу за допомогою електронних підписів. Підтримується широкий спектр електронних підписів, таких як тексти, зображення, цифрові сертифікати, штрих-коди, QR-коди, штампи або метадані. Клієнти можуть додавати, видаляти, редагувати, перевіряти або шукати цифрові підписи в PDF-файлах, документах MS Word, робочих книгах MS Excel, презентаціях MS PowerPoint, файлах Adobe Photoshop і різних форматах зображень. Доступні численні корисні функції та налаштування.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Як змінити підписи Image у вашому документі Docm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) містить такі корисні функції, як оновлення підписів Image, розміщених у документах Docm. Це дозволяє змінювати функції підписів без додаткового коду.
        
        * Для початку створіть об’єкт Signature, передаючи як шлях параметра конструктора до документа, який має бути оновлений.
        * Потім створіть відповідний конкретний об’єкт підпису та налаштуйте його ідентифікатор і властивості, які потрібно змінити.
        * Нарешті, викликайте метод оновлення підпису, передаючи певний об’єкт підпису.
        * Процес оновлення результатів до вашого повідомлення.

    title_right: "Системні вимоги"
    content_right: |
        GroupDocs.Signature for .NET підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Завантажте останню версію GroupDocs.Signature for .NET з [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Docm file
        string filePath = "input.docm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                ImageSignature signatureToUpdate = new ImageSignature(id)
                {
                    // specify signature width
                    Width = 170,
                    // specify signature height
                    Height = 250,
                    // set left position
                    Left = 10,
                    // set top position
                    Top = 10
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
    title: "Оновлення підписів Image на сторінках документа – демонстрація в реальному часі"
    content: |
       Відредагуйте різні електронні підписи документа Docm прямо зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Оновіть різні підписи Image через C#"
    content: |
        "Редагування цифрових підписів, які розміщені в документах різних форматів. Оновіть дані підписів без додаткового коду."
    format: 
       
       
back_to_top:
    enable: true
---