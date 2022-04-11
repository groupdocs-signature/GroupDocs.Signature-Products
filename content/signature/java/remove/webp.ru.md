---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:40:09+03:00
draft: false
############################# Head ############################
head_title: "Удалить цифровые подписи из WEBP в Java"
head_description: "Библиотека Java для очистки &amp; удалить цифровые подписи из файла WEBP с помощью API GroupDocs.Signature - управлять изображением, штрих-кодом, QR-кодом, штампом, текстом, оптическим и amp; Подписи метаданных из документов с цифровой подписью."
############################# Header ############################
title: "Удалить цифровую подпись из WEBP через Java"
description: "Библиотека Java eSignature для удаления цифровых подписей из файла WEBP. Легко манипулируйте изображениями, штрих-кодами, QR-кодами, штампами, текстовыми, оптическими и метаданными подписями из документов с цифровой подписью."
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
        [GroupDocs.Signature for Java](/ru/signature/java/) — это расширенная библиотека Java eSignature для цифровой подписи документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Добавив всего несколько строк кода, расширьте возможности своих Java-приложений для просмотра, добавления, редактирования, проверки, удаления и поиска цифровых подписей в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, метафайлах и форматах файлов изображений. API электронной подписи также поддерживает дополнительные функции для настройки свойств подписи в соответствии с требованиями.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как удалить цифровые подписи из WEBP"
    content_left: |
        В приведенном ниже примере кода Java четко показаны шаги по **удалению текстовых подписей из файла WEBP в Java** путем добавления всего нескольких строк кода.
        * Создайте новый экземпляр класса **Signature** и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте объект **TextSearchOptions** с нужными свойствами.
        * Вызовите метод **search**, чтобы получить список **TextSignatures**.
        * Выберите объекты **TextSignature**, которые необходимо удалить из документа.
        * Вызвать метод **delete** объекта **Signature**, передать ему одну или несколько подписей.
        * Проанализируйте результаты **DeleteResult**, чтобы убедиться, что подписи были обновлены или нет.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Signature для Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, IntelliJ IDEA, Eclipse
        * Фреймворки: Java 7 (1.7) и выше
        * Загрузите последнюю версию GroupDocs.Signature для Java с [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
    code: |
        ```java
        // инициализируем экземпляр Signature
        Signature signature = new Signature("signed.pdf");
         
        TextSearchOptions options = new TextSearchOptions();
         
        List signatures = signature.search(TextSignature.class,options);
        List signaturesToDelete = new ArrayList();
        // собираем подписи для удаления
        for (TextSignature temp : signatures)
        {
            if (temp.getText().contains("JS"))
            {
                signaturesToDelete.add(temp);
            }
        }
        // удаляем подписи
        DeleteResult deleteResult = signature.delete("signed.webp", signaturesToDelete);
        if (deleteResult.getSucceeded().size() == signaturesToDelete.size())
        {
            System.out.print("All signatures were successfully deleted!");
        }
        else
        {
            System.out.print("Successfully deleted signatures : " + deleteResult.getSucceeded().size());
            System.out.print("Not deleted signatures : " + deleteResult.getFailed().size());
        }
        System.out.print("List of deleted signatures:");
        for(BaseSignature temp : deleteResult.getSucceeded())
        {
            System.out.print("Signature# Id:"+temp.getSignatureId()+", Location: "+temp.getLeft()+"x"+temp.getTop()+". Size: "+temp.getWidth()+"x"+temp.getHeight());
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Удалить живые демонстрации подписи WEBP"
    content: |
        Добавьте электронные подписи файлов WEBP прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые демонстрации](https://products.groupdocs.app/signature/family). Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-webp"
          title: "Что такое формат файла WEBP"
          content: |
            WebP, представленный Google, представляет собой современный формат файлов растровых веб-изображений, основанный на сжатии без потерь и с потерями. Он обеспечивает такое же качество изображения при значительном уменьшении размера изображения. Поскольку большинство веб-страниц используют изображения в качестве эффективного представления данных, использование изображений WebP на веб-страницах приводит к более быстрой загрузке веб-страниц. По данным Google, изображения WebP без потерь на 26% меньше по размеру по сравнению с PNG, а изображения WebP с потерями на 25-34% меньше, чем сопоставимые изображения JPEG. Изображения сравниваются на основе индекса структурного сходства (SSIM) между WebP и другими форматами файлов изображений. WebP — это родственный проект формата мультимедийных контейнеров WebM. Узнайте больше о формате файла WEBP
          link: "https://docs.fileformat.com/image/webp/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие доступные варианты"
    content: |
        Многоформатный API удаления цифровых подписей для документов и изображений. Удалите подписи из некоторых популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Удалить подписи из PDF"
          link: "/signature/java/remove/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Удалить подписи из DOC"
          link: "/signature/java/remove/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Удалить подписи из DOCM"
          link: "/signature/java/remove/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Удалить подписи из DOCX"
          link: "/signature/java/remove/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Удалить подписи из DOT"
          link: "/signature/java/remove/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Удалить подписи из DOTX"
          link: "/signature/java/remove/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Удалить подписи из DOTM"
          link: "/signature/java/remove/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Удалить подписи из RTF"
          link: "/signature/java/remove/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Удалить подписи из ODT"
          link: "/signature/java/remove/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Удалить подписи из OTT"
          link: "/signature/java/remove/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Удалить подписи из XLS"
          link: "/signature/java/remove/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Удалить подписи из XLSX"
          link: "/signature/java/remove/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Удалить подписи из XLSM"
          link: "/signature/java/remove/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Удалить подписи из XLSM"
          link: "/signature/java/remove/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Удалить подписи из XLSB"
          link: "/signature/java/remove/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Удалить подписи из XLTX"
          link: "/signature/java/remove/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Удалить подписи из XLTM"
          link: "/signature/java/remove/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Удалить подписи из ODS"
          link: "/signature/java/remove/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Удалить подписи из OTS"
          link: "/signature/java/remove/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Удалить подписи из PPT"
          link: "/signature/java/remove/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Удалить подписи из PPTX"
          link: "/signature/java/remove/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Удалить подписи из PPS"
          link: "/signature/java/remove/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Удалить подписи из PPSX"
          link: "/signature/java/remove/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Удалить подписи из POTM"
          link: "/signature/java/remove/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Удалить подписи из POTX"
          link: "/signature/java/remove/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Удалить подписи из PPTM"
          link: "/signature/java/remove/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Удалить подписи из ODP"
          link: "/signature/java/remove/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Удалить подписи из OTP"
          link: "/signature/java/remove/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Удалить подписи из WEBP"
          link: "/signature/java/remove/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Удалить подписи из TIFF"
          link: "/signature/java/remove/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Удалить подписи из JPEG"
          link: "/signature/java/remove/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Удалить подписи из GIF"
          link: "/signature/java/remove/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Удалить подписи из PNG"
          link: "/signature/java/remove/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Удалить подписи из BMP"
          link: "/signature/java/remove/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Удалить подписи из CDR"
          link: "/signature/java/remove/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Удалить подписи из SVG"
          link: "/signature/java/remove/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Удалить подписи из PSD"
          link: "/signature/java/remove/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Удалить подписи из WMF"
          link: "/signature/java/remove/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Удалить подписи из EMF"
          link: "/signature/java/remove/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Удалить подписи из CMX"
          link: "/signature/java/remove/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Удалить подписи из DJVU"
          link: "/signature/java/remove/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Удалить подписи из PPSM"
          link: "/signature/java/remove/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Удалить подписи из DCM"
          link: "/signature/java/remove/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
