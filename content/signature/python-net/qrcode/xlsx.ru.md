



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:03
draft: false
lang: ru
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Генерация QR-кодов для файлов XLSX с использованием Python"
head_description: "Используйте API GroupDocs.Signature для генерации и интеграции QR-кодов в файлы XLSX. Размещайте QR-коды на любой странице для добавления дополнительных возможностей."

############################# Header ############################
title: "Генерация QR-кодов для XLSX" 
description: "Создавайте двумерные штрих-коды с использованием текстовых или численных данных и применяйте их на различных страницах и форматах, включая PDF, Word, Excel и многое другое с помощью GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Бесплатная пробная версия"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Изучите возможности GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Узнать больше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) предлагает широкий спектр возможностей, позволяя пользователям генерировать и встроить различные типы подписей в основных форматах документов. Будь то PDF, Word, Excel, PowerPoint или изображения, улучшите свои документы с помощью текстовых, изображенческих, штрих-кодов, QR-кодов, метаданных, цифровых или печатных подписей.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги для генерации и вставки QR-кода в XLSX"
    content: |
      [GroupDocs.Signature](/signature/python-net/) позволяет создавать QR-коды в популярных форматах и размещать их на страницах XLSX. С поддержкой более 10 типов QR-кодов вы можете безупречно интегрировать эту функциональность в приложения Python via .NET. Улучшите свои документы с помощью подписей QR-кодов, используя наш продукт.
      
      1. Получите файл или поток XLSX, в который будет добавлен QR-код.
      2. Предоставьте необходимый текст для QrCodeSignOptions.
      3. Настройте визуальные параметры, такие как цвет, положение и размер.
      4. Сохраните документ с встроенным QR-кодом.
   
    code:
      platform: "python-net"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Примеры подписей"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "щелкните, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Инициализируйте новый экземпляр Signature с документом
            with sg.Signature('input.xlsx') as signature:

                # Используйте QrCodeSignOptions для встраивания QR-кода в документ
                options = sg.QrCodeSignOptions("Text Content")

                # Укажите тип подписи и задайте её положение на странице
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # Сохраните документ с встроенным QR-кодом
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Полноценная интеграция подписей для документов"
  description: "С помощью API GroupDocs.Signature for Python via .NET пользователи могут генерировать, изменять, искать, проверять и удалять различные типы подписей, упрощая рабочие процессы с документами с высокой точностью."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Ключевые особенности GroupDocs.Signature"
  features:
    # feature loop
    - title: "Применение нескольких типов подписей"
      content: "GroupDocs.Signature позволяет применять текстовые, изображенческие, штрих-коды, QR-коды и печатные подписи к любому документу. Вы можете точно размещать подписи на любой странице и управлять метаданными. Защитите свои документы от несанкционированных изменений с помощью цифровых сертификатов."

    # feature loop
    - title: "Поиск и проверка подписей"
      content: "Проверяйте подписи документов на подлинность и точность с помощью продвинутых инструментов валидации. Легко получите подробный список всех подписей, встроенных в документ, для лучшего контроля."

    # feature loop
    - title: "Изменение существующих подписей"
      content: "Вы можете обновлять ранее применённые подписи, настраивая содержимое, положение, цвет, размер и другие параметры в соответствии с вашими конкретными требованиями."

    # feature loop
    - title: "Удаление подписей"
      content: "Облегчите управление документами, быстро удаляя ненужные подписи. Будь то цифровой сертификат или другой тип подписи, удаление производится эффективно."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Настройка сгенерированного QR-кода"
      content: |
        Этот пример демонстрирует, как разместить настроенный QR-код на странице XLSX.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Получите документ для подписи и передайте его в Signature
              with sg.Signature('input.xlsx') as signature:

                    # Настройте опции QR-кода с необходимым текстом
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # Установите положение QR-кода на странице
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # Настройте отступ для подписи
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Выберите цвет QR-кода
                    options.ForeColor = sg.Color.Red

                    # Определите параметры шрифта для сообщения
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Установите цвет фона и кисть для QR-кода
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # Встраивайте QR-код в документ
                    result = signature.Sign("output.xlsx", options)
          ```
        platform: "python-net"
        copy_title: "Копировать"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "щелкните, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.xlsx"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Используйте функции GroupDocs.Signature бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачивание PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Изучите наши решения по подписям"
    exclude: "qrcode"
    description: "Мы предлагаем широкий выбор типов подписей и операций для удовлетворения ваших потребностей в документах."
    items: 
          
        # operation loop 1
        - name: "Электронные подписи"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "Добавляйте различные типы подписей к поддерживаемым форматам файлов"

        # operation loop 2
        - name: "Добавить текст в документы"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "Усовершенствуйте содержимое документа настраиваемыми текстовыми подписями"

        # operation loop 3
        - name: "Подписи изображений"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "Размещайте любое изображение в любом месте документа"

        # operation loop 4
        - name: "Генерация штрихкодов"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Создавайте и вставляйте различные штрихкоды в поддерживаемые документы"

        # operation loop 5
        - name: "Генерация QR-кодов"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Генерируйте QR-коды для подписания документов"
          
        # operation loop 6
        - name: "Цифровые сертификаты"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "Защищайте документы и подписывайте их с помощью цифровых сертификатов"

        # operation loop 7
        - name: "Штамповые подписи"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Используйте Конструктор штампов для создания настраиваемых круглых или квадратных штампов"
          
        # operation loop 8
        - name: "Поиск подписей"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "Находите любые ранее добавленные подписи в документе"
          
        # operation loop 9
        - name: "Проверка подписи"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "Подтверждайте подлинность подписей после их применения"
          
        # operation loop 10
        - name: "Изменение подписей"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "Редактируйте разнообразные подписи в документе"
          
        # operation loop 11
        - name: "Удаление подписей"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "Удаляйте широкий спектр ранее примененных подписей"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Встраивание QR-кодов в различные форматы документов"
    exclude: "XLSX"
    description: "Используйте API Python via .NET для интеграции QR-кодов в любой стандартный формат документа. Храните и кодируйте важную информацию в двумерных штрих-кодах для простоты сканирования и извлечения данных."
    items: 
          
        # format loop 1
        - name: "QR-код для PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Формат документа, независимый от аппаратных средств Adobe"
          
        # format loop 2
        - name: "QR-код для DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-код для JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Изображение JPEG"
          
        # format loop 4
        - name: "QR-код для PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-код для XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---