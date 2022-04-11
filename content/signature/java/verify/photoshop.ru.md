---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:20+03:00
draft: false
############################# Head ############################
head_title: "Как проверить цифровые подписи в PHOTOSHOP на Java"
head_description: "Узнайте, как проверять цифровые подписи в файле PHOTOSHOP на Java с помощью API GroupDocs.Siganture — добавляйте настраиваемые электронные подписи в популярные форматы деловых документов и файлов изображений."
############################# Header ############################
title: "Проверка цифровых подписей в PHOTOSHOP через Java"
description: "Библиотека Java для проверки всех популярных типов цифровых подписей в файле PHOTOSHOP. Легко управляйте свойствами Photoshop и настраивайте параметры подписи в документах и изображениях."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Скачать бесплатную пробную версию"
    link: "https://downloads.groupdocs.com/signature/java"
############################# SubMenu ############################
submenu:
    enable: true
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"
    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/signature/java"
              text: "Справочник по API"
            # button loop
            - link: "https://github.com/groupdocs-signature"
              text: "Примеры кода"
            # button loop
            - link: "https://products.groupdocs.app/signature/family"
              text: "Живые демонстрации"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Цены"
    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java"
        link_buy: "https://purchase.groupdocs.com"
############################# About ############################
about:
    enable: true
    title: "О GroupDocs.Signature для Java API"
    content: |
        [GroupDocs.Signature for Java](/ru/signature/java/) — это расширенная библиотека Java для цифровой подписи документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Добавив всего несколько строк кода, расширьте возможности своих Java-приложений для просмотра, добавления, редактирования, проверки, удаления и поиска цифровых подписей в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, метафайлах и форматах файлов изображений. API электронной подписи также поддерживает дополнительные функции для настройки свойств подписи в соответствии с требованиями.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как проверить цифровые подписи в файле PHOTOSHOP"
    content_left: |
        В приведенном ниже примере кода четко показаны действия по **проверке цифровых подписей в уже подписанном файле PHOTOSHOP на Java** с использованием библиотеки [GroupDocs.Signature](/ru/signature/java/) путем добавления всего нескольких строк кода.
        * Создайте новый экземпляр класса [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature) и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте объект [DigitalVerifyOptions](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.options.verify/DigitalVerifyOptions) в соответствии с вашими требованиями и укажите параметры проверки.
        * Вызовите [verify](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature#verify(com.groupdocs.signature.options.verify.VerifyOptions)) метод [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature) и передать [DigitalVerifyOptions](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.options.Verify/DigitalVerifyOptions).
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Signature для Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, IntelliJ IDEA, Eclipse
        * Фреймворки: Java 7 (1.7) и выше
        * Загрузите последнюю версию GroupDocs.Signature для Java с [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
    code: |
        ```java
        Signature signature = new Signature("sample.pdf");
        DigitalVerifyOptions options = new DigitalVerifyOptions(Constants.CertificatePfx);
        options.setComments("Test comment");
        options.setPassword("1234567890");
        
        // проверяем подписи документов
        VerificationResult result = signature.verify(options);
        if (result.isValid())
        {
            System.out.print("Документ успешно проверен!");
        }
        else
        {
            System.out.print("Документ не прошел проверку.");
        }
############################# Demos ############################
demos:
    enable: true
    title: "Подтвердите живые демонстрации PHOTOSHOP Signature"
    content: |
        Добавьте электронные подписи файлов PHOTOSHOP прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые демонстрации](https://products.groupdocs.app/signature/family). Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-photoshop"
          title: "Что такое формат файла PHOTOSHOP"
          content: |
            PSD, документ Photoshop, представляет собой собственный формат файлов Adobe Photoshop, используемый для графического дизайна и разработки. Файлы PSD могут включать в себя слои изображений, корректирующие слои, маски слоев, аннотации, информацию о файле, ключевые слова и другие элементы, характерные для Photoshop. Файлы Photoshop по умолчанию имеют расширение .PSD, максимальную высоту и ширину 30 000 пикселей и ограничение по длине в два гигабайта. Узнайте больше о формате файлов PHOTOSHOP
          link: "https://docs.fileformat.com/image/psd/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие доступные варианты"
    content: |
        Многоформатный API проверки цифровых подписей для документов и изображений. Обновите подписи некоторых популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Проверка электронных подписей в PDF"
          link: "/signature/java/verify/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Проверка электронных подписей в DOC"
          link: "/signature/java/verify/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Проверка электронных подписей в DOCM"
          link: "/signature/java/verify/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в DOCX"
          link: "/signature/java/verify/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Проверка электронных подписей в DOT"
          link: "/signature/java/verify/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Проверка электронных подписей в DOTX"
          link: "/signature/java/verify/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Проверка электронных подписей в DOTM"
          link: "/signature/java/verify/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в RTF"
          link: "/signature/java/verify/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Проверка электронных подписей в ODT"
          link: "/signature/java/verify/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Проверка электронных подписей в OTT"
          link: "/signature/java/verify/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Проверка электронных подписей в XLS"
          link: "/signature/java/verify/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Проверка электронных подписей в XLSX"
          link: "/signature/java/verify/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Проверка электронных подписей в XLSM"
          link: "/signature/java/verify/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в XLSM"
          link: "/signature/java/verify/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в XLSB"
          link: "/signature/java/verify/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Проверка электронных подписей в XLTX"
          link: "/signature/java/verify/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Проверка электронных подписей в XLTM"
          link: "/signature/java/verify/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в ODS"
          link: "/signature/java/verify/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Проверка электронных подписей в OTS"
          link: "/signature/java/verify/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Проверка электронных подписей в PPT"
          link: "/signature/java/verify/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Проверка электронных подписей в PPTX"
          link: "/signature/java/verify/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Проверка электронных подписей в PPS"
          link: "/signature/java/verify/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Проверка электронных подписей в PPSX"
          link: "/signature/java/verify/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Проверка электронных подписей в POTM"
          link: "/signature/java/verify/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в POTX"
          link: "/signature/java/verify/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Проверка электронных подписей в PPTM"
          link: "/signature/java/verify/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Проверка электронных подписей в ODP"
          link: "/signature/java/verify/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Проверка электронных подписей в OTP"
          link: "/signature/java/verify/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Проверка электронных подписей в WEBP"
          link: "/signature/java/verify/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Проверка электронных подписей в TIFF"
          link: "/signature/java/verify/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Проверка электронных подписей в JPEG"
          link: "/signature/java/verify/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Проверка электронных подписей в GIF"
          link: "/signature/java/verify/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Проверка электронных подписей в PNG"
          link: "/signature/java/verify/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Проверка электронных подписей в BMP"
          link: "/signature/java/verify/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Проверка электронных подписей в CDR"
          link: "/signature/java/verify/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Проверка электронных подписей в SVG"
          link: "/signature/java/verify/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Проверка электронных подписей в PSD"
          link: "/signature/java/verify/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Проверка электронных подписей в WMF"
          link: "/signature/java/verify/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Проверка электронных подписей в EMF"
          link: "/signature/java/verify/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Проверка электронных подписей в CMX"
          link: "/signature/java/verify/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Проверка электронных подписей в DJVU"
          link: "/signature/java/verify/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Проверка электронных подписей в PPSM"
          link: "/signature/java/verify/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Проверка электронных подписей в DCM"
          link: "/signature/java/verify/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
