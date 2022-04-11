---
############################# Static ############################
layout: "auto-gen"
date: 2021-11-10T13:40:24+03:00
draft: false
############################# Head ############################
head_title: "Создать штрих-код Planet и подписать файл XLSX в .NET | Подписывать документы"
head_description: "Подписывайте файлы XLSX с помощью штрих-кодов Planet в .NET — добавляйте штрих-коды в популярные деловые документы и файлы изображений."
############################# Header ############################
title: "Добавить подписи штрих-кода планеты в файл XLSX на C#"
description: "Подпишите свои файлы XLSX, используя штрих-код Planet. Управляйте свойствами подписи и настраивайте расширенные параметры подписи в документах в соответствии с вашими потребностями."
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
    title_left: "Как сгенерировать штрих-код планеты для файла XLSX в C#"
    content_left: |
        [GroupDocs.Signature](/ru/signature/net/) позволяет разработчикам .NET легко добавлять штрих-коды Planet в файлы XLSX в своих приложениях, выполняя несколько простых шагов.
        * Создайте новый экземпляр класса Signature и передайте исходный путь к документу XLSX в качестве параметра конструктора.
        * Создайте экземпляр объекта BarcodeSignOptions с требуемым текстом и установите для свойства EncodeType значение Planet.
        * Вызовите метод Sign класса Signature и передайте ему выходное имя файла XLSX с BarcodeSignOptions.
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
        using (Signature signature = new Signature("sample.xlsx"))
        {
            // Инициализировать параметры штрих-кода с предопределенным текстом штрих-кода
            BarcodeSignOptions options = new BarcodeSignOptions("JohnSmith")
            {
                // настроить тип кодирования штрих-кода
                EncodeType = BarcodeTypes.Планета,

                // установить позицию подписи
                Left = 50,
                Top = 150,
                Width = 200,
                Height = 50
            };

            // Подпишите файл XLSX и сохраните результат
            signature.Sign("signed.xlsx", options);
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации — онлайн-приложение для создания подписей штрих-кодов планет"
    content: |
        Добавьте штрих-коды Planet в файлы XLSX прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые события](https://products.groupdocs.app/signature/family).
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "О планетарном штрих-коде"
          content: |
            Система символов почтового алфавитно-цифрового кодирования (PLANET) USPS была разработана Почтовой службой США (USPS) для автоматической идентификации, сортировки и отслеживания почтовых отправлений. Обычно он использовался в сочетании с символикой почтового числового кодирования USPS (USPS POSTNET).
          link: ""
############################# More Formats ############################
more_formats:
    enable: true
    title: "Подписание других форматов документов с помощью Planet Barcode с использованием C#"
    content: |
        API управления подписями штрих-кодов .NET для документов и изображений. Добавьте подписи штрих-кода к некоторым из популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Добавить электронные подписи в PDF"
          link: "/signature/net/add/barcode/pdf/planet/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Добавить электронные подписи в DOC"
          link: "/signature/net/add/barcode/doc/planet/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOCM"
          link: "/signature/net/add/barcode/docm/planet/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в DOCX"
          link: "/signature/net/add/barcode/docx/planet/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Добавить электронные подписи в DOT"
          link: "/signature/net/add/barcode/dot/planet/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOTX"
          link: "/signature/net/add/barcode/dotx/planet/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Добавить электронные подписи в DOTM"
          link: "/signature/net/add/barcode/dotm/planet/"
          description: "Шаблон Microsoft Word с поддержкой макросов"       
        # format loop
        - name: "Добавить электронные подписи в ODT"
          link: "/signature/net/add/barcode/odt/planet/"
          description: "Открыть текст документа"
        # format loop
        - name: "Добавить электронные подписи в OTT"
          link: "/signature/net/add/barcode/ott/planet/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в XLS"
          link: "/signature/net/add/barcode/xls/planet/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLSX"
          link: "/signature/net/add/barcode/xlsx/planet/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Добавить электронные подписи в XLSM"
          link: "/signature/net/add/barcode/xlsm/planet/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в XLSB"
          link: "/signature/net/add/barcode/xlsb/planet/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTX"
          link: "/signature/net/add/barcode/xltx/planet/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTM"
          link: "/signature/net/add/barcode/xltm/planet/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в ODS"
          link: "/signature/net/add/barcode/ods/planet/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Добавить электронные подписи в OTS"
          link: "/signature/net/add/barcode/ots/planet/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в PPT"
          link: "/signature/net/add/barcode/ppt/planet/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в PPTX"
          link: "/signature/net/add/barcode/pptx/planet/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Добавить электронные подписи в PPS"
          link: "/signature/net/add/barcode/pps/planet/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Добавить электронные подписи в PPSX"
          link: "/signature/net/add/barcode/ppsx/planet/"
          description: "Слайд-шоу PowerPoint Open XML"                              
        # format loop
        - name: "Добавить электронные подписи в ODP"
          link: "/signature/net/add/barcode/odp/planet/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в OTP"
          link: "/signature/net/add/barcode/otp/planet/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в WEBP"
          link: "/signature/net/add/barcode/webp/planet/"
          description: "Веб-изображение"
        # format loop
        - name: "Добавить электронные подписи в TIF"
          link: "/signature/net/add/barcode/tif/planet/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Добавить электронные подписи в JPG"
          link: "/signature/net/add/barcode/jpg/planet/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Добавить электронные подписи в GIF"
          link: "/signature/net/add/barcode/gif/planet/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Добавить электронные подписи в PNG"
          link: "/signature/net/add/barcode/png/planet/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Добавить электронные подписи в BMP"
          link: "/signature/net/add/barcode/bmp/planet/"
          description: "Формат растрового файла"
        # format loop
        - name: "Добавить электронные подписи в CDR"
          link: "/signature/net/add/barcode/cdr/planet/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Добавить электронные подписи в SVG"
          link: "/signature/net/add/barcode/svg/planet/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Добавить электронные подписи в PSD"
          link: "/signature/net/add/barcode/psd/planet/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Добавить электронные подписи в WMF"
          link: "/signature/net/add/barcode/wmf/planet/"
          description: "Метафайл Windows"        
        # format loop
        - name: "Добавить электронные подписи в CMX"
          link: "/signature/net/add/barcode/cmx/planet/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Добавить электронные подписи в DJVU"
          link: "/signature/net/add/barcode/djvu/planet/"
          description: "Дежавю"
        # format loop
        - name: "Добавить электронные подписи в PPSM"
          link: "/signature/net/add/barcode/ppsm/planet/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
############################# Back to top ###############################
back_to_top:
    enable: true
---
