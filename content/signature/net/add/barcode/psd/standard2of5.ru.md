---
############################# Static ############################
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false
############################# Head ############################
head_title: "Создать штрих-код Standard2of5 и подписать PSD-файл в .NET | Подписывать документы"
head_description: "Подписывайте PSD-файлы с помощью подписей штрих-кода Standard2of5 в .NET — добавляйте штрих-коды в популярные деловые документы и форматы файлов изображений."
############################# Header ############################
title: "Добавление подписей штрих-кода Standard2of5 в PSD-файл на C#"
description: "Подпишите файлы PSD, используя штрих-код Standard2of5. Управляйте свойствами подписи и настраивайте расширенные параметры подписи в документах в соответствии с вашими потребностями."
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
    title_left: "Как сгенерировать штрих-код Standard2of5 для файла PSD в C#"
    content_left: |
        [GroupDocs.Signature](/ru/signature/net/) позволяет разработчикам .NET легко добавлять штрих-коды Standard2of5 в файлы PSD в своих приложениях, выполняя несколько простых шагов.
        * Создайте новый экземпляр класса Signature и передайте путь к исходному PSD-документу в качестве параметра конструктора.
        * Создайте экземпляр объекта BarcodeSignOptions с требуемым текстом и установите для свойства EncodeType значение Standard2of5.
        * Вызовите метод Sign класса Signature и передайте ему выходное имя файла PSD с BarcodeSignOptions.
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
        using (Signature signature = new Signature("sample.psd"))
        {
            // Инициализировать параметры штрих-кода с предопределенным текстом штрих-кода
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                // настроить тип кодирования штрих-кода
                EncodeType = BarcodeTypes.Standard2of5,

                // установить позицию подписи
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // Подпишите файл PSD и сохраните результат
            signature.Sign("signed.psd", options);
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации — онлайн-приложение для создания подписей штрих-кода Standard2of5"
    content: |
        Добавьте штрих-коды Standard2of5 в файлы PSD прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые события](https://products.groupdocs.app/signature/family).
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "О штрих-коде Standard2of5"
          content: |
            Стандарт 2 из 5, также известный как IATA 2 из 5, является членом семейства символов Code 2 из 5, которое было впервые разработано в 1968 году. груз. Пробелы в стандартном символе 2 из 5 имеют фиксированную ширину, поэтому для кодирования информации используются только полосы. Название 2 из 5 происходит от того факта, что из пяти полос, которые используются для кодирования каждого символа, две широкие и три узкие.
          link: ""
############################# More Formats ############################
more_formats:
    enable: true
    title: "Подписание других форматов документов с помощью штрих-кода Standard2of5 с использованием C#"
    content: |
        API управления подписями штрих-кодов .NET для документов и изображений. Добавьте подписи штрих-кода к некоторым из популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Добавить электронные подписи в PDF"
          link: "/signature/net/add/barcode/pdf/standard2of5/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Добавить электронные подписи в DOC"
          link: "/signature/net/add/barcode/doc/standard2of5/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOCM"
          link: "/signature/net/add/barcode/docm/standard2of5/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в DOCX"
          link: "/signature/net/add/barcode/docx/standard2of5/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Добавить электронные подписи в DOT"
          link: "/signature/net/add/barcode/dot/standard2of5/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOTX"
          link: "/signature/net/add/barcode/dotx/standard2of5/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Добавить электронные подписи в DOTM"
          link: "/signature/net/add/barcode/dotm/standard2of5/"
          description: "Шаблон Microsoft Word с поддержкой макросов"       
        # format loop
        - name: "Добавить электронные подписи в ODT"
          link: "/signature/net/add/barcode/odt/standard2of5/"
          description: "Открыть текст документа"
        # format loop
        - name: "Добавить электронные подписи в OTT"
          link: "/signature/net/add/barcode/ott/standard2of5/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в XLS"
          link: "/signature/net/add/barcode/xls/standard2of5/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLSX"
          link: "/signature/net/add/barcode/xlsx/standard2of5/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Добавить электронные подписи в XLSM"
          link: "/signature/net/add/barcode/xlsm/standard2of5/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в XLSB"
          link: "/signature/net/add/barcode/xlsb/standard2of5/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTX"
          link: "/signature/net/add/barcode/xltx/standard2of5/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTM"
          link: "/signature/net/add/barcode/xltm/standard2of5/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в ODS"
          link: "/signature/net/add/barcode/ods/standard2of5/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Добавить электронные подписи в OTS"
          link: "/signature/net/add/barcode/ots/standard2of5/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в PPT"
          link: "/signature/net/add/barcode/ppt/standard2of5/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в PPTX"
          link: "/signature/net/add/barcode/pptx/standard2of5/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Добавить электронные подписи в PPS"
          link: "/signature/net/add/barcode/pps/standard2of5/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Добавить электронные подписи в PPSX"
          link: "/signature/net/add/barcode/ppsx/standard2of5/"
          description: "Слайд-шоу PowerPoint Open XML"                              
        # format loop
        - name: "Добавить электронные подписи в ODP"
          link: "/signature/net/add/barcode/odp/standard2of5/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в OTP"
          link: "/signature/net/add/barcode/otp/standard2of5/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в WEBP"
          link: "/signature/net/add/barcode/webp/standard2of5/"
          description: "Веб-изображение"
        # format loop
        - name: "Добавить электронные подписи в TIF"
          link: "/signature/net/add/barcode/tif/standard2of5/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Добавить электронные подписи в JPG"
          link: "/signature/net/add/barcode/jpg/standard2of5/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Добавить электронные подписи в GIF"
          link: "/signature/net/add/barcode/gif/standard2of5/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Добавить электронные подписи в PNG"
          link: "/signature/net/add/barcode/png/standard2of5/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Добавить электронные подписи в BMP"
          link: "/signature/net/add/barcode/bmp/standard2of5/"
          description: "Формат растрового файла"
        # format loop
        - name: "Добавить электронные подписи в CDR"
          link: "/signature/net/add/barcode/cdr/standard2of5/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Добавить электронные подписи в SVG"
          link: "/signature/net/add/barcode/svg/standard2of5/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Добавить электронные подписи в PSD"
          link: "/signature/net/add/barcode/psd/standard2of5/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Добавить электронные подписи в WMF"
          link: "/signature/net/add/barcode/wmf/standard2of5/"
          description: "Метафайл Windows"        
        # format loop
        - name: "Добавить электронные подписи в CMX"
          link: "/signature/net/add/barcode/cmx/standard2of5/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Добавить электронные подписи в DJVU"
          link: "/signature/net/add/barcode/djvu/standard2of5/"
          description: "Дежавю"
        # format loop
        - name: "Добавить электронные подписи в PPSM"
          link: "/signature/net/add/barcode/ppsm/standard2of5/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
############################# Back to top ###############################
back_to_top:
    enable: true
---
