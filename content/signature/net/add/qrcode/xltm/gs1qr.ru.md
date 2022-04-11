---
############################# Static ############################
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false
############################# Head ############################
head_title: "Сгенерируйте QR-код GS1QR и подпишите файл XLTM в .NET | Подписывать документы"
head_description: "Подписывайте файлы XLTM с помощью подписей QR-кода GS1QR в .NET — добавляйте штрих-коды в популярные форматы деловых документов и файлов изображений."
############################# Header ############################
title: "Добавьте QR-коды GS1QR в файл XLTM на C#"
description: "Подпишите файлы XLTM, используя QR-код GS1QR. Управляйте свойствами подписи и настраивайте расширенные параметры подписи в документах в соответствии с вашими потребностями."
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
    title_left: "Как сгенерировать QR-код Gs1qr для файла XLTM в C#"
    content_left: |
        [GroupDocs.Signature](/ru/signature/net/) позволяет разработчикам .NET легко добавлять штрих-коды Gs1qr в файлы XLTM в своих приложениях, выполняя несколько простых шагов.
        * Создайте новый экземпляр класса Signature и передайте исходный путь к документу XLTM в качестве параметра конструктора.
        * Создайте экземпляр объекта QrCodeSignOptions с требуемым текстом и установите для свойства EncodeType значение GS1QR.
        * Вызовите метод Sign класса Signature и передайте ему имя выходного XLTM-файла с QrCodeSignOptions.
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
        using (Signature signature = new Signature("sample.xltm"))
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
            // Подписываем XLTM файл и сохраняем результат 
            signature.Sign("signed.xltm", options);
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации - онлайн-приложение для создания подписей QR-кода Gs1qr"
    content: |
        Добавьте qr-коды Gs1qr в файлы XLTM прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые события](https://products.groupdocs.app/signature/family).
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-qrcode"
          title: "О QR-коде GS1QR"
          content: |
            QR-код GS1 — это вариант QR-кода, соответствующий спецификациям GS1. Он был разработан специально для обмена расширенной информацией об упаковке, такой как номер партии, идентификатор продукта и количество.
          link: ""
############################# More Formats ############################
more_formats:
    enable: true
    title: "Подписание других форматов файлов с помощью QR-кода Gs1qr с использованием C#"
    content: |
        .NET API управления подписями qr-кода для документов и изображений. Добавьте подписи qr-кода в некоторые популярные форматы файлов, как указано ниже.
    format: 
        # format loop
        - name: "Добавить электронные подписи в PDF"
          link: "/signature/net/add/qrcode/pdf/gs1qr/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Добавить электронные подписи в DOC"
          link: "/signature/net/add/qrcode/doc/gs1qr/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOCM"
          link: "/signature/net/add/qrcode/docm/gs1qr/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в DOCX"
          link: "/signature/net/add/qrcode/docx/gs1qr/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Добавить электронные подписи в DOT"
          link: "/signature/net/add/qrcode/dot/gs1qr/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOTX"
          link: "/signature/net/add/qrcode/dotx/gs1qr/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Добавить электронные подписи в DOTM"
          link: "/signature/net/add/qrcode/dotm/gs1qr/"
          description: "Шаблон Microsoft Word с поддержкой макросов"       
        # format loop
        - name: "Добавить электронные подписи в ODT"
          link: "/signature/net/add/qrcode/odt/gs1qr/"
          description: "Открыть текст документа"
        # format loop
        - name: "Добавить электронные подписи в OTT"
          link: "/signature/net/add/qrcode/ott/gs1qr/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в XLS"
          link: "/signature/net/add/qrcode/xls/gs1qr/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLSX"
          link: "/signature/net/add/qrcode/xlsx/gs1qr/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Добавить электронные подписи в XLSM"
          link: "/signature/net/add/qrcode/xlsm/gs1qr/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в XLSB"
          link: "/signature/net/add/qrcode/xlsb/gs1qr/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTX"
          link: "/signature/net/add/qrcode/xltx/gs1qr/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTM"
          link: "/signature/net/add/qrcode/xltm/gs1qr/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в ODS"
          link: "/signature/net/add/qrcode/ods/gs1qr/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Добавить электронные подписи в OTS"
          link: "/signature/net/add/qrcode/ots/gs1qr/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в PPT"
          link: "/signature/net/add/qrcode/ppt/gs1qr/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в PPTX"
          link: "/signature/net/add/qrcode/pptx/gs1qr/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Добавить электронные подписи в PPS"
          link: "/signature/net/add/qrcode/pps/gs1qr/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Добавить электронные подписи в PPSX"
          link: "/signature/net/add/qrcode/ppsx/gs1qr/"
          description: "Слайд-шоу PowerPoint Open XML"                              
        # format loop
        - name: "Добавить электронные подписи в ODP"
          link: "/signature/net/add/qrcode/odp/gs1qr/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в OTP"
          link: "/signature/net/add/qrcode/otp/gs1qr/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в WEBP"
          link: "/signature/net/add/qrcode/webp/gs1qr/"
          description: "Веб-изображение"
        # format loop
        - name: "Добавить электронные подписи в TIF"
          link: "/signature/net/add/qrcode/tif/gs1qr/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Добавить электронные подписи в JPG"
          link: "/signature/net/add/qrcode/jpg/gs1qr/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Добавить электронные подписи в GIF"
          link: "/signature/net/add/qrcode/gif/gs1qr/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Добавить электронные подписи в PNG"
          link: "/signature/net/add/qrcode/png/gs1qr/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Добавить электронные подписи в BMP"
          link: "/signature/net/add/qrcode/bmp/gs1qr/"
          description: "Формат растрового файла"
        # format loop
        - name: "Добавить электронные подписи в CDR"
          link: "/signature/net/add/qrcode/cdr/gs1qr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Добавить электронные подписи в SVG"
          link: "/signature/net/add/qrcode/svg/gs1qr/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Добавить электронные подписи в PSD"
          link: "/signature/net/add/qrcode/psd/gs1qr/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Добавить электронные подписи в WMF"
          link: "/signature/net/add/qrcode/wmf/gs1qr/"
          description: "Метафайл Windows"        
        # format loop
        - name: "Добавить электронные подписи в CMX"
          link: "/signature/net/add/qrcode/cmx/gs1qr/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Добавить электронные подписи в DJVU"
          link: "/signature/net/add/qrcode/djvu/gs1qr/"
          description: "Дежавю"
        # format loop
        - name: "Добавить электронные подписи в PPSM"
          link: "/signature/net/add/qrcode/ppsm/gs1qr/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
############################# Back to top ###############################
back_to_top:
    enable: true
---
