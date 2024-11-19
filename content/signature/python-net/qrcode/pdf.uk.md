



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:23
draft: false
lang: uk
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Генеруйте QR-коди для файлів PDF за допомогою Python"
head_description: "Використовуйте API GroupDocs.Signature для генерації та вбудовування QR-кодів у файли PDF. Легко розміщуйте QR-коди на будь-якій сторінці, щоб додати додаткову функціональність."

############################# Header ############################
title: "Генеруйте QR-коди для PDF" 
description: "Створюйте 2D-штрих-коди, використовуючи текст або числові дані, та застосовуйте їх до різних сторінок і форматів, включаючи PDF, Word, Excel та інше за допомогою GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Безкоштовна пробна версія"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Досліджуйте можливості GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Дізнатися більше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) пропонує широкий спектр можливостей, дозволяючи користувачам генерувати та вбудовувати різні типи підписів у основних форматах документів. Незалежно від того, чи це PDF, Word, Excel, PowerPoint чи зображення, покращуйте свої документи підписами: Текстовими, Зображеннями, Штрих-кодами, QR-кодами, Метаданими, Цифровими або Штампами.

############################# Steps ############################
steps:
    enable: true
    title: "Кроки для генерації та вставки QR-коду в PDF"
    content: |
      [GroupDocs.Signature](/signature/python-net/) дозволяє створювати QR-коди у популярних форматах та розміщувати їх на сторінках PDF. Завдяки підтримці понад 10 типів QR-кодів, ви можете безперешкодно інтегрувати цю функціональність у додатки Python via .NET. Покращте свої документи підписами QR-кодів за допомогою нашого продукту.
      
      1. Отримайте файл PDF або потік, куди буде додано QR-код.
      2. Надайте необхідний текст у QrCodeSignOptions.
      3. Налаштуйте візуальні параметри, такі як колір, позиція та розмір.
      4. Збережіть документ з вбудованим QR-кодом.
   
    code:
      platform: "python-net"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Приклад підписів"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "натисніть для копіювання"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Ініціалізуйте новий екземпляр Signature з документом
            with sg.Signature('input.pdf') as signature:

                # Використовуйте QrCodeSignOptions для вбудовування QR-коду в документ
                options = sg.QrCodeSignOptions("Text Content")

                # Вкажіть тип підпису та задайте його позицію на сторінці
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # Збережіть документ з вбудованим QR-кодом
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Комплексна інтеграція підписів для документів"
  description: "З API GroupDocs.Signature for Python via .NET користувачі можуть генерувати, змінювати, шукати, підтверджувати та видаляти різні типи підписів, спростивши документи за допомогою точності."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Ключові особливості GroupDocs.Signature"
  features:
    # feature loop
    - title: "Застосування кількох типів підписів"
      content: "GroupDocs.Signature дозволяє застосовувати текстові, зображення, штрих-коди, QR-коди та штампи до будь-якого документа. Ви можете точно розміщувати підписи на будь-якій сторінці та легко керувати метаданими. Захистіть свої документи від несанкціонованих змін за допомогою цифрових сертифікатів."

    # feature loop
    - title: "Шукати та підтверджувати підписи"
      content: "Перевіряйте підписи документів на достовірність та точність за допомогою розширених інструментів перевірки. Легко отримуйте детальний список усіх підписів, інтегрованих у документ, для кращого контролю."

    # feature loop
    - title: "Змінюйте наявні підписи"
      content: "Ви можете оновлювати раніше застосовані підписи, налаштовуючи вміст, позицію, колір, розмір та інші атрибути відповідно до ваших конкретних потреб."

    # feature loop
    - title: "Швидко видаляйте підписи"
      content: "Оптимізуйте управління документами, швидко видаляючи непотрібні підписи. Незалежно від того, чи це цифровий сертифікат або інший тип підпису, видалення можна виконати ефективно."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Налаштування згенерованого QR-коду"
      content: |
        Цей приклад показує, як розмістити налаштований QR-код на сторінці PDF.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Отримайте документ, що підписується, та передайте його в Signature
              with sg.Signature('input.pdf') as signature:

                    # Налаштуйте параметри QR-коду з необхідним текстом
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # Встановіть позицію QR-коду на сторінці
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # Встановіть відступи для підпису
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Виберіть колір QR-коду
                    options.ForeColor = sg.Color.Red

                    # Визначте шрифтові параметри для повідомлення
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Встановіть колір фону та малюнок для QR-коду
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # Вбудуйте QR-код у документ
                    result = signature.Sign("output.pdf", options)
          ```
        platform: "python-net"
        copy_title: "Копіювати"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "натисніть для копіювання"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.pdf"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Спробуйте можливості GroupDocs.Signature безкоштовно або запросіть ліцензію"
  items:
    #  loop
    - title: "Завантаження PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Досліджуйте наші рішення для підписів"
    exclude: "qrcode"
    description: "Ми пропонуємо широкий вибір типів підписів та операцій, щоб задовольнити ваші документообігові потреби."
    items: 
          
        # operation loop 1
        - name: "Електронні підписи"
          operation: "esign"
          link: "/signature/python-net/esign/pdf/"
          description: "Додавайте різні типи підписів до підтримуваних форматів файлів"

        # operation loop 2
        - name: "Додати текст до документів"
          operation: "text"
          link: "/signature/python-net/text/pdf/"
          description: "Збагачуйте вміст документів настроювальними текстовими підписами"

        # operation loop 3
        - name: "Зображення підписів"
          operation: "image"
          link: "/signature/python-net/image/pdf/"
          description: "Розміщуйте будь-яке зображення у будь-якому місці документа"

        # operation loop 4
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/signature/python-net/barcode/pdf/"
          description: "Створюйте та вставляйте різні штрих-коди у підтримувані документи"

        # operation loop 5
        - name: "Генерувати QR-коди"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Генеруйте QR-коди для підписання документів"
          
        # operation loop 6
        - name: "Цифрові сертифікати"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Захистіть бізнес і підписуйте документи за допомогою цифрових сертифікатів"

        # operation loop 7
        - name: "Печатки підписів"
          operation: "stamp"
          link: "/signature/python-net/stamp/pdf/"
          description: "Використовуйте Конструктор печаток для створення індивідуальних круглих або квадратних печаток"
          
        # operation loop 8
        - name: "Шукати підписи"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "Знаходьте будь-які попередньо додані підписи в документі"
          
        # operation loop 9
        - name: "Перевірка підписів"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "Перевіряйте автентичність підписів після їхнього застосування"
          
        # operation loop 10
        - name: "Змінювати підписи"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "Редагуйте різноманітні підписи в документі"
          
        # operation loop 11
        - name: "Видалити підписи"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "Видаляйте широкий спектр раніше застосованих підписів"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Вбудовуйте QR-коди в різні формати документів"
    exclude: "PDF"
    description: "Використовуйте API Python via .NET для вбудовування QR-кодів у будь-який стандартний формат документів. Зберігайте та кодуйте важливу інформацію у 2D-штрих-кодах для простого сканування та отримання даних."
    items: 
          
        # format loop 1
        - name: "QR-Код для PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Адріс фільмування документів Adobe"
          
        # format loop 2
        - name: "QR-Код для DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Код для JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Зображення JPEG"
          
        # format loop 4
        - name: "QR-Код для PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Код для XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---