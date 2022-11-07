---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: G S1 Data Matrix
fileformat: Dot
productName: .NET
lang: uk
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Dot for C#

############################# Head ############################
head_title: "eSign Dot документ із G S1 Data Matrix QR-кодом у C#"
head_description: "Створіть QR-код G S1 Data Matrix і помістіть його у файл Dot за допомогою .NET із коротким фрагментом коду C#. Використовуйте API підпису документів GroupDocs для електронного підпису своїх ділових документів і файлів за допомогою QR-коду."

############################# Header ############################
title: "Згенеруйте підпис QR-коду G S1 Data Matrix для документа Dot у C#"
description: "Електронно підписуйте свої Dot документи та контракти за допомогою G S1 Data Matrix QR-коду. Згенеруйте підпис QR-коду швидко та легко."
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
    title: "Про API підписів QR-коду GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) — це зрілий API для створення та генерування підписів QR-коду для документів. Користувачі можуть генерувати підписи QR-коду з текстом, щоб завантажити його або поділитися зображенням у соціальних мережах. Підписаний документ можна сканувати за допомогою API або просто на мобільну камеру! Підписуйте в електронному вигляді свої ділові контракти та офіційні документи, додаючи підпис QR-коду, і маніпулюйте ним. Будь-який підпис QR-коду міститиме унікальну спеціальну інформацію для ідентифікації підписувача або авторизації документа. Крім того, вміст QR-коду можна зашифрувати та розшифрувати за допомогою особистих ключів програмним шляхом. Це відкриває багато можливостей для обміну конфіденційними даними в публічних документах. Після підписання користувач може оновлювати, перевіряти, видаляти, переглядати або шукати QR-коди в PDF-файлах, документах MS Word, робочих книгах MS Excel, презентаціях MS PowerPoint, файлах Adobe Photoshop і різних форматах зображень. QR-коди можна додатково налаштувати.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Кроки для підпису Dot за допомогою Qrcode у C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) надає можливість швидко та легко підписувати документи Dot за допомогою підписів Qrcode.
        
        * Створіть екземпляр класу підпису, який надає файл Dot, який має бути підписаний як шлях або потік пам’яті
        * Створіть екземпляр класу SignOptions і встановіть усі потрібні дані.
        * Викликати метод Signature.Sign(), передаючи вихідний файл Dot або потік пам’яті

    title_right: " Системні вимоги"
    content_right: |
        GroupDocs.Signature for .NET підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Отримайте останню версію GroupDocs.Signature for .NET від [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dot file
        string filePath = "input.dot";
        // Set up output file
        string outputFilePath = "output.dot";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined QrCode text
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // setup QrCode encoding type
                    EncodeType = QrCodeTypes.G S1 Data Matrix,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign Dot document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Підпис документів Dot за допомогою Qrcode Live Demo"
    content: |
       Підпишіть файл Dot різними підписами просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Безкоштовна онлайн-демоверсія чекає на вас.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About G S1 Data Matrix QrCode"
          content: |
            GS1 Data Matrix є варіантом Data Matrix, який відповідає специфікаціям GS1. Використовуйте GS1 DataMatrix для кодування такої інформації, як, але не обмежуючись, такою: AI(01) глобальний номер торгової одиниці (GTIN), AI(17) термін придатності, AI(10) номер партії, AI(21) серійний номер .
          characterset: |
             Набір символів: великі та малі літери та спеціальні символи $@%*+-./:=<>;&*_,'! усі з правильними ідентифікаторами програми.
          textcapacity: |
             Місткість кодового тексту: до 3116 цифрових цифр або 2335 буквено-цифрових символів.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Інші підтримувані підписи Qrcode для C#"
    content: |
        "Ви також можете підписати Dot іншими типами підписів. Перегляньте список нижче."
    format: 
        
       
back_to_top:
    enable: true
---