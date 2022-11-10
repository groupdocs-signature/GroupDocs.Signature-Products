---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Ppsm
productName: .NET
lang: bg
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ppsm for C#

############################# Head ############################
head_title: "eSign Ppsm документ с Interleaved2of5 баркод в C#"
head_description: "Създайте Interleaved2of5 баркод подпис и го поставете в Ppsm документ с .NET, като използвате няколко реда код. Използвайте API на GroupDocs Document Signature за подписване на различни файлови формати."

############################# Header ############################
title: "Генерирайте Interleaved2of5 баркод подпис за документ Ppsm в C#"
description: "Електронно подпишете вашите Ppsm бизнес документи с Interleaved2of5 баркод. Генерирайте баркод подпис бързо и лесно с няколко реда код, за да зададете опции за подписване."
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
    title: "Относно API за подписи на баркодове на GroupDocs.Signature for .NET."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) е бърз и лесен API за управление на електронно подписване на цифрови документи с помощта на типове баркодове като UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 и много други. Клиентите могат лесно да създават баркодове, предоставящи необходимия текст, и да ги поставят в PDF, Microsoft Office Words документи, Microsoft Office Excel работни книги, MS PowerPoint презентации, Adobe Photoshop файлове и различни формати на изображения. Баркодовете, поставени в документи, могат да бъдат актуализирани, търсени, потвърдени, изтрити или визуализирани. Освен това се поддържа персонализиране на баркодове.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Стъпки за подписване на Ppsm с Barcode в C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) предоставя възможност за бързо и лесно подписване на Ppsm документи с Barcode подписи.
        
        * Създайте екземпляр на клас подпис, предоставящ файл Ppsm, който трябва да се подписва като път или поток от памет
        * Създайте клас SignOptions и задайте всички изисквани данни.
        * Извикване на метода Signature.Sign(), предаващ изходен файл Ppsm или поток от памет

    title_right: " Системни изисквания"
    content_right: |
        GroupDocs.Signature for .NET се поддържат от всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.

        * Операционни системи: Microsoft Windows, Linux, MacOS
        * Среди за разработка: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Вземете най-новия GroupDocs.Signature for .NET от [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Ppsm file
        string filePath = "input.ppsm";
        // Set up output file
        string outputFilePath = "output.ppsm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Interleaved2of5,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Ppsm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписване на Ppsm документи с Barcode Демо на живо"
    content: |
       Подпишете файл Ppsm с различни подписи точно сега, като посетите уебсайта [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безплатна онлайн демонстрация ви очаква.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF) е непрекъсната символика на баркод с две ширини, кодираща цифри. Използва се в търговската мрежа на филм 135, за баркодове ITF-14 и върху картонени кутии на някои продукти, докато продуктите вътре са етикетирани с UPC или EAN.
          characterset: |
             Цифри (0-9).
          textcapacity: |
             Променлива дължина.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Други поддържани подписи Barcode за C#"
    content: |
        "Можете също да подпишете Ppsm с други типове подписи. Моля, вижте списъка по-долу."
    format: 
        
       
back_to_top:
    enable: true
---