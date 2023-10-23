---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: Aztec
fileformat: Tar
productName: .NET
lang: ru
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Tar for C#

############################# Head ############################
head_title: "eSign Tar документ с QR-кодом Aztec в C#"
head_description: "Создайте QR-код Aztec и поместите его в файл Tar, используя .NET с коротким фрагментом кода C#. Используйте API подписи документов GroupDocs для электронной подписи ваших деловых документов и файлов с помощью QR-кода."

############################# Header ############################
title: "Создайте подпись QR-кода Aztec для документа Tar в C#"
description: "Электронная подпись Tar документов и контрактов с Aztec QR-кодом. Создавайте подпись QR-кода быстро и легко."
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
    title_left: "Действия по подписанию Tar с помощью Qrcode в C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) позволяет быстро и легко подписывать документы Tar с подписями Qrcode.
        
        * Создайте экземпляр класса Signature, предоставляющий файл Tar, который должен быть подписан как путь или поток памяти.
        * Создайте экземпляр класса SignOptions и установите все требуемые данные.
        * Вызвать метод Signature.Sign(), передав выходной файл Tar или поток памяти

    title_right: " Системные Требования"
    content_right: |
        GroupDocs.Signature for .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Получите последнюю версию GroupDocs.Signature for .NET из [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Tar file
        string filePath = "input.tar";
        // Set up output file
        string outputFilePath = "output.tar";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined QrCode text
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // setup QrCode encoding type
                    EncodeType = QrCodeTypes.Aztec,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign Tar document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание Tar документов с помощью Qrcode Live Demo"
    content: |
       Подпишите файл Tar с различными подписями прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Бесплатная онлайн-демонстрация ждет вас.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Aztec QrCode"
          content: |
            Aztec Code — это двумерная (2-D) матричная система символов общего назначения, разработанная для обеспечения более высокой точности, чем другие 2-D системы символов. Символ кода ацтеков может кодировать до 3832 цифровых цифр; 3067 буквенных символов; или 1914 байт данных.
          characterset: |
             Все 256 символов ASCII.
          textcapacity: |
             До 3832 цифровых цифр, или 3067 буквенных символов, или 1914 байтов данных.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие поддерживаемые подписи Qrcode для C#"
    content: |
        "Вы также можете подписать Tar другими типами подписи. См. список ниже."
    format: 
        
       
back_to_top:
    enable: true
---