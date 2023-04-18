---
############################# Static ############################
layout: "product"
date: 2022-03-01T15:12:22
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ru
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET Digital Signature API — Электронный знак PDF Word Excel Изображения"
head_description: "API цифровой подписи C# .NET, библиотека eSignature для электронной подписи PDF, Word, электронных таблиц Excel, PowerPoint, изображений и графических форматов документов."

############################# Header ############################
title: "Собственный .NET API для электронных подписей"
description: "Добавляйте цифровые подписи в форматы документов и внедряйте популярные типы электронных подписей (текст, изображение, QR-код, штрих-код, штамп и метаданные) в приложениях .NET."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/signature/net"
              text: "Цены"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      Используйте API GroupDocs.Signature для .NET для создания приложений на C#, ASP.NET и других технологиях на основе .NET, которые позволяют подписывать цифровые деловые документы, такие как PDF, Microsoft Word, электронные таблицы Excel, презентации PowerPoint, изображения, OpenDocument и другие стандартные форматы файлов без необходимости установки какого-либо дополнительного программного обеспечения. С этой библиотекой электронных подписей легко работать, и разработчики .NET могут легко добавлять расширенные функции цифровой подписи в свои приложения, предоставляя пользователям возможность безопасно подписывать, искать и проверять электронные подписи из популярных форматов документов. Он поддерживает реализацию различных типов подписи, таких как текст, изображение, штрих-код, QR-код, поле формы, штамп и метаданные.  

      API подписи документа предоставляет вам простые и расширенные параметры поиска, позволяющие мгновенно находить нужные подписи в документе. Параметры для применения стиля подписи, управления внешним видом и настройки свойств подписи, таких как размеры, тень, выравнивание и т. д., также доступны с помощью этого многофункционального API для подписи документов.  

      GroupDocs.Signature для .NET можно использовать в любой среде разработки, поддерживающей платформу .NET. Он совместим со всеми языками на основе .NET и поддерживает популярные операционные системы (Windows, Linux, MacOS), в которых могут быть установлены платформы Mono или .NET (включая .NET Core).
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ниже приведен обзор GroupDocs.Signature для .NET:
      
        left:
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
            * Подпись метаданных
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Signature для .NET поддерживает просмотр всех популярных [форматов файлов документов](https://docs.groupdocs.com/signature/net/supported-document-formats/). Всего несколькими строками кода добавьте подпись PDF, Microsoft Office Word, электронные таблицы Excel, изображения, HTML, электронную почту Outlook, OneNote, Project и возможности просмотра графики в приложениях .NET.

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
          GroupDocs.Signature для .NET поддерживает следующие операционные системы, платформы и менеджеры пакетов:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операционные системы"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Поддерживаемые платформы"
              content: |
                * .NET Framework 2.0 or higher
                * Mono Framework 1.2 or higher
                * .NET Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Менеджер пакетов"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Среды разработки"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature для функций .NET"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Создание, поиск, обновление, скрытие, проверка и удаление электронных подписей из поддерживаемых форматов документов"

      # feature loop
      - icon: "fas fa-eye"
        content: "Укажите расширенные электронные подписи XML (XAdES) для электронных таблиц Excel"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Извлечение содержимого изображения из документов, подписанных QR-кодом, штрих-кодом и подписью изображения"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Установите высоту, ширину, поля и выравнивание для подписи текста или изображения и поместите на определенной странице"

      # feature loop
      - icon: "fas fa-code"
        content: "Поиск, проверка и цифровая подпись документов презентаций PowerPoint"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Подписывайте форматы документов для обработки текстов с помощью встроенных текстовых водяных знаков"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Поддерживает закругленные углы для прямоугольных типов подписи штампа"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Применить текстовую или графическую подпись к определенному листу Excel или установить электронную подпись для всех листов"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Укажите конкретный номер строки и столбца для размещения подписи текста или изображения на листе Excel"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Примените тень к текстовой подписи в Microsoft PowerPoint и настройте ее цвет, угол и прозрачность"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Настройка стилей границ и параметров шрифта текстовой подписи для листов Excel"

      # feature loop
      - icon: "fas fa-columns"
        content: "Установите тип подписи изображения, например. Круглый или квадратный и настроить поля, цвет шрифта, поворот"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Применение цифровых сертификатов к документам, электронным таблицам и PDF-файлам с помощью строки подписи"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Выполнение настроек цвета, применение прозрачности и поворота к текстовой подписи"

      # feature loop
      - icon: "fas fa-print"
        content: "Настройте параметры яркости и оттенков серого и укажите отступ подписи изображения в изображении"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Внедрение пользовательских объектов, сериализация, а также шифрование и расшифровка значений подписи метаданных PDF-документа"

      # feature loop
      - icon: "fas fa-lock"
        content: "Скрыть, удалить или настроить внешний вид цифровых подписей из документов PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Подписывайте PDF-документы с полем цифровой формы и текстовой подписью в виде изображения, аннотации, наклейки или водяного знака"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Поместите текстовую подпись в поля формы документов MS Word и PDF"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Указание произвольных страниц документов для обработки подписи или расширенной проверки электронной подписи для файлов Word"

      # feature loop
      - icon: "fas fa-heading"
        content: "Сохранить подписанный файл изображения в другом формате и экспортировать подписанную электронную таблицу в виде изображения или многостраничного TIFF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Назначение, изменение и удаление пароля для подписанных файлов и применение электронной подписи к файлам, защищенным паролем"

      # feature loop
      - icon: "fas fa-cube"
        content: "Рабочие листы eSign, слайды PowerPoint, документы Word и изображения с настраиваемыми объектами в метаданных"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Настройте фирменные стили кистей: Solid, Texture, Linear Gradient и Radial Gradient"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Подписывайте документы с помощью пользовательского зашифрованного текста или данных QR-кода"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Поиск и подпись файлов в формате DjVu в виде документа изображения"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Извлечение информации о документе, например, количество страниц, через URL-адрес файла"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Поиск, подпись и проверка файлов CorelDraw как графических документов"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Хранить историю обработанных или удаленных подписей в метаданных"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Добавьте пользовательский объект данных, VCard или объект электронной почты в QR-код и проверьте зашифрованный QR-код в файлах PDF"

    more_feature:
      # more_feature_loop
      - title: "Легко добавляйте цифровые подписи"
        content: |
          GroupDocs.Signature for .NET API позволяет добавлять различные типы подписей к поддерживаемым форматам файлов. Типы подписи, такие как текст, изображение, цифровая подпись, штамп, QR-код, штрих-код и метаданные, можно применять с помощью GroupDocs.Signature для .NET. В следующем примере кода показано, как применить текстовую подпись к документу PDF:

          ```cs
          using (Signature signature = new Signature("D:\\sample.pdf"))
          {
          TextSignOptions options = new TextSignOptions("John Smith")
          {
          // установить цвет текста
          ForeColor = Color.Red
          };
          // подписать документ в файл
          signature.Sign("D:\\signed.pdf", options);
          }
          ```

      # more_feature_loop
      - title: "Поддерживаемые типы подписи штрих-кода"
        content: |
          Наш API для обработки подписей предлагает вам возможность применять подписи штрих-кода к поддерживаемым форматам документов. GroupDocs.Signature для .NET поддерживает различные типы штрих-кодов, такие как Code128, Code39Extended, Code39Standard, EAN14, EAN8, ITF14, UPCA и UPCE. Также предоставляется статический объект с именем «AllTypes» для поддержки всех зарегистрированных типов штрих-кодов.

      # more_feature_loop
      - title: "Поиск подписей и сертификатов"
        content: |
          GroupDocs.Signature для .NET API позволяет выполнять поиск цифровых сертификатов в документах Word, электронных таблицах Excel и файлах PDF. Вы также можете получить все цифровые сертификаты, зарегистрированные в системе. Подписи метаданных также можно искать в документах Word, электронных таблицах Excel, изображениях и файлах PDF с помощью API GroupDocs.Signature для .NET.  

          С помощью GroupDocs.Signature для .NET API вы можете искать подписи QR-кода и штрих-кода в любом документе, презентации, электронной таблице, изображении, а также в файле PDF и получать информацию о ходе поиска. Вы также можете искать пользовательский объект данных в документах, подписанных с помощью подписи QR-Code.

      # more_feature_loop
      - title: "Параметры расширенного поиска для штрих-кода"
        content: |
          Вы можете очень легко искать и находить нужный штрих-код с помощью API GroupDocs.Signature для .NET, поскольку наш API подписи предлагает расширенные параметры поиска. Они позволяют выполнять поиск штрих-кода на определенной странице, выполнять поиск по всему документу, указывать разные страницы для поиска (первая, последняя, ​​четная, нечетная), искать штрих-код определенного типа кодировки, искать штрих-код на основе определенной текстовой строки или искать штрих-код. на основе строки с опцией «содержит».

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature предлагает API для просмотра документов для других популярных сред разработки."

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
          product: "GroupDocs.Signature"
          platform: "Java"
          link: "/signature/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---