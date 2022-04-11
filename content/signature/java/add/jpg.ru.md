---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T13:39:51+03:00
draft: false
############################# Head ############################
head_title: "Как добавить цифровые подписи к файлам JPG в Java"
head_description: "Узнайте, как добавлять цифровые подписи в файл JPG на языке Java с помощью API GroupDocs.Siganture — добавляйте настраиваемые электронные подписи в популярные форматы деловых документов и файлов изображений."
############################# Header ############################
title: "Добавить цифровые подписи в JPG в Java"
description: "Защитите свои файлы JPG, добавив популярные типы цифровых подписей с помощью библиотеки Java. Управляйте свойствами электронных подписей и настраивайте параметры предварительной подписи в документах по мере необходимости."
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
        [GroupDocs.Signature for Java](/ru/signature/java/) — это расширенная библиотека Java для цифровой подписи документов с использованием различных типов подписи, таких как текст, изображение, штрих-код, штамп, поле формы, QR-код и метаданные. Добавив всего несколько строк кода, добавьте в свои Java-приложения функции добавления, редактирования, проверки, удаления и поиска цифровых подписей в документах PDF, Microsoft Word, Excel, презентациях PowerPoint, Adobe Photoshop, метафайлах и форматах файлов изображений. API электронной подписи также поддерживает дополнительные функции для настройки свойств подписи в соответствии с требованиями.
############################# Steps ############################
steps:
    enable: true
    title_left: "Как добавить цифровые подписи в файл JPG"
    content_left: |
        В приведенном ниже примере кода четко показаны действия по **добавлению цифровых подписей в файл JPG с помощью библиотеки [GroupDocs.Signature](/ru/signature/java/) в Java** путем добавления всего нескольких строк кода.
        * Создайте новый экземпляр класса [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature) и передайте путь к исходному документу в качестве параметра конструктора.
        * Создайте объект [DigitalSignOptions](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.options.sign/DigitalSignOptions) с необходимым сертификатом и паролем.
        * Вызов [Sign](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature#sign(java.io.OutputStream,%20com.groupdocs.signature.options.sign.SignOptions)) метод экземпляра класса [Signature](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature/Signature); передайте ему DigitalSignOptions.
        * Проанализируйте результат [SignResult](https://apireference.groupdocs.com/java/signature/com.groupdocs.signature.domain/SignResult), чтобы при необходимости проверить вновь созданные подписи.
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
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");
        // сертифицируем пароль
        options.setPassword("1234567890");
        // сведения о цифровом сертификате
        options.setReason("Sign");
        options.setContact("JohnSmith");
        options.setLocation("Office1");
        // изображение в виде цифрового сертификата на страницах документа
        options.setImageFilePath("sample.jpg");
        //
        options.setAllPages(true);
        options.setWidth(80);
        options.setHeight(60);
        options.setVerticalAlignment(VerticalAlignment.Bottom);
        options.setHorizontalAlignment(HorizontalAlignment.Right);
        Padding padding = new Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        SignResult signResult = signature.sign("signed.jpg", options);
        // анализ результата
        System.out.print("List of newly created signatures:");
        int number = 1;
        for(BaseSignature temp: signResult.getSucceeded())
        {
            System.out.print("Подпись #"+ число++ +": Тип: "+temp.getSignatureType()+" Id:"+temp.getSignatureId()+
                    ",Location: "+temp.getLeft()+"x"+temp.getTop()+". Size: "+temp.getWidth()+"x"+temp.getHeight());
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Добавьте живые демонстрации подписи JPG"
    content: |
        Добавьте электронные подписи файлов JPG прямо сейчас, посетив веб-сайт [GroupDocs.Signature Живые демонстрации](https://products.groupdocs.app/signature/family). Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpg"
          title: "Что такое формат файла JPG"
          content: |
            JPEG — это тип формата изображения, который сохраняется с использованием метода сжатия с потерями. Выходное изображение в результате сжатия представляет собой компромисс между размером хранилища и качеством изображения. Пользователи могут настроить уровень сжатия для достижения желаемого уровня качества и в то же время уменьшить размер хранилища. Качество изображения незначительно ухудшается, если к изображению применяется сжатие 10:1. Чем выше значение сжатия, тем выше ухудшение качества изображения. Узнайте больше о формате файла JPG
          link: "https://docs.fileformat.com/image/jpeg/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие доступные варианты"
    content: |
        Многоформатный API цифровых подписей для документов и изображений. Добавьте подписи к некоторым популярным форматам файлов, как указано ниже.
    format: 
        # format loop
        - name: "Добавить электронные подписи в PDF"
          link: "/signature/java/add/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Добавить электронные подписи в DOC"
          link: "/signature/java/add/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOCM"
          link: "/signature/java/add/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в DOCX"
          link: "/signature/java/add/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Добавить электронные подписи в DOT"
          link: "/signature/java/add/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Добавить электронные подписи в DOTX"
          link: "/signature/java/add/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Добавить электронные подписи в DOTM"
          link: "/signature/java/add/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в RTF"
          link: "/signature/java/add/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Добавить электронные подписи в ODT"
          link: "/signature/java/add/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Добавить электронные подписи в OTT"
          link: "/signature/java/add/ott/"
          description: "Текстовый шаблон OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в XLS"
          link: "/signature/java/add/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLSX"
          link: "/signature/java/add/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Добавить электронные подписи в XLSM"
          link: "/signature/java/add/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в XLSM"
          link: "/signature/java/add/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в XLSB"
          link: "/signature/java/add/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTX"
          link: "/signature/java/add/xltx/"
          description: "Шаблон Microsoft Excel"
        # format loop
        - name: "Добавить электронные подписи в XLTM"
          link: "/signature/java/add/xltm/"
          description: "Шаблон Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в ODS"
          link: "/signature/java/add/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Добавить электронные подписи в OTS"
          link: "/signature/java/add/ots/"
          description: "Шаблон электронной таблицы OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в PPT"
          link: "/signature/java/add/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в PPTX"
          link: "/signature/java/add/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Добавить электронные подписи в PPS"
          link: "/signature/java/add/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Добавить электронные подписи в PPSX"
          link: "/signature/java/add/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Добавить электронные подписи в POTM"
          link: "/signature/java/add/potm/"
          description: "Шаблон Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в POTX"
          link: "/signature/java/add/potx/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в PPTM"
          link: "/signature/java/add/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Добавить электронные подписи в ODP"
          link: "/signature/java/add/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в OTP"
          link: "/signature/java/add/otp/"
          description: "Шаблон презентации OpenDocument"
        # format loop
        - name: "Добавить электронные подписи в WEBP"
          link: "/signature/java/add/webp/"
          description: "Веб-изображение"
        # format loop
        - name: "Добавить электронные подписи в TIFF"
          link: "/signature/java/add/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Добавить электронные подписи в JPEG"
          link: "/signature/java/add/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Добавить электронные подписи в GIF"
          link: "/signature/java/add/gif/"
          description: "Формат обмена графикой"
        # format loop
        - name: "Добавить электронные подписи в PNG"
          link: "/signature/java/add/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Добавить электронные подписи в BMP"
          link: "/signature/java/add/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Добавить электронные подписи в CDR"
          link: "/signature/java/add/cdr/"
          description: "CorelDraw векторный графический рисунок"
        # format loop
        - name: "Добавить электронные подписи в SVG"
          link: "/signature/java/add/svg/"
          description: "Масштабируемая векторная графика"
        # format loop
        - name: "Добавить электронные подписи в PSD"
          link: "/signature/java/add/psd/"
          description: "Документ Adobe Photoshop"
        # format loop
        - name: "Добавить электронные подписи в WMF"
          link: "/signature/java/add/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Добавить электронные подписи в EMF"
          link: "/signature/java/add/emf/"
          description: "Расширенный формат метафайла"
        # format loop
        - name: "Добавить электронные подписи в CMX"
          link: "/signature/java/add/cmx/"
          description: "Изображение обмена метафайлами Corel"
        # format loop
        - name: "Добавить электронные подписи в DJVU"
          link: "/signature/java/add/djvu/"
          description: "Дежавю"
        # format loop
        - name: "Добавить электронные подписи в PPSM"
          link: "/signature/java/add/ppsm/"
          description: "Слайд-шоу Microsoft PowerPoint с поддержкой макросов"
        # format loop
        - name: "Добавить электронные подписи в DCM"
          link: "/signature/java/add/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
############################# Back to top ###############################
back_to_top:
    enable: true
---
