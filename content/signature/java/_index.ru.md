---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API цифровой подписи Java, добавление электронной подписи в изображение PDF Word Excel"
head_description: "API цифровой подписи Java. Библиотека электронных подписей для цифровой подписи PDF, Microsoft Word, электронных таблиц Excel, презентаций PowerPoint и форматов документов с изображениями."

############################# Header ############################
title: "Java API для управления цифровыми подписями"
description: "Управляйте электронной подписью изображений, QR-кодов, штрих-кодов, метаданных, типов текста и штампов в приложениях Java для подписи изображений и форматов файлов цифровых документов."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Обзор"

            # button loop
            - link: "#features"
              text: "Функции"

            # button loop
            - link: "#support"
              text: "Поддерживать"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Живая демонстрация"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Цены"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API помогает разрабатывать Java-приложения с функциями электронной подписи для подписи цифровых документов поддерживаемых форматов без установки какого-либо внешнего программного обеспечения. Он поддерживает манипулирование и управление различными типами электронных подписей, такими как изображения, штрих-коды, QR-коды, штампы, текстовые, оптические и метаданные. Все ваши электронные деловые документы, такие как Microsoft Office Word, презентации PowerPoint, электронные таблицы Excel, изображения и файлы PDF, могут быть подписаны цифровой подписью путем настройки свойств подписи, например. тень, размеры, выравнивание и многое другое в соответствии с вашими требованиями. Библиотека цифровых подписей проста и легка и состоит из одного DLL-файла, который можно легко интегрировать в новое или существующее приложение Java.  

      Через GroupDocs.Signature for Java API вы можете загрузить все зарегистрированные сертификаты из системы или найти существующие подписи, используя простой и расширенный поиск. Опции для работы с документами, защищенными паролем, указание общих свойств подписи (размер текста, непрозрачность, поворот, проверка, свойства шрифта, параметры цвета, номер страницы, ширина, верхнее, левое и т. д.) и поддержка реализации различных типов электронной подписи делают его надежным Решение для управления электронными подписями для цифровых документов.  

      GroupDocs.Signature for Java совместим со всеми версиями Java и поддерживает популярные операционные системы (Windows, Linux, MacOS), способные запускать среду выполнения Java.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Это обзор функций GroupDocs.Signature для Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Типы подписи"
          content: |
            * Текстовая подпись
            * Подпись изображения
            * Цифровые подписи
            * Подпись QR-кода
            * Подпись штрих-кода
            * Печать Подпись
            * Подпись поля формы
      
      ## TAB TWO ##
      tab_two:
        description: |
          API электронной подписи Java поддерживает различные форматы файлов документов, перечисленные ниже. [Поддерживаемые форматы документов.](https://docs.groupdocs.com/signature/java/supported-document-formats/)

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **Изображений**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Метафайлы**: EMF, WMF, CMX
                * **Портативный**: PDF
                * **Масштабируемая векторная графика**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Другие**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature для Java поддерживает следующие операционные системы, платформы и менеджеры пакетов:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операционные системы"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Поддерживаемые платформы"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Среды разработки"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Инструмент автоматизации сборки"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature для функций Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Создание, чтение, изменение, скрытие и удаление электронных подписей из поддерживаемых форматов документов"

      # feature loop
      - icon: "fas fa-eye"
        content: "Доступ к подписанному документу из потока, относительного или абсолютного пути"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Применение текстовой подписи к документам, электронным таблицам, презентациям, изображениям и файлам PDF"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Добавление текстовой подписи в качестве аннотации, наклейки, изображения в файлы PDF, а также настройка стиля и цвета"

      # feature loop
      - icon: "fas fa-code"
        content: "Подпишите PDF-документ, файл изображения и получите вывод в другом формате файла"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Цифровая подпись изображений с текстовой подписью в качестве водяного знака и добавление прозрачности, вращение к электронной подписи"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Ищите сертификаты и подписывайте документы Microsoft Word, Excel и PDF с помощью цифровых сертификатов"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Подписывайте форматы документов для обработки текстов с помощью встроенных текстовых водяных знаков"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Используйте QR-код, штрих-код для подписи файлов Word, слайдов, ячеек, PDF и изображений"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Настройка и применение штампов подписи для защиты поддерживаемых форматов файлов"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Настройка и назначение подписей изображений документам, электронным таблицам, презентациям, изображениям и файлам PDF"

      # feature loop
      - icon: "fas fa-columns"
        content: "Настройте свойства подписи, например внешний вид, поля, выравнивание и т. д."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Применение цифровой подписи к защищенному паролем документу"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Выполнение проверки текста PDF-документов с помощью обработчика подписи"

      # feature loop
      - icon: "fas fa-print"
        content: "Цифровая проверка документов Word, Cell, PDF с контейнерами сертификатов .CER и .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Укажите различные типы единиц измерения (например, миллиметры, пиксели и т. д.) для текстовых подписей PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Получение информации о документе через файл или URL-адрес — добавление подписей полей формы в документы PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Добавьте пользовательский объект данных, встроенную VCard, электронную почту, EPC, MeCard или объект события в QR-код"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Применение различных стилей кисти к подписям, например, градиентной, радиальной, сплошной и текстурной кисти."

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Подпишите документ, расположенный на FTP или в облачном хранилище Azure."

      # feature loop
      - icon: "fas fa-heading"
        content: "Установите выравнивание текста внутри фигур для документов, слайдов, изображений и файлов PDF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Поиск, проверка и цифровая подпись документов презентаций PowerPoint"

      # feature loop
      - icon: "fas fa-cube"
        content: "Размещение подписи с использованием пикселей в документах ячеек и позиционирование текста для подписей штампов"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Внедрение подписи прямоугольного штампа с закругленными углами"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Расширьте подписи штрих-кодов и QR-кодов с помощью содержимого данных изображения"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Добавление подписей зашифрованных метаданных при работе с параметрами подписи и поиска"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Внедрение пользовательских объектов в подписи метаданных в Word, Excel и презентациях"

    more_feature:
      # more_feature_loop
      - title: "Простая настройка и применение электронных подписей"
        content: |
          GroupDocs.Signature for Java API позволяет настраивать и добавлять электронные подписи в поддерживаемые форматы документов. Ниже приведен пример кода, показывающий, насколько просто применить текстовую подпись к файлу PDF:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // установить позицию подписи
          options.setLeft(100);
          options.setTop(100);
          
          // установить прямоугольник подписи
          options.setWidth(100);
          options.setHeight(30);

          // установить цвет текста и шрифт
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // подписать документ в файл
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Поддерживаемые типы кодирования штрих-кода для электронной подписи"
        content: |
          Используя GroupDocs.Signature for Java API, вы можете применять подписи штрих-кодов и QR-кодов к поддерживаемым форматам файлов. GroupDocs.Signature для Java поддерживает широкий спектр типов кодирования штрих-кода, чтобы удовлетворить большинство требований. Поддерживаемые типы кодирования штрих-кода включают Code 11, Code 128, Code 16K/32, коды Databar, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard и Расширенный код 39.

          Точно так же API GroupDocs.Signature для Java позволяет использовать типы QR-кода, такие как QR, Aztec и Data Matrix. Поддерживаемые типы кодирования QR-кода включают Aztec, DataMatrix, GS1 DataMatrix и GS1 QR.

      # more_feature_loop
      - title: "Поиск подписей и сертификатов"
        content: |
          С помощью GroupDocs.Signature for Java API вы можете искать подписи QR-кода и штрих-кода в любом документе, презентации, электронной таблице, изображении, а также в файле PDF и получать результат поиска. Вы также можете искать настраиваемые объекты данных в документах, подписанных с помощью подписи QR-кода, а также выполнять поиск стандартных VCard и объектов электронной почты в документах, подписанных с помощью QR-кода. Также поддерживается проверка зашифрованного текста подписей QR-кода, а также поиск подписи метаданных в документах PDF. Применяйте дополнительные критерии поиска цифровых подписей документов Words & Cells.  

          Параметр поиска также доступен для подписи метаданных для документов Word, слайдов и электронных таблиц, а поиск по полю формы доступен для документов PDF.

      # more_feature_loop
      - title: "Настройка свойств электронной подписи"
        content: |
          Чтобы улучшить UX конечных пользователей, GroupDocs.Signature для API Java предоставляет множество свойств, которые можно довольно легко настроить. Вы можете установить параметры шрифта и цвета (цвет фона, цвет переднего плана, полужирный, курсив, подчеркивание, семейство шрифтов, размер шрифта и т. д.), параметры фона и границы (цвет фона, прозрачность фона, цвет границы, стиль тире границы, толщина границы, Прозрачность границ и т. д.), поля подписи (слева, сверху, ширина, высота, отступы и т. д.) и область подписи изображения настройки и выравнивание подписи (горизонтальное выравнивание, вертикальное выравнивание и т. д.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature предлагает API для подписи документов для других популярных сред разработки."

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---