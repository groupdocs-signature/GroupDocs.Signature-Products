---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Doc
productName: .NET
lang: uk
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Doc with C#

############################# Head ############################
head_title: "Шукайте підписи Digital у файлі Doc у C#"
head_description: "Використовуйте .NET для пошуку підписів Digital у файлах Doc за допомогою кількох рядків коду."

############################# Header ############################
title: "Шукайте підписи Digital у файлі Doc"
description: "Власний API .NET дозволяє шукати підписи Digital у вже підписаних файлах Doc. Виконайте розширений пошук електронного підпису в документах Doc за допомогою кількох рядків коду."
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
    title: "Про API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) надає API .NET для обробки документів з використанням різних типів підписів, таких як тексти, зображення, цифрові сертифікати, штрих-коди, QR-коди, штампи або метадані. Користувачі можуть додавати, видаляти, оновлювати, перевіряти або шукати електронні підписи в PDF-файлах, документах MS Word, робочих книгах MS Excel, презентаціях MS PowerPoint, файлах Adobe Photoshop і різних форматах зображень, з додатковою підтримкою налаштування властивостей підписів за потреби.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Як шукати підписи Digital у Doc"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) полегшує розробникам .NET пошук підписів Digital у файлах Doc у їхніх програмах, виконавши кілька простих кроків.
        
        * Створіть новий екземпляр класу підпису та передайте шлях до вихідного документа як параметр конструктора.
        * Створіть екземпляр об’єкта SearchOptions відповідно до ваших вимог і вкажіть параметри пошуку.
        * Викличте метод Search екземпляра класу Signature і передайте йому SearchOptions.
        * Обробляйте результати пошуку відповідно до ваших вимог.

    title_right: "Системні вимоги"
    content_right: |
        GroupDocs.Signature for .NET підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Завантажте останню версію GroupDocs.Signature for .NET з [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";

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

                // search for Digital signatures in Doc document
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
    title: "Шукайте електронні підписи Digital Демонстрація в реальному часі"
    content: |
       Знайдіть у документі різні електронні підписи до файлів Doc просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Шукайте інші підписи Digital за допомогою C#"
    content: |
        "Пошук електронних підписів у різних документах. Знайдіть підписи в одному з популярних форматів файлів, як показано нижче."
    format: 
           
       
back_to_top:
    enable: true
---