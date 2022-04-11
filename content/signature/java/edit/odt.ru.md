---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:39:59+03:00
draft: false
############################# Head ############################
head_title: "Пример кода Java для просмотра &amp; Редактировать цифровые подписи из файлов ODT"
head_description: "Пример кода Java для просмотра и редактирования цифровых подписей из файла ODT с использованием API GroupDocs.Siganture — добавление настраиваемых электронных подписей в популярные форматы деловых документов и файлов изображений."
############################# Header ############################
title: "Редактировать цифровые подписи в ODT через Java"
description: "Библиотека Java для просмотра &amp; редактировать цифровые подписи в файле ODT, используя популярные типы электронных подписей. Управляйте свойствами ODT и настраивайте параметры подписи в документах и изображениях."
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
        [GroupDocs.Signature for Java](/ru/signature/java/) — это расширенная библиотека Java для цифровой подписи документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Добавив всего несколько строк кода, расширьте возможности своих Java-приложений для просмотра, добавления, обновления, проверки, удаления и поиска цифровых подписей в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, метафайлах и форматах файлов изображений. API электронной подписи также поддерживает дополнительные функции для настройки свойств подписи в соответствии с требованиями.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как редактировать цифровые подписи в ODT"
    content_left: |
        В приведенном ниже примере кода четко показаны действия по **редактированию цифровых подписей в уже подписанном ODT-файле на Java** с использованием библиотеки [GroupDocs.Signature](/ru/signature/java/) путем добавления всего нескольких строк кода.
        * Создайте новый экземпляр класса [Signature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature) и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте объект [ImageSearchOptions](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.options.search/ImageSearchOptions) с нужными свойствами.
        * Вызов [поиск](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature#search(java.lang.Class,%20com.groupdocs.signature.options.search.SearchOptions)) метод для получения списка [ImageSignatures](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.domain.signatures/ImageSignature).
        * Выберите из списка [ImageSignature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature.domain.signatures/ImageSignature) объекты, которые необходимо обновить.
        * Вызовите объект [Signature](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature).[update](https://apireference.groupdocs.com/signature/java/com.groupdocs.signature/Signature#update(java.io.OutputStream,%20com.groupdocs.signature.domain.signatures.BaseSignature)) и передать ему одну или несколько подписей.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Signature для Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, IntelliJ IDEA, Eclipse
        * Фреймворки: Java 7 (1.7) и выше
        * Загрузите последнюю версию GroupDocs.Signature для Java с [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
    code: |
        ```java
        Signature signature = new Signature("sampleSigned.pdf");
        try 
        {
            ImageSearchOptions options = new ImageSearchOptions();
        
            // search for image signatures in document
            List signatures = signature.search(ImageSignature.class,options);
            if (signatures.size() > 0)
            {
                ImageSignature imageSignature = signatures.get(0);
                imageSignature.setLeft(100);
                imageSignature.setTop(100);
                boolean result = signature.update("sampleSigned-output.odt",imageSignature);
                if (result)
                {
                    System.out.print("Image signature at location " + imageSignature.getLeft() + "x" + imageSignature.getTop() + " and Size " + imageSignature.getSize() + " was updated in the document [" + fileName + ".");
                }
                else
                {
                    System.out.print("Signature was not updated in the document! Signature at location " + imageSignature.getLeft() + "x" + imageSignature.getTop() + " and Size " + imageSignature.getSize() + " was not found!");
                }
            }
        } catch (Exception e) {
            throw new GroupDocsSignatureException(e.getMessage());
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Редактировать живые демонстрации ODT Signature"
    content: |
        Добавьте электронные подписи файлов ODT прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые демонстрации](https://products.groupdocs.app/signature/family). Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-odt"
          title: "Что такое формат файла ODT"
          content: |
            Файлы ODT представляют собой тип документов, созданных с помощью приложений для обработки текстов, основанных на формате текстового файла OpenDocument. Они создаются с помощью приложений текстового процессора, таких как бесплатный OpenOffice Writer, и могут содержать такое содержимое, как текст, изображения, объекты и стили. Файл ODT для текстового процессора Writer является тем же, чем файл DOCX для Microsoft Word. Несколько приложений, включая Google Docs и веб-текстовый процессор Google, входящий в состав Google Диска, могут открывать файлы ODT для редактирования. Microsoft Word также может открывать файлы ODT и сохранять их в других форматах, таких как DOC и DOCX. Узнайте больше о формате файла ODT
          link: "https://docs.fileformat.com/word-processing/odt/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие доступные варианты"
    content: |
        Многоформатный API редактирования цифровых подписей для документов и изображений. Обновите подписи некоторых популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Редактировать электронные подписи из PDF"
          link: "/signature/java/edit/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Редактировать электронные подписи из DOC"
          link: "/signature/java/edit/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Редактировать электронные подписи из DOCM"
          link: "/signature/java/edit/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из DOCX"
          link: "/signature/java/edit/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Редактировать электронные подписи из DOT"
          link: "/signature/java/edit/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Редактировать электронные подписи из DOTX"
          link: "/signature/java/edit/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Редактировать электронные подписи из DOTM"
          link: "/signature/java/edit/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из RTF"
          link: "/signature/java/edit/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Редактировать электронные подписи из ODT"
          link: "/signature/java/edit/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Редактировать электронные подписи из OTT"
          link: "/signature/java/edit/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Редактировать электронные подписи из XLS"
          link: "/signature/java/edit/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Редактировать электронные подписи из XLSX"
          link: "/signature/java/edit/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Редактировать электронные подписи из XLSM"
          link: "/signature/java/edit/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из XLSM"
          link: "/signature/java/edit/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из XLSB"
          link: "/signature/java/edit/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Редактировать электронные подписи из XLTX"
          link: "/signature/java/edit/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Редактировать электронные подписи из XLTM"
          link: "/signature/java/edit/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из ODS"
          link: "/signature/java/edit/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Редактировать электронные подписи из OTS"
          link: "/signature/java/edit/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Редактировать электронные подписи из PPT"
          link: "/signature/java/edit/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Редактировать электронные подписи из PPTX"
          link: "/signature/java/edit/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Редактировать электронные подписи из PPS"
          link: "/signature/java/edit/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Редактировать электронные подписи из PPSX"
          link: "/signature/java/edit/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Редактировать электронные подписи из POTM"
          link: "/signature/java/edit/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из POTX"
          link: "/signature/java/edit/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Редактировать электронные подписи из PPTM"
          link: "/signature/java/edit/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Редактировать электронные подписи из ODP"
          link: "/signature/java/edit/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Редактировать электронные подписи из OTP"
          link: "/signature/java/edit/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Редактировать электронные подписи из WEBP"
          link: "/signature/java/edit/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Редактировать электронные подписи из TIFF"
          link: "/signature/java/edit/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Редактировать электронные подписи из JPEG"
          link: "/signature/java/edit/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Редактировать электронные подписи из GIF"
          link: "/signature/java/edit/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Редактировать электронные подписи из PNG"
          link: "/signature/java/edit/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Редактировать электронные подписи из BMP"
          link: "/signature/java/edit/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Редактировать электронные подписи из CDR"
          link: "/signature/java/edit/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Редактировать электронные подписи из SVG"
          link: "/signature/java/edit/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Редактировать электронные подписи из PSD"
          link: "/signature/java/edit/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Редактировать электронные подписи из WMF"
          link: "/signature/java/edit/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Редактировать электронные подписи из EMF"
          link: "/signature/java/edit/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Редактировать электронные подписи из CMX"
          link: "/signature/java/edit/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Редактировать электронные подписи из DJVU"
          link: "/signature/java/edit/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Редактировать электронные подписи из PPSM"
          link: "/signature/java/edit/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Редактировать электронные подписи из DCM"
          link: "/signature/java/edit/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
