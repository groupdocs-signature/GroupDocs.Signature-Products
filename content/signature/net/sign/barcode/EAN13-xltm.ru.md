---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: E A N13
fileformat: Xltm
productName: .NET
lang: ru
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Xltm for C#

############################# Head ############################
head_title: "eSign Xltm документ со штрих-кодом E A N13 в C#"
head_description: "Создайте подпись штрих-кода E A N13 и поместите ее в документ Xltm с .NET, используя пару строк кода. Используйте API подписи документов GroupDocs для подписи файлов различных форматов."

############################# Header ############################
title: "Создайте подпись штрих-кода E A N13 для документа Xltm в C#"
description: "Подпишите свои бизнес-документы Xltm с помощью штрих-кода E A N13. Быстро и легко создавайте подпись штрих-кода с помощью нескольких строк кода для настройки параметров подписи."
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
    title: "Об API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) — это популярный API для электронной подписи цифровых документов с использованием многих типов штрих-кодов, таких как UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN, ITF14. и многие другие. Клиенты могут легко создавать штрих-коды, содержащие только необходимый текст, и размещать их в PDF-файлах, документах MS Word, рабочих книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений. Штрих-коды, размещенные в документах, можно обновлять, искать, проверять, удалять или предварительно просматривать. Кроме того, поддерживается настройка штрих-кодов.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Действия по подписанию Xltm с помощью Barcode в C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) позволяет быстро и легко подписывать документы Xltm с подписями Barcode.
        
        * Создайте экземпляр класса Signature, предоставляющий файл Xltm, который должен быть подписан как путь или поток памяти.
        * Создайте экземпляр класса SignOptions и установите все требуемые данные.
        * Вызвать метод Signature.Sign(), передав выходной файл Xltm или поток памяти

    title_right: "System Requirements"
    content_right: |
        Подписание документов с помощью GroupDocs.Signature for .NET можно выполнить всего за несколько простых шагов. Наши API поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Получите последнюю версию GroupDocs.Signature for .NET из [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Xltm file
        string filePath = "input.xltm";
        // Set up output file
        string outputFilePath = "output.xltm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.E A N13,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Xltm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание Xltm документов с помощью Barcode Live Demo"
    content: |
       Подпишите файл Xltm с различными подписями прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Бесплатная онлайн-демонстрация ждет вас.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About E A N13 Barcode"
          content: |
            Наиболее часто используемый стандарт EAN — это 13-значный EAN-13, надмножество исходного 12-значного стандарта универсального кода продукта.
          characterset: |
             Только числовые цифры (0-9).
          textcapacity: |
             Емкость кодового текста: ровно 12 цифр + 1 контрольная цифра.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAGwAAABjCAYAAAB+MOUYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAARpSURBVHhe7ZFBimBRCMT6/pfuUYaAi6pe58MLSJCAG39+H5/iPexjvId9jPewj/Ee9jHewz7Ge9jH+PNhPz//M4bdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXh5K3sM+xnvYx3gP+xjvYR/jPexT/P7+A4FOQDtpBhIBAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие поддерживаемые подписи Barcode для C#"
    content: |
        "Вы также можете подписать Xltm другими типами подписи. См. список ниже."
    format: 
           
       
back_to_top:
    enable: true
---