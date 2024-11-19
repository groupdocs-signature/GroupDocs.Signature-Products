



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: ru
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Генерация QR-кода для файлов PDF с использованием C#"
head_description: "Используйте API GroupDocs.Signature для генерации QR-кода для файлов PDF. Легко встраивайте QR-коды на любые страницы для повышения функциональности."

############################# Header ############################
title: "Генерация QR-кодов для PDF" 
description: "Генерируйте 2D-штрих-коды, используя текстовые или числовые данные, и применяйте их на нескольких страницах и в различных форматах, включая PDF, Word, Excel и др., через GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Начните свою бесплатную пробную версию"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Изучите возможности GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Узнать больше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) предлагает широкий спектр функций, позволяющих пользователям генерировать и встраивать различные типы подписей в основные форматы документов. Будь то PDF, документы Word, таблицы Excel, презентации PowerPoint или файловые изображения, вы можете улучшить свои документы, добавив текстовые, изображенческие, штрих-кодовые, QR-коды, метаданные, цифровые и штампованные подписи.

############################# Steps ############################
steps:
    enable: true
    title: "Как сгенерировать и вставить QR-код в любом месте документа PDF"
    content: |
      [GroupDocs.Signature](/signature/net/) упрощает генерацию QR-кодов в различных популярных форматах и их размещение на страницах PDF. Поддерживая более 10 типов QR-кодов, наша библиотека может быть легко интегрирована в приложения .NET. Улучшите свои документы с помощью подписей QR-кода, используя наш продукт.
      
      1. Получите файл или поток PDF, который необходимо подписать QR-кодом.
      2. Предоставьте необходимый текст для QrCodeSignOptions.
      3. Настройте визуальные параметры, такие как цвет, положение, размер и т. д.
      4. Сохраните документ с встроенным QR-кодом.
   
    code:
      platform: "net"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Примеры подписей"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "щелкните, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Инициализируйте новый экземпляр Signature с документом
        using (Signature signature = new Signature("input.pdf"))
        {
            // Используйте QrCodeSignOptions для встраивания QR-кода в документ
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // Укажите тип подписи и определите её положение на странице
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // Сохраните документ с интегрированным QR-кодом
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Комплексная интеграция подписей для документов"
  description: "С помощью API GroupDocs.Signature for .NET пользователи могут без усилий генерировать, изменять, искать, проверять и удалять разнообразные типы подписей, оптимизируя рабочие процессы с документами с беспрецедентной точностью."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Ключевые функции GroupDocs.Signature"
  features:
    # feature loop
    - title: "Подписание документов с несколькими типами подписей"
      content: "GroupDocs.Signature позволяет применять текстовые, изображенческие, штрих-кодовые, QR-кодовые и штампованные подписи к любому формату документа. Подписи могут быть точно размещены на любой странице, а управление метаданными может осуществляться через метаданные подписей. Защитите целостность своих документов, внедрив цифровые сертификаты, которые предотвращают несанкционированные изменения."

    # feature loop
    - title: "Поиск и валидация подписей"
      content: "Проверьте подлинность и точность подписей документа с помощью продвинутого процесса валидации. Легко получите подробный список всех подписей, встроенных в документ, для комплексного контроля."

    # feature loop
    - title: "Настраиваемое редактирование подписей"
      content: "Обновляйте и доработывайте ранее нанесенные подписи, изменяя содержимое, расположение, цвет, размер и другие атрибуты в соответствии с вашими конкретными требованиями."

    # feature loop
    - title: "Эффективное удаление подписей"
      content: "Оптимизируйте управление документами, программно удаляя ненужные подписи. Независимо от того, касается ли это цифровых сертификатов или других видов подписей, удаление может быть выполнено быстро и эффективно."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Как сгенерировать QR-код с различными параметрами?"
      content: |
        Этот пример демонстрирует, как разместить настроенный QR-код на странице PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Получите документ для подписи и передайте его в Signature
          using (Signature signature = new Signature("input.pdf"))
          {
              // Настройте параметры QR-кода с необходимым текстом
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // Укажите относительное положение QR-кода на странице
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // Установите отступы для подписи
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // Укажите цвет QR-кода
                    ForeColor = Color.Red,

                    // Определите параметры шрифта для сообщения
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // Настройте цвет фона QR-кода и его стиль
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // Вставьте QR-код в документ
              SignResult result = signature.Sign("output.pdf", options);
          }
          ```
        platform: "net"
        copy_title: "Копировать"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "щелкните, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.pdf"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Используйте функции GroupDocs.Signature бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачивание Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Узнайте о наших решениях по подписям"
    exclude: "qrcode"
    description: "С гордостью представляем широкий спектр типов подписей и эксплуатационных возможностей"
    items: 
          
        # operation loop 1
        - name: "Электронные подписи"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "Добавляйте различные типы подписей к поддерживаемым форматам файлов"

        # operation loop 2
        - name: "Добавить текст в документы"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "Усовершенствуйте содержимое документа настраиваемыми текстовыми подписями"

        # operation loop 3
        - name: "Подписи изображений"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "Размещайте любое изображение в любом месте документа"

        # operation loop 4
        - name: "Генерация штрихкодов"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "Создавайте и вставляйте различные штрихкоды в поддерживаемые документы"

        # operation loop 5
        - name: "Генерация QR-кодов"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "Генерируйте QR-коды для подписания документов"
          
        # operation loop 6
        - name: "Цифровые сертификаты"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Защищайте документы и подписывайте их с помощью цифровых сертификатов"

        # operation loop 7
        - name: "Штамповые подписи"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
          description: "Используйте Конструктор штампов для создания настраиваемых круглых или квадратных штампов"
          
        # operation loop 8
        - name: "Поиск подписей"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "Находите любые ранее добавленные подписи в документе"
          
        # operation loop 9
        - name: "Проверка подписи"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "Подтверждайте подлинность подписей после их применения"
          
        # operation loop 10
        - name: "Изменение подписей"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "Редактируйте разнообразные подписи в документе"
          
        # operation loop 11
        - name: "Удаление подписей"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "Удаляйте широкий спектр ранее примененных подписей"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Генерация QR-кодов для других форматов документов"
    exclude: "PDF"
    description: "Улучшите все стандартные форматы файлов с возможностью встраивания QR-кодов с помощью API .NET. Храните и кодируйте критически важную информацию в 2D-штрих-коды для бесшовного сканирования и извлечения данных."
    items: 
          
        # format loop 1
        - name: "QR-код для PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "Формат документа, независимый от аппаратных средств Adobe"
          
        # format loop 2
        - name: "QR-код для DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-код для JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "Изображение JPEG"
          
        # format loop 4
        - name: "QR-код для PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-код для XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---