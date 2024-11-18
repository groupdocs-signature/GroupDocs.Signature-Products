



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:08
draft: false
lang: uk
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Вставте штрих-код у ваш XLSX з Python"
head_description: "Ефективно додавайте штрих-кодні підписи до документів XLSX з кількома рядками коду в Python. GroupDocs.Signature забезпечує безшовні рішення для підписання багатьох форматів документів."

############################# Header ############################
title: "Генерація штрих-кодів для XLSX" 
description: "За допомогою GroupDocs.Signature for Python via .NET ви можете розміщувати штрих-коди у ваших бізнес-документах у будь-якому необхідному місці. Наше рішення пропонує гнучкі варіанти для налаштування підпису штрих-коду."
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
    title: "Про GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Дізнатися більше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) – це потужний інструмент для підписання документів, який підтримує широкий спектр типів підписів, включаючи текст, зображення, штрих-коди, цифрові сертифікати та печатки. Сумісний більш ніж з 60 форматами файлів, такими як PDF, MS Office, зображення, ZIP та інші, він не лише дозволяє вам застосовувати підписи, але й дозволяє шукати, перевіряти, змінювати або видаляти їх за потреби.

############################# Steps ############################
steps:
    enable: true
    title: "Кроки для генерації та вставки штрих-коду в XLSX"
    content: |
      [GroupDocs.Signature](/signature/python-net/) дозволяє швидко та ефективно генерувати і вбудовувати штрих-коди в документи XLSX. Підтримуючи понад 60 форматів штрих-кодів, програми Python via .NET можуть безперешкодно додавати функціональність підписання штрих-кодів, інтегруючи нашу бібліотеку.
      
      1. Надайте файл XLSX або потік для обробки.
      2. Вкажіть текст штрих-коду для об'єкта BarcodeSignOptions.
      3. Налаштуйте параметри штрих-коду, такі як позиція і розмір.
      4. Збережіть документ з вбудованим штрих-кодом.
   
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

            # Ініціалізуйте об'єкт Signature з шляхом до документа
            with sg.Signature('input.xlsx') as signature:

                # Використовуйте BarcodeSignOptions для додавання штрих-коду до документа
                options = sg.BarcodeSignOptions('Business data')

                # Встановіть тип штрих-коду та налаштуйте його властивості
                options.EncodeType = sg.BarcodeTypes.Code128
                options.Left = 50
                options.Top = 150

                # Збережіть підписаний документ
                result = signature.Sign('output.xlsx', options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Покращте свої документи розширеними функціями підпису"
  description: "Бібліотека GroupDocs.Signature for Python via .NET надає комплексні рішення для підписання та обробки документів у загально вживаних форматах. Ви можете додавати, змінювати, перевіряти або видаляти різні типи підписів відповідно до ваших потреб."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Ключові особливості GroupDocs.Signature"
  features:
    # feature loop
    - title: "Гнучке підписання документів"
      content: "Підписуйте будь-яку сторінку в підтримуваних документах текстом, зображеннями, штрих-кодами, QR-кодами або печатками. Додавайте приховані метадані, такі як EXIF-дані в зображеннях, та забезпечуйте захист вмісту цифровими сертифікатами, щоб запобігти несанкціонованим змінам."

    # feature loop
    - title: "Шукайте та перевіряйте підписи"
      content: "Наш інструмент забезпечує цілісність ваших документів, дозволяючи перевіряти підписи. Ви також можете отримати повний список усіх підписів у документі для зручного управління."

    # feature loop
    - title: "Змінюйте підписи без зусиль"
      content: "Модифікуйте наявні підписи без труднощів. Налаштуйте текст, перемістіть елементи або змініть кольори, щоб відповідати потребам вашого документа."

    # feature loop
    - title: "Легко видаляйте підписи"
      content: "З повною функціональністю CRUD GroupDocs.Signature for Python via .NET спрощує видалення будь-яких небажаних або застарілих підписів з ваших документів."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Створення та розміщення підпису штрих-коду"
      content: |
        Цей приклад демонструє, як вставити користувацький штрих-код у документ XLSX.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Надайте документ для підписання
              with sg.Signature('input.xlsx') as signature:

                  # Встановіть текст штрих-коду та параметри підпису
                  options = sg.BarcodeSignOptions('Accepted')
                  options.EncodeType = sg.BarcodeTypes.Code39FullASCII

                  # Виберіть місце для штрих-коду на сторінці
                  options.VerticalAlignment = sg.VerticalAlignment.Top
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left

                  # Встановіть відстань між штрих-кодом і краєм сторінки
                  options.Margin = sg.Padding()
                  options.Margin.Top = 180
                  options.Margin.Right = 20

                  # Вкажіть колір смужок штрих-коду
                  options.ForeColor = sg.Color.Red

                  # Виберіть стиль шрифту для повідомлення штрих-коду
                  options.Font = sg.SignatureFont()
                  options.Font.Size = 12
                  options.Font.FamilyName = 'Arial'

                  # Встановіть позицію тексту повідомлення
                  options.CodeTextAlignment = sg.CodeTextAlignment.Above

                  # Підпишіть і збережіть документ
                  result = signature.Sign('output.xlsx', options)
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
            link: "/examples/signature/formats/signature_barcode.xlsx"
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
    title: "Ознайомтеся з нашими ключовими функціями"
    exclude: "barcode"
    description: "Ми пропонуємо широкий спектр варіантів підпису та операцій для ваших документів."
    items: 
          
        # operation loop 1
        - name: "Електронні підписи"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "Додавайте різні типи підписів до підтримуваних форматів файлів"

        # operation loop 2
        - name: "Додати текст до документів"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "Збагачуйте вміст документів настроювальними текстовими підписами"

        # operation loop 3
        - name: "Зображення підписів"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "Розміщуйте будь-яке зображення у будь-якому місці документа"

        # operation loop 4
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Створюйте та вставляйте різні штрих-коди у підтримувані документи"

        # operation loop 5
        - name: "Генерувати QR-коди"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Генеруйте QR-коди для підписання документів"
          
        # operation loop 6
        - name: "Цифрові сертифікати"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "Захистіть бізнес і підписуйте документи за допомогою цифрових сертифікатів"

        # operation loop 7
        - name: "Печатки підписів"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Використовуйте Конструктор печаток для створення індивідуальних круглих або квадратних печаток"
          
        # operation loop 8
        - name: "Шукати підписи"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "Знаходьте будь-які попередньо додані підписи в документі"
          
        # operation loop 9
        - name: "Перевірка підписів"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "Перевіряйте автентичність підписів після їхнього застосування"
          
        # operation loop 10
        - name: "Змінювати підписи"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "Редагуйте різноманітні підписи в документі"
          
        # operation loop 11
        - name: "Видалити підписи"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "Видаляйте широкий спектр раніше застосованих підписів"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Підписуйте документи у різних форматах"
    exclude: "XLSX"
    description: "API Python via .NET підтримує підписання більше ніж 60 форматів файлів, що дозволяє додавати різні типи підписів на будь-яку сторінку або в конкретне місце в ваших документах."
    items: 
          
        # format loop 1
        - name: "Додати штрих-код до PDF"
          format: "PDF"
          link: "/signature/python-net/barcode/pdf/"
          description: "Адріс фільмування документів Adobe"
          
        # format loop 2
        - name: "Додати штрих-код до DOCX"
          format: "DOCX"
          link: "/signature/python-net/barcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Додати штрих-код до JPEG"
          format: "JPEG"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Зображення JPEG"
          
        # format loop 4
        - name: "Додати штрих-код до PPTX"
          format: "PPTX"
          link: "/signature/python-net/barcode/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 5
        - name: "Додати штрих-код до XLSX"
          format: "XLSX"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---