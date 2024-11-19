



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:15
draft: false
lang: ru
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Добавьте текстовые подписи к DOCX с помощью Python"
head_description: "Используйте API Python для вставки текстовых подписей в файлы DOCX, поддерживающие форматы такие как PDF, Word, Excel, PowerPoint, изображения и ZIP."

############################# Header ############################
title: "Добавьте текстовые подписи к DOCX" 
description: "Интегрируйте настраиваемые текстовые подписи в ваши документы с использованием GroupDocs.Signature for Python via .NET. Упростите свои рабочие процессы с гибкими параметрами настройки подписей."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Попробуйте бесплатно сегодня"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Исследуйте возможности GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Узнать больше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) предлагает всестороннюю платформу для вставки настраиваемых текстовых подписей, делая рабочие процессы с документами более удобными. Персонализируйте содержимое и внешний вид подписей в разных документах, чтобы повысить эффективность и улучшить управление документами.

############################# Steps ############################
steps:
    enable: true
    title: "Как создать текстовые подписи для DOCX с помощью Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) позволяет легко интегрировать текстовые подписи в файлы DOCX в приложениях Python via .NET. Быстро добавьте функциональность в свои продукты с помощью этого решения.
      
      1. Передайте документ DOCX в конструктор Signature.
      2. Создайте TextSignOptions с текстом вашей подписи.
      3. Настройте визуальные свойства подписи.
      4. Вставьте подпись на желаемые страницы документа.
   
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

            # Инициализируйте Signature с путем к документу
            with sg.Signature('input.docx') as signature:

                # Настройте TextSignOptions с вашим желаемым текстом подписи
                options = sg.TextSignOptions("Approved")

                # Выберите цвет и шрифт для подписи
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # Примените текстовую подпись к документу
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Полное управление текстовыми подписями"
  description: "GroupDocs.Signature for Python via .NET помогает вам управлять рабочими процессами документов, добавляя настраиваемые текстовые подписи к популярным форматам. Контролируйте внешний вид, размещение и содержимое подписей в соответствии с вашими потребностями."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Изучите функции GroupDocs.Signature"
  features:
    # feature loop
    - title: "Гибкие подписи для документов"
      content: "Добавляйте различные типы подписей — текстовые, изображения, штрих-коды, QR-коды и печати — на любую страницу документа. Используйте метаданные для включения скрытой информации и защиты ваших файлов с помощью цифровых сертификатов."

    # feature loop
    - title: "Проверка и поиск подписей"
      content: "Используйте расширенные инструменты для проверки целостности ваших подписанных документов. Ищите и анализируйте все подписи в файле для дальнейшей валидации."

    # feature loop
    - title: "Редактирование или удаление подписей"
      content: "Обновляйте содержимое, внешний вид или размещение существующих подписей. Удаляйте устаревшие подписи, чтобы ваши документы оставались актуальными."

    # feature loop
    - title: "Специализированные текстовые подписи"
      content: "Применяйте текстовые подписи, специфичные для документов, такие как водяные знаки для файлов Word или штампы для PDF, добавляя дополнительный уровень контроля и настройки."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Добавление текстовых подписей в документы"
      content: |
        Узнайте, как вставлять текстовые подписи в документы, чтобы оптимизировать ваши процессы.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Выберите документ для подписи
              with sg.Signature('input.docx') as signature:

                    # Настройте текстовые параметры с желаемым содержанием
                    options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                    # Определите размер и размещение подписи
                    options.Left = 100
                    options.Top = 180
                    options.Width = 230
                    options.Height = 30

                    # Установите отступы от краев страницы
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Выберите цвет текста и стиль шрифта
                    options.ForeColor = sg.Color.Red
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Добавьте рамку вокруг текстовой подписи
                    options.Border = sg.Border()
                    options.Border.Color = sg.Color.Red
                    options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                    options.Border.Transparency = 0.5
                    options.Border.Visible = True
                    options.Border.Weight = 2

                    # Настройте фон при необходимости
                    options.Background = sg.Background()
                    options.Background.Color = sg.Color.Yellow
                    options.Background.Transparency = 0.8

                    # Опционально сохраните подпись как изображение для совместимости
                    options.SignatureImplementation = sg.TextSignatureImplementation.Image

                    # Сохраните документ с встраиваемой подписью
                    result = signature.Sign("output.docx", options)
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
            link: "/examples/signature/formats/signature_text.docx"
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
    title: "Расширенные функции подписей"
    exclude: "text"
    description: "Наш API поддерживает полное управление жизненным циклом для семи типов подписей, позволяя вам создавать, управлять, проверять и настраивать ваши подписи."
    items: 
          
        # operation loop 1
        - name: "Электронные подписи"
          operation: "esign"
          link: "/signature/python-net/esign/docx/"
          description: "Добавляйте различные типы подписей к поддерживаемым форматам файлов"

        # operation loop 2
        - name: "Добавить текст в документы"
          operation: "text"
          link: "/signature/python-net/text/docx/"
          description: "Усовершенствуйте содержимое документа настраиваемыми текстовыми подписями"

        # operation loop 3
        - name: "Подписи изображений"
          operation: "image"
          link: "/signature/python-net/image/docx/"
          description: "Размещайте любое изображение в любом месте документа"

        # operation loop 4
        - name: "Генерация штрихкодов"
          operation: "barcode"
          link: "/signature/python-net/barcode/docx/"
          description: "Создавайте и вставляйте различные штрихкоды в поддерживаемые документы"

        # operation loop 5
        - name: "Генерация QR-кодов"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/docx/"
          description: "Генерируйте QR-коды для подписания документов"
          
        # operation loop 6
        - name: "Цифровые сертификаты"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "Защищайте документы и подписывайте их с помощью цифровых сертификатов"

        # operation loop 7
        - name: "Штамповые подписи"
          operation: "stamp"
          link: "/signature/python-net/stamp/docx/"
          description: "Используйте Конструктор штампов для создания настраиваемых круглых или квадратных штампов"
          
        # operation loop 8
        - name: "Поиск подписей"
          operation: "search"
          link: "/signature/python-net/search/docx/"
          description: "Находите любые ранее добавленные подписи в документе"
          
        # operation loop 9
        - name: "Проверка подписи"
          operation: "verify"
          link: "/signature/python-net/verify/docx/"
          description: "Подтверждайте подлинность подписей после их применения"
          
        # operation loop 10
        - name: "Изменение подписей"
          operation: "modify"
          link: "/signature/python-net/modify/docx/"
          description: "Редактируйте разнообразные подписи в документе"
          
        # operation loop 11
        - name: "Удаление подписей"
          operation: "delete"
          link: "/signature/python-net/delete/docx/"
          description: "Удаляйте широкий спектр ранее примененных подписей"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Встраивание текстовых подписей в несколько форматов"
    exclude: "DOCX"
    description: "С помощью API Python via .NET вы можете добавлять текстовые подписи в различные офисные документы, получая полный контроль над жизненным циклом документа и улучшая безопасность."
    items: 
          
        # format loop 1
        - name: "Подписи текста в PDF"
          format: "PDF"
          link: "/signature/python-net/text/pdf/"
          description: "Формат документа, независимый от аппаратных средств Adobe"
          
        # format loop 2
        - name: "Подписи текста в DOCX"
          format: "DOCX"
          link: "/signature/python-net/text/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Подписи текста в JPEG"
          format: "JPEG"
          link: "/signature/python-net/text/jpeg/"
          description: "Изображение JPEG"
          
        # format loop 4
        - name: "Подписи текста в PPTX"
          format: "PPTX"
          link: "/signature/python-net/text/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 5
        - name: "Подписи текста в XLSX"
          format: "XLSX"
          link: "/signature/python-net/text/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---