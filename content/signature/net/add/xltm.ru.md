---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:24+03:00
draft: false
############################# Head ############################
head_title: "Добавление цифровых подписей к файлам XLTM в .NET | Подписывать документы"
head_description: "Подписывайте файлы XLTM с помощью цифровых подписей в .NET — добавляйте настраиваемые электронные подписи к популярным форматам деловых документов и файлов изображений."
############################# Header ############################
title: "Добавьте цифровые подписи в файл XLTM"
description: "Подпишите свои файлы XLTM, используя популярные типы цифровой подписи. Управляйте свойствами подписи и настраивайте параметры предварительной подписи в документах в соответствии с вашими потребностями."
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
    title_left: "Как добавить цифровые подписи в XLTM"
    content_left: |
        [GroupDocs.Signature](/ru/signature/net/) позволяет разработчикам .NET легко добавлять электронные подписи к файлам XLTM в своих приложениях, выполняя несколько простых шагов.
        * Создайте новый экземпляр класса Signature и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте экземпляр объекта DigitalSignOptions с требуемым сертификатом и паролем.
        * Вызовите метод Sign класса Signature и передайте ему DigitalSignOptions.
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
            // инициализируем цифровую опцию с путем к файлу сертификата
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // сертифицируем пароль
                Password = "1234567890",
                // сведения о цифровом сертификате
                Reason = "Sign",
                Contact = "JohnSmith",
                Location = "Office1",
                // изображение в виде цифрового сертификата на страницах документа
                ImageFilePath = "sample.jpg",
                AllPages = true,
                Width = 80,
                Height = 60,
                VerticalAlignment = VerticalAlignment.Bottom,
                HorizontalAlignment = HorizontalAlignment.Right,
                Margin = new Padding() {  Bottom = 10, Right = 10},
            };
            signature.Sign("signed.xltm", options);
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации — онлайн-приложение для добавления цифровых подписей"
    content: |
        Добавьте подписи к файлам XLTM прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые события](https://products.groupdocs.app/signature/family).
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xltm"
          title: "О формате файла XLTM"
          content: |
            Расширение файла XLTM представляет файлы, созданные Microsoft Excel, как файлы шаблонов с поддержкой макросов. Файлы XLTM аналогичны XLTX по структуре, за исключением того, что последний не поддерживает создание файлов шаблонов с макросами. Такие файлы шаблонов используются для создания и установки макета, форматирования и других параметров вместе с макросами, чтобы облегчить создание аналогичных файлов XLSX.
          link: "https://docs.fileformat.com/spreadsheet/xltm"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Подписание других форматов цифровых документов"
    content: |
        API управления цифровыми подписями .NET для документов и изображений. Добавьте электронные подписи к некоторым из популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Добавить электронные подписи в PDF"
          link: "/signature/net/add/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Добавить электронные подписи в DOC"
          link: "/signature/net/add/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOCM"
          link: "/signature/net/add/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в DOCX"
          link: "/signature/net/add/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Добавить электронные подписи в DOT"
          link: "/signature/net/add/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOTX"
          link: "/signature/net/add/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Добавить электронные подписи в DOTM"
          link: "/signature/net/add/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в RTF"
          link: "/signature/net/add/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Добавить электронные подписи в ODT"
          link: "/signature/net/add/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Добавить электронные подписи в OTT"
          link: "/signature/net/add/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в XLS"
          link: "/signature/net/add/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLSX"
          link: "/signature/net/add/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Добавить электронные подписи в XLSM"
          link: "/signature/net/add/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в XLSM"
          link: "/signature/net/add/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в XLSB"
          link: "/signature/net/add/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTX"
          link: "/signature/net/add/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTM"
          link: "/signature/net/add/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в ODS"
          link: "/signature/net/add/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Добавить электронные подписи в OTS"
          link: "/signature/net/add/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в PPT"
          link: "/signature/net/add/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в PPTX"
          link: "/signature/net/add/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Добавить электронные подписи в PPS"
          link: "/signature/net/add/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Добавить электронные подписи в PPSX"
          link: "/signature/net/add/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Добавить электронные подписи в POTM"
          link: "/signature/net/add/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в POTX"
          link: "/signature/net/add/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в PPTM"
          link: "/signature/net/add/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в ODP"
          link: "/signature/net/add/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в OTP"
          link: "/signature/net/add/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в WEBP"
          link: "/signature/net/add/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Добавить электронные подписи в TIFF"
          link: "/signature/net/add/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Добавить электронные подписи в JPEG"
          link: "/signature/net/add/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Добавить электронные подписи в GIF"
          link: "/signature/net/add/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Добавить электронные подписи в PNG"
          link: "/signature/net/add/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Добавить электронные подписи в BMP"
          link: "/signature/net/add/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Добавить электронные подписи в CDR"
          link: "/signature/net/add/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Добавить электронные подписи в SVG"
          link: "/signature/net/add/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Добавить электронные подписи в PSD"
          link: "/signature/net/add/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Добавить электронные подписи в WMF"
          link: "/signature/net/add/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Добавить электронные подписи в EMF"
          link: "/signature/net/add/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Добавить электронные подписи в CMX"
          link: "/signature/net/add/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Добавить электронные подписи в DJVU"
          link: "/signature/net/add/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Добавить электронные подписи в PPSM"
          link: "/signature/net/add/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в DCM"
          link: "/signature/net/add/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
