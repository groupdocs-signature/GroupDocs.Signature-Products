---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:55+03:00
draft: false
############################# Head ############################
head_title: "Проверка цифровых подписей в RTF-файле на C# .NET"
head_description: "C# .NET API для проверки &amp; проверять цифровые подписи в подписанном файле RTF, других форматах файлов изображений и документов, используя несколько строк кода."
############################# Header ############################
title: "Проверка цифровых подписей в файле RTF"
description: "C# .NET API для проверки цифровых подписей в уже подписанном файле RTF с использованием популярных типов электронных подписей. Управляйте свойствами электронной подписи в своих документах, добавляя несколько строк кода."
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
        [GroupDocs.Signature for .NET](/ru/signature/net/) — это расширенный .NET API для электронной подписи цифровых документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Пользователи могут загружать, редактировать, проверять, сохранять, удалять, просматривать и искать цифровые подписи в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, метафайлах и форматах файлов изображений с дополнительной поддержкой настройки свойств подписи по мере необходимости.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как проверить цифровые подписи в RTF"
    content_left: |
        [GroupDocs.Signature](/ru/signature/net/) позволяет разработчикам .NET легко проверять цифровые подписи в файлах RTF из своих приложений, выполняя несколько простых шагов.
        1. Создайте новый экземпляр класса Signature и передайте путь к исходному документу в качестве параметра конструктора.
        2. Создайте экземпляр объекта DigitalVerifyOptions в соответствии с вашими требованиями и укажите параметры проверки.
        3. Вызвать метод Verify класса Signature и передать ему DigitalVerifyOptions.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Signature для .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Signature для .NET из [NuGet](https://www.nuget.org/packages/groupdocs.signature).
    code: |
        ```cs
        using (Signature signature = new Signature("sample.pdf"))
        {
            DigitalVerifyOptions options = new DigitalVerifyOptions("certificate.pfx")
            {
                Comments = "Test comment"
            };
            // проверять подписи документов
            VerificationResult result = signature.Verify(options);
            if (result.IsValid)
            {
                Console.WriteLine("Документ успешно проверен!");
            }
            else
            {
                Console.WriteLine("Документ не прошел проверку.");
            }
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Проверка подписи RTF в режиме реального времени"
    content: |
        Добавьте электронные подписи файлов RTF прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые демонстрации](https://products.groupdocs.app/signature/family). Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-rtf"
          title: "Что такое формат файла RTF"
          content: |
            Представленный и задокументированный Microsoft формат Rich Text Format (RTF) представляет собой метод кодирования форматированного текста и графики для использования в приложениях. Формат облегчает межплатформенный обмен документами с другими продуктами Microsoft, что служит цели функциональной совместимости. Эта возможность делает его стандартом передачи данных между программным обеспечением для обработки текстов, и, следовательно, содержимое может быть передано из одной операционной системы в другую без потери форматирования документа. Спецификации формата файлов доступны Microsoft для общедоступной загрузки, и на них можно ссылаться с точки зрения разработчика. Узнайте больше о формате файла RTF
          link: "https://docs.fileformat.com/word-processing/rtf/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие доступные варианты"
    content: |
        Многоформатный API проверки цифровых подписей для документов и изображений. Проверьте подписи некоторых популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Проверка электронных подписей в PDF"
          link: "/signature/net/verify/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Проверка электронных подписей в DOC"
          link: "/signature/net/verify/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Проверка электронных подписей в DOCM"
          link: "/signature/net/verify/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в DOCX"
          link: "/signature/net/verify/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Проверка электронных подписей в DOT"
          link: "/signature/net/verify/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Проверка электронных подписей в DOTX"
          link: "/signature/net/verify/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Проверка электронных подписей в DOTM"
          link: "/signature/net/verify/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в RTF"
          link: "/signature/net/verify/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Проверка электронных подписей в ODT"
          link: "/signature/net/verify/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Проверка электронных подписей в OTT"
          link: "/signature/net/verify/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Проверка электронных подписей в XLS"
          link: "/signature/net/verify/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Проверка электронных подписей в XLSX"
          link: "/signature/net/verify/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Проверка электронных подписей в XLSM"
          link: "/signature/net/verify/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в XLSM"
          link: "/signature/net/verify/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в XLSB"
          link: "/signature/net/verify/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Проверка электронных подписей в XLTX"
          link: "/signature/net/verify/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Проверка электронных подписей в XLTM"
          link: "/signature/net/verify/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в ODS"
          link: "/signature/net/verify/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Проверка электронных подписей в OTS"
          link: "/signature/net/verify/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Проверка электронных подписей в PPT"
          link: "/signature/net/verify/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Проверка электронных подписей в PPTX"
          link: "/signature/net/verify/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Проверка электронных подписей в PPS"
          link: "/signature/net/verify/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Проверка электронных подписей в PPSX"
          link: "/signature/net/verify/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Проверка электронных подписей в POTM"
          link: "/signature/net/verify/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в POTX"
          link: "/signature/net/verify/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Проверка электронных подписей в PPTM"
          link: "/signature/net/verify/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Проверка электронных подписей в ODP"
          link: "/signature/net/verify/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Проверка электронных подписей в OTP"
          link: "/signature/net/verify/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Проверка электронных подписей в WEBP"
          link: "/signature/net/verify/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Проверка электронных подписей в TIFF"
          link: "/signature/net/verify/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Проверка электронных подписей в JPEG"
          link: "/signature/net/verify/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Проверка электронных подписей в GIF"
          link: "/signature/net/verify/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Проверка электронных подписей в PNG"
          link: "/signature/net/verify/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Проверка электронных подписей в BMP"
          link: "/signature/net/verify/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Проверка электронных подписей в CDR"
          link: "/signature/net/verify/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Проверка электронных подписей в SVG"
          link: "/signature/net/verify/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Проверка электронных подписей в PSD"
          link: "/signature/net/verify/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Проверка электронных подписей в WMF"
          link: "/signature/net/verify/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Проверка электронных подписей в EMF"
          link: "/signature/net/verify/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Проверка электронных подписей в CMX"
          link: "/signature/net/verify/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Проверка электронных подписей в DJVU"
          link: "/signature/net/verify/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Проверка электронных подписей в PPSM"
          link: "/signature/net/verify/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в DCM"
          link: "/signature/net/verify/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
