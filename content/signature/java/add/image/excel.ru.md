---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:24+03:00
draft: false
############################# Head ############################
head_title: "Подпишите файлы Excel с помощью подписи изображений в Java"
head_description: "Добавляйте графические подписи для цифровой подписи документов Excel на Java — добавляйте настраиваемые электронные подписи к популярным деловым документам и форматам файлов изображений."
############################# Header ############################
title: "Добавить подписи изображений в файлы Excel в Java"
description: "Добавляйте цифровые подписи в файлы Excel, используя популярные типы подписей изображений. Безопасно добавляйте настраиваемые подписи изображений, манипулируя свойствами подписи — настраивайте параметры предварительной подписи в документах в соответствии с вашими потребностями."
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
        [GroupDocs.Signature for Java](/ru/signature/java/) — это собственный Java API для электронной подписи цифровых документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Пользователи могут добавлять, обновлять, проверять, удалять и искать цифровые подписи в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, OpenDocument, метафайлах и форматах файлов изображений с дополнительной поддержкой настройки свойств подписи по мере необходимости.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как добавить подписи к изображениям в Excel"
    content_left: |
        [GroupDocs.Signature](/ru/signature/java/) позволяет разработчикам Java легко добавлять подписи изображений к файлам Excel в своих приложениях, выполняя несколько простых шагов.
        * Создайте новый экземпляр класса Signature и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте экземпляр объекта ImageSignOptions в соответствии с вашими требованиями и укажите параметры подписи изображения.
        * Вызовите метод Sign экземпляра класса Signature и передайте ему ImageSignOptions.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Signature для Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, IntelliJ IDEA, Eclipse
        * Фреймворки: Java 7 (1.7) и выше
        * Загрузите последнюю версию GroupDocs.Signature для Java с [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
    code: |
        ```java
        Signature signature = new Signature("sample.xlsx"))
        ImageSignOptions options = new ImageSignOptions("signature.jpg") ;
        // устанавливаем позицию подписи
        options.setLeft(100);
        options.setTop(100);
        // устанавливаем номера страниц
        options.setPageNumber(1);
        // подписать документ в файл
        signature.sign("SampleSigned.xlsx", options);
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации — онлайн-приложение для добавления цифровых подписей"
    content: |
        Добавьте электронные подписи к файлам Excel прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые события](https://products.groupdocs.app/signature/family).
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-excel-o"
          title: "О формате файла Excel"
          content: |
            Файл электронной таблицы содержит данные в виде строк и столбцов. Файл электронной таблицы можно сохранить в нескольких различных форматах файлов, каждый из которых имеет свое расширение файла для уникального представления. Данные хранятся в ячейках либо в простой форме, такой как текстовая строка, числа, дата, валюта и т. д., либо в виде формул, которые изменяют значение ячейки при изменении ссылочных значений ячейки. Общие расширения файлов электронных таблиц и их форматы файлов включают XLSX (электронная таблица Microsoft Excel Open XML), ODS (электронная таблица OpenDocument) и XLS (формат двоичных файлов Microsoft Excel).
          link: "https://docs.fileformat.com/spreadsheet/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Подписание других форматов цифровых документов"
    content: |
        API управления цифровыми подписями Java для документов и изображений. Добавьте подписи изображений к некоторым из популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Добавить подписи к изображениям в PDF"
          link: "/signature/java/add/image/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Добавить подписи к изображениям в DOC"
          link: "/signature/java/add/image/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Добавить подписи к изображениям в DOCM"
          link: "/signature/java/add/image/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить подписи к изображениям в DOCX"
          link: "/signature/java/add/image/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Добавить подписи к изображениям в DOT"
          link: "/signature/java/add/image/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Добавить подписи к изображениям в DOTX"
          link: "/signature/java/add/image/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Добавить подписи к изображениям в DOTM"
          link: "/signature/java/add/image/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить подписи к изображениям в RTF"
          link: "/signature/java/add/image/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Добавить подписи к изображениям в ODT"
          link: "/signature/java/add/image/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Добавить подписи к изображениям в OTT"
          link: "/signature/java/add/image/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Добавить подписи к изображениям в XLS"
          link: "/signature/java/add/image/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Добавить подписи к изображениям в XLSX"
          link: "/signature/java/add/image/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Добавить подписи к изображениям в XLSM"
          link: "/signature/java/add/image/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить подписи к изображениям в XLSM"
          link: "/signature/java/add/image/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить подписи к изображениям в XLSB"
          link: "/signature/java/add/image/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Добавить подписи к изображениям в XLTX"
          link: "/signature/java/add/image/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Добавить подписи к изображениям в XLTM"
          link: "/signature/java/add/image/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить подписи к изображениям в ODS"
          link: "/signature/java/add/image/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Добавить подписи к изображениям в OTS"
          link: "/signature/java/add/image/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Добавить подписи к изображениям в PPT"
          link: "/signature/java/add/image/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Добавить подписи к изображениям в PPTX"
          link: "/signature/java/add/image/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Добавить подписи к изображениям в PPS"
          link: "/signature/java/add/image/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Добавить подписи к изображениям в PPSX"
          link: "/signature/java/add/image/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Добавить подписи к изображениям в POTM"
          link: "/signature/java/add/image/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Добавить подписи к изображениям в POTX"
          link: "/signature/java/add/image/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Добавить подписи к изображениям в PPTM"
          link: "/signature/java/add/image/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Добавить подписи к изображениям в ODP"
          link: "/signature/java/add/image/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Добавить подписи к изображениям в OTP"
          link: "/signature/java/add/image/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Добавить подписи к изображениям в WEBP"
          link: "/signature/java/add/image/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Добавить подписи к изображениям в TIFF"
          link: "/signature/java/add/image/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Добавить подписи к изображениям в JPEG"
          link: "/signature/java/add/image/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Добавить подписи к изображениям в GIF"
          link: "/signature/java/add/image/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Добавить подписи к изображениям в PNG"
          link: "/signature/java/add/image/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Добавить подписи к изображениям в BMP"
          link: "/signature/java/add/image/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Добавить подписи к изображениям в CDR"
          link: "/signature/java/add/image/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Добавить подписи к изображениям в SVG"
          link: "/signature/java/add/image/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Добавить подписи к изображениям в PSD"
          link: "/signature/java/add/image/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Добавить подписи к изображениям в WMF"
          link: "/signature/java/add/image/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Добавить подписи к изображениям в EMF"
          link: "/signature/java/add/image/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Добавить подписи к изображениям в CMX"
          link: "/signature/java/add/image/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Добавить подписи к изображениям в DJVU"
          link: "/signature/java/add/image/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Добавить подписи к изображениям в PPSM"
          link: "/signature/java/add/image/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Добавить подписи к изображениям в DCM"
          link: "/signature/java/add/image/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
