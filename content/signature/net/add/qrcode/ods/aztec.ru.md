---
############################# Static ############################
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false
############################# Head ############################
head_title: "Сгенерируйте QR-код Aztec и подпишите файл ODS в .NET | Подписывать документы"
head_description: "Подписывайте файлы ODS с помощью подписей QR-кода Aztec в .NET — добавляйте штрих-коды в популярные форматы деловых документов и файлов изображений."
############################# Header ############################
title: "Добавьте QR-коды Aztec в файл ODS на C#"
description: "Подпишите файлы ODS, используя QR-код Aztec. Управляйте свойствами подписи и настраивайте расширенные параметры подписи в документах в соответствии с вашими потребностями."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Скачать бесплатную пробную версию"
    link: "https://downloads.groupdocs.com/signature/net"
############################# SubMenu ############################
submenu:
    enable: true
    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"
    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/signature/net"
              text: "Справочник по API"
            # button loop
            - link: "https://github.com/groupdocs-signature"
              text: "Примеры кода"
            # button loop
            - link: "https://products.groupdocs.app/signature/family"
              text: "Живые демонстрации"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/net"
              text: "Цены"
    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net"
        link_buy: "https://purchase.groupdocs.com"
############################# About ############################
about:
    enable: true
    title: "О GroupDocs.Signature для .NET API"
    content: |
        [GroupDocs.Signature for .NET](/ru/signature/net/) — это собственный API-интерфейс .NET для электронной подписи цифровых документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Пользователи могут добавлять, редактировать, проверять, удалять и искать цифровые подписи в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, метафайлах и форматах файлов изображений с дополнительной поддержкой настройки свойств подписи по мере необходимости.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как сгенерировать QR-код Aztec для файла ODS в C#"
    content_left: |
        [GroupDocs.Signature](/ru/signature/net/) позволяет разработчикам .NET легко добавлять штрих-коды Aztec в файлы ODS в своих приложениях, выполняя несколько простых шагов.
        * Создайте новый экземпляр класса Signature и передайте путь к исходному документу ODS в качестве параметра конструктора.
        * Создайте объект QrCodeSignOptions с требуемым текстом и установите для свойства EncodeType значение Aztec.
        * Вызовите метод Sign класса Signature и передайте ему имя выходного файла ODS с QrCodeSignOptions.
        * Проанализируйте результат SignResult, чтобы проверить вновь созданные подписи, если это необходимо.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Signature для .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Signature для .NET из [NuGet](https://www.nuget.org/packages/groupdocs.signature).
    code: |
        ```cs
        using (Signature signature = new Signature("sample.ods"))
        {
            // Инициализировать параметры qr-кода предопределенным текстом
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
            {
                // устанавливаем тип кодировки QRCode
                EncodeType = QrCodeTypes.QR,
                // устанавливаем позицию подписи
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };
            // Подписываем ODS файл и сохраняем результат 
            signature.Sign("signed.ods", options);
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации — онлайн-приложение для создания подписей QR-кода Aztec"
    content: |
        Добавьте qr-коды Aztec в файлы ODS прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые события](https://products.groupdocs.app/signature/family).
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-qrcode"
          title: "О QR-коде Aztec"
          content: |
            Aztec Code — это двумерная (2-D) матричная система символов общего назначения, которая обеспечивает более высокую точность, чем другие двумерные системы символов. Символ кода ацтеков может кодировать до 3832 цифровых цифр; 3067 буквенных символов; или 1914 байт данных. Код ацтеков был изобретен Эндрю Лонгакром-младшим и Робертом Хасси в 1995 году. Код был опубликован AIM, Inc. в 1997 году. Хотя код ацтеков был запатентован, этот патент официально стал общественным достоянием. Кодекс ацтеков также опубликован как стандарт ISO/IEC 24778:2008. Код Aztec, названный в честь сходства шаблона центрального искателя с пирамидой ацтеков, потенциально может занимать меньше места, чем другие матричные штрих-коды, поскольку он не требует окружающей пустой тихой зоны.
          link: ""
############################# More Formats ############################
more_formats:
    enable: true
    title: "Подписание других форматов файлов с помощью QR-кода Aztec с использованием C#"
    content: |
        .NET API управления подписями qr-кода для документов и изображений. Добавьте подписи qr-кода в некоторые популярные форматы файлов, как указано ниже.
    format: 
        # format loop
        - name: "Добавить электронные подписи в PDF"
          link: "/signature/net/add/qrcode/pdf/aztec/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Добавить электронные подписи в DOC"
          link: "/signature/net/add/qrcode/doc/aztec/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOCM"
          link: "/signature/net/add/qrcode/docm/aztec/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в DOCX"
          link: "/signature/net/add/qrcode/docx/aztec/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Добавить электронные подписи в DOT"
          link: "/signature/net/add/qrcode/dot/aztec/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOTX"
          link: "/signature/net/add/qrcode/dotx/aztec/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Добавить электронные подписи в DOTM"
          link: "/signature/net/add/qrcode/dotm/aztec/"
          description: "Шаблон Microsoft Word с поддержкой макросов"       
        # format loop
        - name: "Добавить электронные подписи в ODT"
          link: "/signature/net/add/qrcode/odt/aztec/"
          description: "Открыть текст документа"
        # format loop
        - name: "Добавить электронные подписи в OTT"
          link: "/signature/net/add/qrcode/ott/aztec/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в XLS"
          link: "/signature/net/add/qrcode/xls/aztec/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLSX"
          link: "/signature/net/add/qrcode/xlsx/aztec/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Добавить электронные подписи в XLSM"
          link: "/signature/net/add/qrcode/xlsm/aztec/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в XLSB"
          link: "/signature/net/add/qrcode/xlsb/aztec/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTX"
          link: "/signature/net/add/qrcode/xltx/aztec/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTM"
          link: "/signature/net/add/qrcode/xltm/aztec/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в ODS"
          link: "/signature/net/add/qrcode/ods/aztec/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Добавить электронные подписи в OTS"
          link: "/signature/net/add/qrcode/ots/aztec/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в PPT"
          link: "/signature/net/add/qrcode/ppt/aztec/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в PPTX"
          link: "/signature/net/add/qrcode/pptx/aztec/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Добавить электронные подписи в PPS"
          link: "/signature/net/add/qrcode/pps/aztec/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Добавить электронные подписи в PPSX"
          link: "/signature/net/add/qrcode/ppsx/aztec/"
          description: "Слайд-шоу PowerPoint Open XML"                              
        # format loop
        - name: "Добавить электронные подписи в ODP"
          link: "/signature/net/add/qrcode/odp/aztec/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в OTP"
          link: "/signature/net/add/qrcode/otp/aztec/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в WEBP"
          link: "/signature/net/add/qrcode/webp/aztec/"
          description: "Веб-изображение"
        # format loop
        - name: "Добавить электронные подписи в TIF"
          link: "/signature/net/add/qrcode/tif/aztec/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Добавить электронные подписи в JPG"
          link: "/signature/net/add/qrcode/jpg/aztec/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Добавить электронные подписи в GIF"
          link: "/signature/net/add/qrcode/gif/aztec/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Добавить электронные подписи в PNG"
          link: "/signature/net/add/qrcode/png/aztec/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Добавить электронные подписи в BMP"
          link: "/signature/net/add/qrcode/bmp/aztec/"
          description: "Формат растрового файла"
        # format loop
        - name: "Добавить электронные подписи в CDR"
          link: "/signature/net/add/qrcode/cdr/aztec/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Добавить электронные подписи в SVG"
          link: "/signature/net/add/qrcode/svg/aztec/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Добавить электронные подписи в PSD"
          link: "/signature/net/add/qrcode/psd/aztec/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Добавить электронные подписи в WMF"
          link: "/signature/net/add/qrcode/wmf/aztec/"
          description: "Метафайл Windows"        
        # format loop
        - name: "Добавить электронные подписи в CMX"
          link: "/signature/net/add/qrcode/cmx/aztec/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Добавить электронные подписи в DJVU"
          link: "/signature/net/add/qrcode/djvu/aztec/"
          description: "Дежавю"
        # format loop
        - name: "Добавить электронные подписи в PPSM"
          link: "/signature/net/add/qrcode/ppsm/aztec/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
############################# Back to top ###############################
back_to_top:
    enable: true
---
