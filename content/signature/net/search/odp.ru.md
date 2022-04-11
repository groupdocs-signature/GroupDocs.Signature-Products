---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:47+03:00
draft: false
############################# Head ############################
head_title: "Поиск &amp; Проверка цифровых подписей в файле ODP в C# .NET"
head_description: "C# .NET API для поиска цифровых подписей в подписанном ODP-файле, других изображениях и форматах файлов документов с использованием нескольких строк кода."
############################# Header ############################
title: "Поиск цифровых подписей в файле ODP"
description: "Собственный API C# .NET для просмотра &amp; искать цифровые подписи в уже подписанном файле ODP и анализировать сертификат подписи. Выполняйте расширенные операции электронной подписи в ваших документах, используя несколько строк кода."
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
            - link: "https://docs.groupdocs.com/signature/net/release-notes"
              text: "Примечания к выпуску"
    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net"
        link_buy: "https://purchase.groupdocs.com"
############################# About ############################
about:
    enable: true
    title: "О GroupDocs.Signature для .NET API"
    content: |
        [GroupDocs.Signature for .NET](/ru/signature/net/) — это расширенный API-интерфейс .NET для электронной подписи цифровых документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Пользователи могут загружать, редактировать, проверять, сохранять, удалять, находить и просматривать цифровые подписи в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, метафайлах и форматах файлов изображений с дополнительной поддержкой настройки свойств подписи по мере необходимости.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как искать подписи в ODP"
    content_left: |
        [GroupDocs.Signature](/ru/signature/net/) позволяет разработчикам .NET легко просматривать и искать цифровые подписи в файлах ODP из своих приложений, выполняя несколько простых шагов.
        * Создайте новый экземпляр класса Signature и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте экземпляр объекта DigitalSearchOptions в соответствии с вашими требованиями и укажите параметры поиска.
        * Вызвать метод Search экземпляра класса Signature и передать ему DigitalSearchOptions.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Signature для .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Signature для .NET из [NuGet](https://www.nuget.org/packages/groupdocs.signature).
    code: |
        ```cs
        using (Signature signature = new Signature("signed.pdf"))
        {
            DigitalSearchOptions options = new DigitalSearchOptions()
            {
                // указать специальные критерии поиска
                Comments = "Test comment",
                // критерии выдачи сертификата
                IssuerName = "John",
                // предмет цифрового сертификата
                SubjectName = "Test",
                // указать диапазон дат период подписи
                SignDateTimeFrom = DateTime.Now.AddMonths(-1),
                SignDateTimeTo = DateTime.Now,
            };
            // поиск подписей в документе
            List signatures = signature.Search(options);
            Console.WriteLine("Source document contains following signatures.");
            foreach (var digitalSignature in signatures)
            {
                Console.WriteLine("Digital signature found from {0} with validation flag {1}. Certificate SN {2}",
                    digitalSignature.SignTime, digitalSignature.IsValid, digitalSignature.Certificate?.SerialNumber);
            }
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Поиск живых демо ODP Signature"
    content: |
        Добавьте электронные подписи файлов ODP прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые демонстрации](https://products.groupdocs.app/signature/family). Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-odp"
          title: "Что такое формат файла ODP"
          content: |
            Файлы с расширением ODP представляют формат файла презентации, используемый OpenOffice.org в стандарте OASISOpen. Файл презентации — это набор слайдов, каждый из которых может содержать текст, изображения, форматирование, анимацию и другие медиафайлы. Эти слайды представляются аудитории в виде слайд-шоу с пользовательскими настройками презентации. Файлы ODP можно открывать приложениями, которые соответствуют формату OpenDocument (например, OpenOffice или StarOffice). Узнайте больше о формате файла ODP
          link: "https://docs.fileformat.com/presentation/odp/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие доступные варианты"
    content: |
        Многоформатный API поиска цифровых подписей для документов и изображений. Найдите подписи в некоторых популярных форматах файлов, как указано ниже.
    format: 
        # format loop
        - name: "Поиск электронных подписей в PDF"
          link: "/signature/net/search/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Поиск электронных подписей в DOC"
          link: "/signature/net/search/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Поиск электронных подписей в DOCM"
          link: "/signature/net/search/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Поиск электронных подписей в DOCX"
          link: "/signature/net/search/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Поиск электронных подписей в DOT"
          link: "/signature/net/search/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Поиск электронных подписей в DOTX"
          link: "/signature/net/search/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Поиск электронных подписей в DOTM"
          link: "/signature/net/search/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Поиск электронных подписей в RTF"
          link: "/signature/net/search/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Поиск электронных подписей в ODT"
          link: "/signature/net/search/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Поиск электронных подписей в OTT"
          link: "/signature/net/search/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Поиск электронных подписей в XLS"
          link: "/signature/net/search/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Поиск электронных подписей в XLSX"
          link: "/signature/net/search/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Поиск электронных подписей в XLSM"
          link: "/signature/net/search/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Поиск электронных подписей в XLSM"
          link: "/signature/net/search/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Поиск электронных подписей в XLSB"
          link: "/signature/net/search/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Поиск электронных подписей в XLTX"
          link: "/signature/net/search/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Поиск электронных подписей в XLTM"
          link: "/signature/net/search/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Поиск электронных подписей в ODS"
          link: "/signature/net/search/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Поиск электронных подписей в OTS"
          link: "/signature/net/search/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Поиск электронных подписей в PPT"
          link: "/signature/net/search/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Поиск электронных подписей в PPTX"
          link: "/signature/net/search/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Поиск электронных подписей в PPS"
          link: "/signature/net/search/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Поиск электронных подписей в PPSX"
          link: "/signature/net/search/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Поиск электронных подписей в POTM"
          link: "/signature/net/search/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Поиск электронных подписей в POTX"
          link: "/signature/net/search/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Поиск электронных подписей в PPTM"
          link: "/signature/net/search/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Поиск электронных подписей в ODP"
          link: "/signature/net/search/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Поиск электронных подписей в OTP"
          link: "/signature/net/search/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Поиск электронных подписей в WEBP"
          link: "/signature/net/search/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Поиск электронных подписей в TIFF"
          link: "/signature/net/search/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Поиск электронных подписей в JPEG"
          link: "/signature/net/search/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Поиск электронных подписей в GIF"
          link: "/signature/net/search/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Поиск электронных подписей в PNG"
          link: "/signature/net/search/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Поиск электронных подписей в BMP"
          link: "/signature/net/search/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Поиск электронных подписей в CDR"
          link: "/signature/net/search/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Поиск электронных подписей в SVG"
          link: "/signature/net/search/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Поиск электронных подписей в PSD"
          link: "/signature/net/search/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Поиск электронных подписей в WMF"
          link: "/signature/net/search/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Поиск электронных подписей в EMF"
          link: "/signature/net/search/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Поиск электронных подписей в CMX"
          link: "/signature/net/search/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Поиск электронных подписей в DJVU"
          link: "/signature/net/search/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Поиск электронных подписей в PPSM"
          link: "/signature/net/search/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Поиск электронных подписей в DCM"
          link: "/signature/net/search/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
