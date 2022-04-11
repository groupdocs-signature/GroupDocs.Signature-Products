---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:44+03:00
draft: false
############################# Head ############################
head_title: "Найти &amp; Удаление цифровых подписей в файле XLTM в C# .NET"
head_description: "С# .NET API для поиска &amp; удалить цифровые подписи в подписанном файле XLTM, других форматах файлов изображений и документов, используя несколько строк кода."
############################# Header ############################
title: "Удаление цифровых подписей в файле XLTM"
description: "API цифровой подписи C# .NET для поиска &amp; удалить электронные подписи из файлов XLTM с цифровой подписью, добавив всего несколько строк кода. Подписывайте документы одним или несколькими типами подписи одновременно в любое время."
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
        [GroupDocs.Signature for .NET](/ru/signature/net/) — это расширенный API-интерфейс .NET для электронной подписи цифровых документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Пользователи могут легко просматривать, редактировать, проверять, сохранять, удалять, находить и предварительно просматривать цифровые подписи в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, метафайлах и форматах файлов изображений с дополнительной поддержкой настройки свойств подписи по мере необходимости.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как удалить подписи в файле XLTM"
    content_left: |
        [GroupDocs.Signature](/ru/signature/net/) позволяет разработчикам .NET легко находить и удалять цифровые подписи в файле XLTM из своих приложений, выполняя несколько простых шагов.
        * Создайте новый экземпляр класса Signature и передайте путь к исходному документу или его поток в качестве параметра конструктора.
        * Создайте объект DigitalSearchOptions с нужными свойствами.
        * Вызов метода поиска для получения списка цифровых подписей.
        * Выберите из списка объекты DigitalSignature, которые необходимо удалить из документа.
        * Вызвать метод Delete объекта Signature и передать ему одну или несколько подписей.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Signature для .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Signature для .NET из [NuGet](https://www.nuget.org/packages/groupdocs.signature).
    code: |
        ```cs
        using (Signature signature = new Signature("signed.xltm"))
        {
            // поиск ЭЦП в документе
            List signatures = signature.Search(SignatureType.Digital);
            if (signatures.Count > 0)
            {
                DigitalSignature digitalSignature = signatures[0];
                bool result = signature.Delete(digitalSignature);
                if(result)
                {
                    Console.WriteLine($"Digital signature #{digitalSignature.Thumbprint} from {digitalSignature.SignTime.ToShortDateString()} was deleted.");
                }
                else
                {
                    Helper.WriteError($"Signature was not deleted from the document! Signature# {digitalSignature.Thumbprint} was not found!");
                }
            }
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Удалить живые демонстрации XLTM Signature"
    content: |
        Добавьте электронные подписи файлов XLTM прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые демонстрации](https://products.groupdocs.app/signature/family). Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xltm"
          title: "Что такое формат файла XLTM"
          content: |
            Расширение файла XLTM представляет файлы, созданные Microsoft Excel, как файлы шаблонов с поддержкой макросов. Файлы XLTM аналогичны XLTX по структуре, за исключением того, что последний не поддерживает создание файлов шаблонов с макросами. Такие файлы шаблонов используются для создания и установки макета, форматирования и других параметров вместе с макросами, чтобы облегчить создание аналогичных файлов XLSX. Узнайте больше о формате файла XLTM
          link: "https://docs.fileformat.com/spreadsheet/xltm/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие доступные варианты"
    content: |
        Многоформатный API удаления цифровых подписей для документов и изображений. Удалите подписи из некоторых популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Удалить электронные подписи в PDF"
          link: "/signature/net/remove/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Удалить электронные подписи в DOC"
          link: "/signature/net/remove/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Удалить электронные подписи в DOCM"
          link: "/signature/net/remove/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Удалить электронные подписи в DOCX"
          link: "/signature/net/remove/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Удалить электронные подписи в DOT"
          link: "/signature/net/remove/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Удалить электронные подписи в DOTX"
          link: "/signature/net/remove/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Удалить электронные подписи в DOTM"
          link: "/signature/net/remove/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Удалить электронные подписи в RTF"
          link: "/signature/net/remove/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Удалить электронные подписи в ODT"
          link: "/signature/net/remove/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Удалить электронные подписи в OTT"
          link: "/signature/net/remove/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Удалить электронные подписи в XLS"
          link: "/signature/net/remove/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Удалить электронные подписи в XLSX"
          link: "/signature/net/remove/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Удалить электронные подписи в XLSM"
          link: "/signature/net/remove/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Удалить электронные подписи в XLSM"
          link: "/signature/net/remove/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Удалить электронные подписи в XLSB"
          link: "/signature/net/remove/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Удалить электронные подписи в XLTX"
          link: "/signature/net/remove/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Удалить электронные подписи в XLTM"
          link: "/signature/net/remove/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Удалить электронные подписи в ODS"
          link: "/signature/net/remove/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Удалить электронные подписи в OTS"
          link: "/signature/net/remove/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Удалить электронные подписи в PPT"
          link: "/signature/net/remove/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Удалить электронные подписи в PPTX"
          link: "/signature/net/remove/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Удалить электронные подписи в PPS"
          link: "/signature/net/remove/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Удалить электронные подписи в PPSX"
          link: "/signature/net/remove/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Удалить электронные подписи в POTM"
          link: "/signature/net/remove/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Удалить электронные подписи в POTX"
          link: "/signature/net/remove/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Удалить электронные подписи в PPTM"
          link: "/signature/net/remove/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Удалить электронные подписи в ODP"
          link: "/signature/net/remove/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Удалить электронные подписи в OTP"
          link: "/signature/net/remove/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Удалить электронные подписи в WEBP"
          link: "/signature/net/remove/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Удалить электронные подписи в TIFF"
          link: "/signature/net/remove/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Удалить электронные подписи в JPEG"
          link: "/signature/net/remove/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Удалить электронные подписи в GIF"
          link: "/signature/net/remove/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Удалить электронные подписи в PNG"
          link: "/signature/net/remove/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Удалить электронные подписи в BMP"
          link: "/signature/net/remove/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Удалить электронные подписи в CDR"
          link: "/signature/net/remove/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Удалить электронные подписи в SVG"
          link: "/signature/net/remove/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Удалить электронные подписи в PSD"
          link: "/signature/net/remove/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Удалить электронные подписи в WMF"
          link: "/signature/net/remove/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Удалить электронные подписи в EMF"
          link: "/signature/net/remove/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Удалить электронные подписи в CMX"
          link: "/signature/net/remove/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Удалить электронные подписи в DJVU"
          link: "/signature/net/remove/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Удалить электронные подписи в PPSM"
          link: "/signature/net/remove/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Удалить электронные подписи в DCM"
          link: "/signature/net/remove/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
