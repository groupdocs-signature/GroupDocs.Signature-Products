---
############################# Static ############################
layout: "auto-gen"
date: 2021-11-11T13:40:24+03:00
draft: false
############################# Head ############################
head_title: "Добавить круглую печать и подписать файл OTT | Подписывать документы"
head_description: "Подписывайте OTT-файлы с помощью круглых штампов — добавляйте штампы к популярным деловым документам и файлам изображений."
############################# Header ############################
title: "Добавить подписи с круглым штампом в файл OTT"
description: "Подпишите файлы OTT, используя круглую печать в C#. Управляйте свойствами подписи и настраивайте расширенные параметры подписи в документах в соответствии с вашими потребностями."
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
    title_left: "Как подписать OTT-файл с помощью Round Stamp"
    content_left: |
        [GroupDocs.Signature](/ru/signature/net/) позволяет разработчикам .NET легко добавлять круглые штампы в файлы OTT в своих приложениях, выполняя несколько простых шагов.
        * Создайте новый экземпляр класса Signature и передайте путь к исходному OTT-документу в качестве параметра конструктора.
        * Создайте экземпляр объекта StampSignOptions с требуемым текстом и установите для свойства EncodeType значение Round.
        * Вызовите метод Sign класса Signature и передайте ему имя выходного OTT-файла с StampSignOptions.
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
        using (Signature signature = new Signature("sample.ott"))
        {
            // Настраиваем внешний вид круглого штампа - размер, положение на странице документа, размер шрифта, цвет и т.д.
            StampSignOptions signOptions = новые StampSignOptions
            {
                StampType = StampTypes.Round,
                Height = 300,
                Width = 300,
                VerticalAlignment = VerticalAlignment.Center,
                HorizontalAlignment = HorizontalAlignment.Left,
                Background = new Background() { Color = Color.DarkOrange, Transparency = 0.5 },
                ImageFilePath = "handwrite_signature.jpg",
            };
            // Добавляем внешнюю строку подписи
            signOptions.OuterLines.Add(
                new StampLine
                {
                    Text = "* Мистер Джон Смит *",
                    TextRepeatType = StampTextRepeatType.FullTextRepeat,
                    Font = new SignatureFont() { Size = 12, FamilyName = "Arial" },
                    Height = 30,
                    TextBottomIntent = 6,
                    TextColor = Color.WhiteSmoke,
                    BackgroundColor = Color.DarkSlateBlue
                }
            );
            // Подписываем OTT файл и сохраняем результат 
            signature.Sign("signed.ott", options);
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации — онлайн-приложение для создания подписей с круглыми штампами"
    content: |
        Добавьте штампы Round в файлы OTT прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые события](https://products.groupdocs.app/signature/family).
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-stamp"
          title: "О круглой печати"
          content: |
            Круглый тип штампа является наиболее распространенным штампом, и это тип штампа, с которым легче всего столкнуться. Круглая форма часто используется агентствами, школами и компаниями. У него более формальная привлекательность, поэтому он больше подходит для официальных агентств.
          link: ""
############################# More Formats ############################
more_formats:
    enable: true
    title: "Подписание других форматов файлов с круглым штампом с использованием C#"
    content: |
        API управления подписями штампов .NET для документов и изображений. Добавьте штампы подписи к некоторым из популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Добавить электронные подписи в PDF"
          link: "/signature/net/add/stamp/pdf/round/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Добавить электронные подписи в DOC"
          link: "/signature/net/add/stamp/doc/round/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOCM"
          link: "/signature/net/add/stamp/docm/round/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в DOCX"
          link: "/signature/net/add/stamp/docx/round/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Добавить электронные подписи в DOT"
          link: "/signature/net/add/stamp/dot/round/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOTX"
          link: "/signature/net/add/stamp/dotx/round/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Добавить электронные подписи в DOTM"
          link: "/signature/net/add/stamp/dotm/round/"
          description: "Шаблон Microsoft Word с поддержкой макросов"       
        # format loop
        - name: "Добавить электронные подписи в ODT"
          link: "/signature/net/add/stamp/odt/round/"
          description: "Открыть текст документа"
        # format loop
        - name: "Добавить электронные подписи в OTT"
          link: "/signature/net/add/stamp/ott/round/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в XLS"
          link: "/signature/net/add/stamp/xls/round/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLSX"
          link: "/signature/net/add/stamp/xlsx/round/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Добавить электронные подписи в XLSM"
          link: "/signature/net/add/stamp/xlsm/round/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в XLSB"
          link: "/signature/net/add/stamp/xlsb/round/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTX"
          link: "/signature/net/add/stamp/xltx/round/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTM"
          link: "/signature/net/add/stamp/xltm/round/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в ODS"
          link: "/signature/net/add/stamp/ods/round/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Добавить электронные подписи в OTS"
          link: "/signature/net/add/stamp/ots/round/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в PPT"
          link: "/signature/net/add/stamp/ppt/round/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в PPTX"
          link: "/signature/net/add/stamp/pptx/round/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Добавить электронные подписи в PPS"
          link: "/signature/net/add/stamp/pps/round/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Добавить электронные подписи в PPSX"
          link: "/signature/net/add/stamp/ppsx/round/"
          description: "Слайд-шоу PowerPoint Open XML"                              
        # format loop
        - name: "Добавить электронные подписи в ODP"
          link: "/signature/net/add/stamp/odp/round/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в OTP"
          link: "/signature/net/add/stamp/otp/round/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в WEBP"
          link: "/signature/net/add/stamp/webp/round/"
          description: "Веб-изображение"
        # format loop
        - name: "Добавить электронные подписи в TIF"
          link: "/signature/net/add/stamp/tif/round/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Добавить электронные подписи в JPG"
          link: "/signature/net/add/stamp/jpg/round/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Добавить электронные подписи в GIF"
          link: "/signature/net/add/stamp/gif/round/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Добавить электронные подписи в PNG"
          link: "/signature/net/add/stamp/png/round/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Добавить электронные подписи в BMP"
          link: "/signature/net/add/stamp/bmp/round/"
          description: "Формат растрового файла"
        # format loop
        - name: "Добавить электронные подписи в CDR"
          link: "/signature/net/add/stamp/cdr/round/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Добавить электронные подписи в SVG"
          link: "/signature/net/add/stamp/svg/round/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Добавить электронные подписи в PSD"
          link: "/signature/net/add/stamp/psd/round/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Добавить электронные подписи в WMF"
          link: "/signature/net/add/stamp/wmf/round/"
          description: "Метафайл Windows"        
        # format loop
        - name: "Добавить электронные подписи в CMX"
          link: "/signature/net/add/stamp/cmx/round/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Добавить электронные подписи в DJVU"
          link: "/signature/net/add/stamp/djvu/round/"
          description: "Дежавю"
        # format loop
        - name: "Добавить электронные подписи в PPSM"
          link: "/signature/net/add/stamp/ppsm/round/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
############################# Back to top ###############################
back_to_top:
    enable: true
---
