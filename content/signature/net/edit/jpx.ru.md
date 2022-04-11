---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:33+03:00
draft: false
############################# Head ############################
head_title: "Редактировать &amp; Обновление файла JPX с цифровой подписью в .NET | Подписывать документы"
head_description: "Редактируйте файлы JPX с цифровыми подписями в .NET — обновляйте электронные подписи в популярных форматах деловых документов и файлов изображений."
############################# Header ############################
title: "Редактировать цифровые подписи в файле JPX"
description: "C# .NET API для мгновенного редактирования электронных подписей в файлах JPX с использованием популярных типов цифровых подписей. Управляйте свойствами подписи и настраивайте параметры подписи в документах и изображениях."
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
        [GroupDocs.Signature for .NET](/ru/signature/net/) — это собственный API .NET для цифровой подписи документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Пользователи могут легко добавлять, редактировать, проверять, удалять и находить цифровые подписи в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, метафайлах и форматах файлов изображений с дополнительной поддержкой настройки свойств подписи по мере необходимости.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как редактировать цифровые подписи в JPX"
    content_left: |
        [GroupDocs.Signature](/ru/signature/net/) позволяет разработчикам .NET легко редактировать цифровые подписи из файлов JPX в своих приложениях, выполняя несколько простых шагов.
        * Создайте новый экземпляр класса Signature и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте объект TextSearchOptions с нужными свойствами.
        * Вызвать метод Search для получения списка TextSignatures.
        * Выберите из списка объекты TextSignature, которые необходимо обновить.
        * Вызвать метод обновления объекта Signature и передать ему одну/несколько подписей.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Signature для .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Signature для .NET из [NuGet](https://www.nuget.org/packages/groupdocs.signature).
    code: |
        ```cs
        using (Signature signature = new Signature("sampleSigned.pdf"))
        {
            TextSearchOptions options = new TextSearchOptions();
            // поиск текстовых подписей в документе
            List signatures = signature.Search(options);
            if(signatures.Count > 0)
            {
                TextSignature textSignature = signatures[0];
                // изменить свойство Text
                textSignature.Text = "John Walkman";
                // изменить позицию
                textSignature.Left = textSignature.Left + 10;
                textSignature.Top = textSignature.Top + 10;
                // изменить размер. Обратите внимание, что не все документы поддерживают изменение размера подписи.
                textSignature.Width = 200;
                textSignature.Height = 100;
                bool result = signature.Update(textSignature);
                if(result)
                {
                    Console.WriteLine($"Signature with Text '{textSignature.Text}' was updated in the document ['{fileName}'].");
                }
                else
                {
                    Console.WriteLine($"Signature was not updated in  the document! Signature with Text '{textSignature.Text}' was not found!");
                }
            }
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации — онлайн-приложение для обновления цифровых подписей"
    content: |
        Редактируйте подписи в файлах JPX прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые события](https://products.groupdocs.app/signature/family).
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpx"
          title: "О формате файла JPX"
          content: |
            Файл с расширением .jpx является расширением формата файла JPEG 2000. Он в основном использует сжатие JPEG 2000, а также предоставляет расширенные функции, такие как несколько слоев для изображения, различные цветовые пространства, непрозрачность и потоки фрагментированного кода. JPX также поддерживает другие алгоритмы сжатия, такие как JBIG, CCITT Group3, CCITT Group4 и т. д., в дополнение к сжатию JPEG 2000. Формат файла JPX был утвержден в качестве стандарта ISO/IEC 15444-2, но не получил теплого приема из-за широкого использования формата файла JPEG. Приложения, которые могут открывать файлы JPX, включают Corel PaintShop Pro, Adobe Photoshop 2020, Adobe Illustrator 2020 и CorelDraw Graphics Suite 2020.
          link: "https://docs.fileformat.com/image/jpx/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Редактирование подписей из других форматов цифровых документов"
    content: |
        API для редактирования подписей мультиформатных документов и изображений для .NET. Обновите подписи некоторых популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Редактировать электронные подписи из PDF"
          link: "/signature/net/edit/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Редактировать электронные подписи из DOC"
          link: "/signature/net/edit/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Редактировать электронные подписи из DOCM"
          link: "/signature/net/edit/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из DOCX"
          link: "/signature/net/edit/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Редактировать электронные подписи из DOT"
          link: "/signature/net/edit/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Редактировать электронные подписи из DOTX"
          link: "/signature/net/edit/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Редактировать электронные подписи из DOTM"
          link: "/signature/net/edit/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из RTF"
          link: "/signature/net/edit/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Редактировать электронные подписи из ODT"
          link: "/signature/net/edit/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Редактировать электронные подписи из OTT"
          link: "/signature/net/edit/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Редактировать электронные подписи из XLS"
          link: "/signature/net/edit/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Редактировать электронные подписи из XLSX"
          link: "/signature/net/edit/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Редактировать электронные подписи из XLSM"
          link: "/signature/net/edit/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из XLSM"
          link: "/signature/net/edit/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из XLSB"
          link: "/signature/net/edit/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Редактировать электронные подписи из XLTX"
          link: "/signature/net/edit/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Редактировать электронные подписи из XLTM"
          link: "/signature/net/edit/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из ODS"
          link: "/signature/net/edit/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Редактировать электронные подписи из OTS"
          link: "/signature/net/edit/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Редактировать электронные подписи из PPT"
          link: "/signature/net/edit/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Редактировать электронные подписи из PPTX"
          link: "/signature/net/edit/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Редактировать электронные подписи из PPS"
          link: "/signature/net/edit/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Редактировать электронные подписи из PPSX"
          link: "/signature/net/edit/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Редактировать электронные подписи из POTM"
          link: "/signature/net/edit/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из POTX"
          link: "/signature/net/edit/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Редактировать электронные подписи из PPTM"
          link: "/signature/net/edit/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Редактировать электронные подписи из ODP"
          link: "/signature/net/edit/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Редактировать электронные подписи из OTP"
          link: "/signature/net/edit/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Редактировать электронные подписи из WEBP"
          link: "/signature/net/edit/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Редактировать электронные подписи из TIFF"
          link: "/signature/net/edit/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Редактировать электронные подписи из JPEG"
          link: "/signature/net/edit/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Редактировать электронные подписи из GIF"
          link: "/signature/net/edit/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Редактировать электронные подписи из PNG"
          link: "/signature/net/edit/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Редактировать электронные подписи из BMP"
          link: "/signature/net/edit/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Редактировать электронные подписи из CDR"
          link: "/signature/net/edit/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Редактировать электронные подписи из SVG"
          link: "/signature/net/edit/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Редактировать электронные подписи из PSD"
          link: "/signature/net/edit/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Редактировать электронные подписи из WMF"
          link: "/signature/net/edit/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Редактировать электронные подписи из EMF"
          link: "/signature/net/edit/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Редактировать электронные подписи из CMX"
          link: "/signature/net/edit/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Редактировать электронные подписи из DJVU"
          link: "/signature/net/edit/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Редактировать электронные подписи из PPSM"
          link: "/signature/net/edit/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из DCM"
          link: "/signature/net/edit/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
