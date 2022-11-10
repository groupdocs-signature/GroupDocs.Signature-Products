---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Pptx
productName: .NET
lang: bg
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Pptx for C#

############################# Head ############################
head_title: "Актуализирайте Image подписи, поставени във Pptx файлове с C#"
head_description: "Използвайте прост и лесен за разбиране код на .NET за актуализиране на подписи на Image в подписани документи Pptx."

############################# Header ############################
title: "Редактирайте и актуализирайте Image подписи, поставени във Pptx файлове"
description: "API за .NET предоставя функционалност за актуализиране на подписи на Image в документи на Pptx. Актуализирайте електронните подписи във вашите Pptx документи с няколко реда C# код бързо и лесно."
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
    title: "Научете за функциите на API на GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API функционалността съдържа богат избор от средства за обработка във формати на документи по заявка чрез използване на електронни подписи. Поддържат се широк спектър от електронни подписи като текстове, изображения, цифрови сертификати, баркодове, QR-кодове, печати или метаданни. Клиентите могат да добавят, премахват, редактират, валидират или търсят цифрови подписи в PDF файлове, документи на MS Word, работни книги на MS Excel, презентации на MS PowerPoint, файлове на Adobe Photoshop и различни формати на изображения. Налични са множество полезни функции и настройки.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как да промените Image подписи във вашия Pptx документ"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) включва полезни функции като актуализиране на Image подписи, поставени в Pptx документи. Това прави възможно промяната на функциите на подписите без допълнителен код.
        
        * Като начало създайте обект Signature, предаващ като път на параметър на конструктор към документ, който трябва да бъде актуализиран.
        * След това създайте подходящ конкретен обект на подпис и настройте неговия идентификатор и свойства, които трябва да бъдат променени.
        * И накрая, извикайте метода за актуализиране на Signature, предавайки определен обект на подпис.
        * Процес на актуализиране на резултатите до ваше известие.

    title_right: "Системни изисквания"
    content_right: |
        GroupDocs.Signature for .NET се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Изтеглете най-новата версия на GroupDocs.Signature for .NET от [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pptx file
        string filePath = "input.pptx";

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
    title: "Актуализиране на подписите Image на страниците на документа - Демо на живо"
    content: |
       Редактирайте различни електронни подписи на документа Pptx точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Актуализирайте различни Image подписи чрез C#"
    content: |
        "Редактиране на цифрови подписи, които се поставят в различни формати на документи. Актуализирайте данните за подписи без допълнителен код."
    format: 
       
       
back_to_top:
    enable: true
---