---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: Data Matrix
fileformat: Ots
productName: .NET
lang: ru
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Ots for C#

############################# Head ############################
head_title: "eSign Ots документ с QR-кодом Data Matrix в C#"
head_description: "Создайте QR-код Data Matrix и поместите его в файл Ots, используя .NET с коротким фрагментом кода C#. Используйте API подписи документов GroupDocs для электронной подписи ваших деловых документов и файлов с помощью QR-кода."

############################# Header ############################
title: "Создайте подпись QR-кода Data Matrix для документа Ots в C#"
description: "Электронная подпись Ots документов и контрактов с Data Matrix QR-кодом. Создавайте подпись QR-кода быстро и легко."
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
    title: "Об API подписи QR-кода GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) — это зрелый API для создания и создания подписей QR-кода для документов. Пользователи могут генерировать подписи QR-кода, предоставляя текст для его загрузки или публикации в социальных сетях в виде изображения. Подписанный документ можно отсканировать через API или просто через мобильную камеру! Подписывайте в электронном виде свои деловые контракты и официальные документы, добавляя подпись QR-кода, и манипулируйте ею. Любая подпись QR-кода будет содержать уникальную пользовательскую информацию для идентификации подписавшего или авторизации документа. Кроме того, содержимое QR-кода может быть зашифровано и расшифровано с помощью личных ключей программно. Это открывает множество возможностей для обмена конфиденциальными данными в общедоступных документах. После подписания пользователь может обновлять, проверять, удалять, просматривать или искать QR-коды в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений. QR-коды могут быть дополнительно настроены.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Действия по подписанию Ots с помощью Qrcode в C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) позволяет быстро и легко подписывать документы Ots с подписями Qrcode.
        
        * Создайте экземпляр класса Signature, предоставляющий файл Ots, который должен быть подписан как путь или поток памяти.
        * Создайте экземпляр класса SignOptions и установите все требуемые данные.
        * Вызвать метод Signature.Sign(), передав выходной файл Ots или поток памяти

    title_right: " Системные Требования"
    content_right: |
        GroupDocs.Signature for .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Получите последнюю версию GroupDocs.Signature for .NET из [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ots file
        string filePath = "input.ots";
        // Set up output file
        string outputFilePath = "output.ots";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined QrCode text
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // setup QrCode encoding type
                    EncodeType = QrCodeTypes.Data Matrix,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign Ots document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание Ots документов с помощью Qrcode Live Demo"
    content: |
       Подпишите файл Ots с различными подписями прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Бесплатная онлайн-демонстрация ждет вас.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Data Matrix QrCode"
          content: |
            Матрица данных — это двумерный код, состоящий из черных и белых «ячеек» или точек, расположенных в виде квадрата или прямоугольника, также известный как матрица. Кодируемая информация может быть текстовой или числовой.
          characterset: |
             Поддерживает все 256 символов ASCII, все символы ISO и все символы расширенного двоично-десятичного кода обмена (EBCDIC).
          textcapacity: |
             До 3116 цифровых цифр, или 2335 буквенно-цифровых символов, или 1556 двоичных символов.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие поддерживаемые подписи Qrcode для C#"
    content: |
        "Вы также можете подписать Ots другими типами подписи. См. список ниже."
    format: 
        
       
back_to_top:
    enable: true
---