---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:11+03:00
draft: false
############################# Head ############################
head_title: "Поиск цифровых подписей в DOTM через библиотеку Java"
head_description: "Библиотека Java для поиска &amp; проверять цифровые подписи в файле DOTM с помощью API GroupDocs.Siganture - управлять изображением, штрих-кодом, QR-кодом, штампом, текстом, оптическим и amp; Подписи метаданных из документов с цифровой подписью."
############################# Header ############################
title: "Поиск цифровой подписи в DOTM через Java"
description: "Java eSignature API для поиска &amp; проверять цифровые подписи в файле DOTM. Управление изображением, штрих-кодом, QR-кодом, штампом, текстом, оптическим изображением и усилителем; Подписи метаданных из документов с цифровой подписью."
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
        [GroupDocs.Signature for Java](/ru/signature/java/) — это расширенная библиотека Java eSignature для цифровой подписи документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Добавив всего несколько строк кода, расширьте возможности своих Java-приложений для просмотра, создания, редактирования, проверки, удаления и поиска цифровых подписей в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, метафайлах и форматах файлов изображений. API электронной подписи также поддерживает дополнительные функции для настройки свойств подписи в соответствии с требованиями.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как искать цифровые подписи в DOTM"
    content_left: |
        В приведенном ниже примере кода Java четко показаны шаги для **поиска цифровых подписей в файле DOTM на Java** путем добавления всего нескольких строк кода.
        * Создайте новый экземпляр класса **Signature** и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте экземпляр объекта **DigitalSearchOptions** в соответствии с вашими требованиями и укажите параметры поиска.
        * Вызвать метод **search** экземпляра класса **Signature** и передать ему **DigitalSearchOptions**.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Signature для Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, IntelliJ IDEA, Eclipse
        * Фреймворки: Java 7 (1.7) и выше
        * Загрузите последнюю версию GroupDocs.Signature для Java с [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
    code: |
        ```java
        Signature signature = new Signature("signed.pdf");
        DigitalSearchOptions options = new DigitalSearchOptions();
        // указываем специальные критерии поиска
        options.setComments("Test comment");
        // критерии выдачи сертификата
        options.setIssuerName("John");
        // предмет цифрового сертификата
        options.setSubjectName("Test");
        // указываем диапазон дат период подписи
        options.setSignDateTimeFrom(DateUtils.addMonths(new Date(), -1));
        options.setSignDateTimeTo(new Date());
        // поиск подписей в документе
        List signatures = signature.search(DigitalSignature.class, options);
        System.out.print("\nSource document contains following signatures.");
        for (DigitalSignature digitalSignature: подписи)
        {
            System.out.print("Digital signature found from "+digitalSignature.getSignTime()+" with validation flag "+digitalSignature.isValid()+". Certificate SN "+ digitalSignature.getCertificate().getType());
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Поиск DOTM Signature Live Demo"
    content: |
        Добавьте электронные подписи файлов DOTM прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые демонстрации](https://products.groupdocs.app/signature/family). Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dotm"
          title: "Что такое формат файла DOTM"
          content: |
            Файл с расширением DOTM представляет собой файл шаблона, созданный с помощью Microsoft Word 2007 или более поздней версии. Он похож на популярный формат файла DOCX, за исключением того, что он сохраняет определенные пользователем настройки для повторного использования в случае создания новых документов. Такие документы чаще используются в офисах, где создается стандартный файл шаблона с такими настройками, как информация о странице, поля, макет по умолчанию и макросы, и при необходимости используется для создания на его основе новых документов. Однако файлы DOTM сохраняют макросы, представляющие собой серию команд в виде записанных действий для автоматического завершения задачи. Это помогает сэкономить время при выполнении действий, которые повторяются при завершении задачи. Узнайте больше о формате файла DOTM
          link: "https://docs.fileformat.com/word-processing/dotm/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие доступные варианты"
    content: |
        Многоформатный API поиска цифровых подписей для документов и изображений. Найдите подписи в некоторых популярных форматах файлов, как указано ниже.
    format: 
        # format loop
        - name: "Поиск подписей в PDF"
          link: "/signature/java/search/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Поиск подписей в DOC"
          link: "/signature/java/search/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Поиск подписей в DOCM"
          link: "/signature/java/search/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Поиск подписей в DOCX"
          link: "/signature/java/search/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Поиск подписей в DOT"
          link: "/signature/java/search/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Поиск подписей в DOTX"
          link: "/signature/java/search/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Поиск подписей в DOTM"
          link: "/signature/java/search/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Поиск подписей в RTF"
          link: "/signature/java/search/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Поиск подписей в ODT"
          link: "/signature/java/search/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Поиск подписей в OTT"
          link: "/signature/java/search/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Поиск подписей в XLS"
          link: "/signature/java/search/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Поиск подписей в XLSX"
          link: "/signature/java/search/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Поиск подписей в XLSM"
          link: "/signature/java/search/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Поиск подписей в XLSM"
          link: "/signature/java/search/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Поиск подписей в XLSB"
          link: "/signature/java/search/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Поиск подписей в XLTX"
          link: "/signature/java/search/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Поиск подписей в XLTM"
          link: "/signature/java/search/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Поиск подписей в ODS"
          link: "/signature/java/search/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Поиск подписей в OTS"
          link: "/signature/java/search/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Поиск подписей в PPT"
          link: "/signature/java/search/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Поиск подписей в PPTX"
          link: "/signature/java/search/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Поиск подписей в PPS"
          link: "/signature/java/search/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Поиск подписей в PPSX"
          link: "/signature/java/search/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Поиск подписей в POTM"
          link: "/signature/java/search/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Поиск подписей в POTX"
          link: "/signature/java/search/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Поиск подписей в PPTM"
          link: "/signature/java/search/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Поиск подписей в ODP"
          link: "/signature/java/search/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Поиск подписей в OTP"
          link: "/signature/java/search/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Поиск подписей в WEBP"
          link: "/signature/java/search/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Поиск подписей в TIFF"
          link: "/signature/java/search/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Поиск подписей в JPEG"
          link: "/signature/java/search/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Поиск подписей в GIF"
          link: "/signature/java/search/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Поиск подписей в PNG"
          link: "/signature/java/search/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Поиск подписей в BMP"
          link: "/signature/java/search/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Поиск подписей в CDR"
          link: "/signature/java/search/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Поиск подписей в SVG"
          link: "/signature/java/search/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Поиск подписей в PSD"
          link: "/signature/java/search/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Поиск подписей в WMF"
          link: "/signature/java/search/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Поиск подписей в EMF"
          link: "/signature/java/search/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Поиск подписей в CMX"
          link: "/signature/java/search/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Поиск подписей в DJVU"
          link: "/signature/java/search/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Поиск подписей в PPSM"
          link: "/signature/java/search/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Поиск подписей в DCM"
          link: "/signature/java/search/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
