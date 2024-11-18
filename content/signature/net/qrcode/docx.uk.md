



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:02
draft: false
lang: uk
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Генерація QR-коду для файлів DOCX за допомогою C#"
head_description: "Використовуйте API GroupDocs.Signature для генерації QR-коду для файлів DOCX. Безперешкодно вставляйте QR-коди на будь-яку сторінку для покращення функціональності."

############################# Header ############################
title: "Генерація QR-кодів для DOCX" 
description: "Генеруйте 2D-штрих-коди, використовуючи текстові або числові дані, та застосовуйте їх на кількох сторінках і в різних форматах, включаючи PDF, Word, Excel та інше, завдяки GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Розпочніть безкоштовну пробну версію"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Відкрийте можливості GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Дізнатися більше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) пропонує широкий спектр функцій, надаючи користувачам можливість генерувати та вбудовувати різні типи підписів у провідні формати документів. Чи це PDF, Word, Excel, PowerPoint чи зображення, ви можете підняти свої документи за допомогою текстових, зображень, штрих-кодів, QR-кодів, метаданих, цифрових підписів і штампів.

############################# Steps ############################
steps:
    enable: true
    title: "Як згенерувати та вставити QR-код у будь-яке місце в DOCX"
    content: |
      [GroupDocs.Signature](/signature/net/) полегшує генерацію QR-кодів у різних популярних форматах і їх розміщення на сторінках DOCX. Підтримуючи понад 10 типів QR-кодів, наша бібліотека може бути безперешкодно інтегрована в програми .NET. Покращте свої документи, використовуючи підписи з QR-кодами за допомогою нашого продукту.
      
      1. Отримайте файл або потік DOCX, який потрібно підписати з QR-кодом.
      2. Надайте необхідний текст для QrCodeSignOptions.
      3. Налаштуйте візуальні параметри такі як колір, положення, розмір тощо.
      4. Збережіть документ з вбудованим QR-кодом.
   
    code:
      platform: "net"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Приклад підписів"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "натисніть для копіювання"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Ініціалізуйте новий екземпляр Signature з документом
        using (Signature signature = new Signature("input.docx"))
        {
            // Використовуйте QrCodeSignOptions для вбудовування QR-коду в документ
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // Вкажіть тип підпису та визначте його положення на сторінці
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // Збережіть документ з інтегрованим QR-кодом
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Комплексна інтеграція підписів для документів"
  description: "З API GroupDocs.Signature for .NET користувачі можуть генерувати, змінювати, шукати, перевіряти та видаляти різні типи підписів, оптимізуючи документи з неперевершеною точністю."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Ключові функції GroupDocs.Signature"
  features:
    # feature loop
    - title: "Підпис документа з кількома типами підписів"
      content: "GroupDocs.Signature дозволяє застосовувати текстові, зображення, штрих-коди, QR-коди та штампи до будь-якого формату документа. Підписи можна точно розміщувати на будь-якій сторінці, а метадані можна безперешкодно керувати через підписи метаданих. Захистіть цілісність ваших документів, використовуючи цифрові сертифікати, які запобігають несанкціонованим змінам."

    # feature loop
    - title: "Пошук та перевірка підписів"
      content: "Перевірте автентичність та точність підписів документів за допомогою вдосконаленого процесу валідації. Легко отримуйте детальний список усіх підписів, вбудованих у документ для всебічного контролю."

    # feature loop
    - title: "Налаштування модифікації підписів"
      content: "Оновлюйте та вдосконалюйте раніше застосовані підписи, змінюючи вміст, розміщення, колір, розмір та інші атрибути відповідно до ваших специфічних потреб."

    # feature loop
    - title: "Ефективне видалення підписів"
      content: "Оптимізуйте управління документами шляхом програмного видалення небажаних підписів. Незалежно від того, йдеться про цифрові сертифікати чи інші типи підписів, видалення можна здійснити швидко та ефективно."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Як згенерувати QR-код з різними опціями?"
      content: |
        Цей приклад демонструє, як розмістити настроюваний QR-код на сторінці DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Отримайте документ, який потрібно підписати, і передайте його в Signature
          using (Signature signature = new Signature("input.docx"))
          {
              // Налаштуйте опції QR-коду з необхідним текстом
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // Визначте відносне положення QR-коду на сторінці
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // Встановіть відступ підпису
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // Вкажіть колір QR-коду
                    ForeColor = Color.Red,

                    // Визначте шрифтові параметри для повідомлення
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // Налаштуйте колір фону QR-коду та пензлик
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // Вбудуйте QR-код у документ
              SignResult result = signature.Sign("output.docx", options);
          }
          ```
        platform: "net"
        copy_title: "Копіювати"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "натисніть для копіювання"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.docx"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Спробуйте можливості GroupDocs.Signature безкоштовно або запросіть ліцензію"
  items:
    #  loop
    - title: "Завантаження Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Дізнайтеся про наші рішення для підписів"
    exclude: "qrcode"
    description: "Ми гордо представляємо широкий спектр типів підписів і оперативних функцій."
    items: 
          
        # operation loop 1
        - name: "Електронні підписи"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "Додавайте різні типи підписів до підтримуваних форматів файлів"

        # operation loop 2
        - name: "Додати текст до документів"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "Збагачуйте вміст документів настроювальними текстовими підписами"

        # operation loop 3
        - name: "Зображення підписів"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "Розміщуйте будь-яке зображення у будь-якому місці документа"

        # operation loop 4
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "Створюйте та вставляйте різні штрих-коди у підтримувані документи"

        # operation loop 5
        - name: "Генерувати QR-коди"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "Генеруйте QR-коди для підписання документів"
          
        # operation loop 6
        - name: "Цифрові сертифікати"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "Захистіть бізнес і підписуйте документи за допомогою цифрових сертифікатів"

        # operation loop 7
        - name: "Печатки підписів"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "Використовуйте Конструктор печаток для створення індивідуальних круглих або квадратних печаток"
          
        # operation loop 8
        - name: "Шукати підписи"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "Знаходьте будь-які попередньо додані підписи в документі"
          
        # operation loop 9
        - name: "Перевірка підписів"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "Перевіряйте автентичність підписів після їхнього застосування"
          
        # operation loop 10
        - name: "Змінювати підписи"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "Редагуйте різноманітні підписи в документі"
          
        # operation loop 11
        - name: "Видалити підписи"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "Видаляйте широкий спектр раніше застосованих підписів"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Генерація QR-кодів для інших форматів документів"
    exclude: "DOCX"
    description: "Покращте всі стандартні формати файлів можливістю вбудовувати QR-коди за допомогою API .NET. Зберігайте та кодуйте важливу інформацію в 2D-штрих-кодах для безперешкодного сканування та отримання даних."
    items: 
          
        # format loop 1
        - name: "QR-Код для PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "Адріс фільмування документів Adobe"
          
        # format loop 2
        - name: "QR-Код для DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Код для JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "Зображення JPEG"
          
        # format loop 4
        - name: "QR-Код для PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Код для XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---