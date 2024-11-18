



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:01
draft: false
lang: uk
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Створіть QR-код для PPTX за допомогою Java"
head_description: "API GroupDocs.Signature дозволяє створювати QR-коди для файлів PPTX. Генеруйте QR-коди з вашого контенту та розміщуйте їх на будь-якій сторінці."

############################# Header ############################
title: "Створіть QR-коди для PPTX" 
description: "Створюйте 2D штрих-коди з текстовими та числовими даними та розміщуйте їх на будь-якій сторінці різних документів, використовуючи GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Безкоштовна пробна версія"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Дізнайтесь більше про GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Дізнатися більше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) пропонує широкий спектр можливостей для генерації та вбудовування різних типів підписів у всі основні формати документів. Підтримуються PDF, документи Word, електронні таблиці Excel, презентації PowerPoint та зображення. Покращуйте свої документи підписами тексту, зображень, штрих-кодів, QR-кодів, метаданих, цифровими та штампами.

############################# Steps ############################
steps:
    enable: true
    title: "Кроки для генерації та розміщення QR-коду в будь-якому місці в PPTX"
    content: |
      [GroupDocs.Signature](/signature/java/) може генерувати QR-коди у багатьох популярних форматах і розміщувати їх на сторінках PPTX. Підтримується понад 10 типів QR-кодів, які можна швидко інтегрувати в додатки Java. Використовуйте наш продукт для підписання документів зі згенерованими QR-кодами.
      
      1. Отримайте файл або потік PPTX, який необхідно підписати QR-кодом.
      2. Надайте текст для QrCodeSignOptions.
      3. Налаштуйте візуальні параметри, такі як колір, позиція, розмір тощо.
      4. Збережіть файл з QR-кодом.
   
    code:
      platform: "java"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Приклад підписів"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "натисніть для копіювання"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // Передайте документ до нового екземпляра Signature
        Signature signature = new Signature("input.pptx");

        // Використовуйте QrCodeSignOptions, щоб додати QR-код до документа
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // Вкажіть тип підпису та позицію на сторінці
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // Збережіть файл з доданим QR-кодом
        signature.sign("output.pptx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Додайте підписи до ваших документів"
  description: "API GroupDocs.Signature for Java підтримує підписання всіх популярних форматів файлів. Генеруйте, модифікуйте, шукайте, перевіряйте та видаляйте різні типи підписів."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Ключові функції GroupDocs.Signature"
  features:
    # feature loop
    - title: "Підписуйте документи"
      content: "GroupDocs.Signature підтримує підписання текстом, зображеннями, штрих-кодами, QR-кодами та штампами. Розміщуйте їх на будь-якій сторінці будь-якого підтримуваного формату документа. Керуйте метаданими документів за допомогою метаданих підписів та захищайте контент від несанкціонованих змін за допомогою цифрових сертифікатів."

    # feature loop
    - title: "Пошук та перевірка"
      content: "Переконайтеся, що всі підписи в документі дійсні, шляхом перевірки. Отримуйте повний список підписів у документі, використовуючи вбудовану функцію пошуку."

    # feature loop
    - title: "Модифікація підписів"
      content: "Модифікуйте властивості підпису після підписання. Налаштуйте вміст, позицію, колір, розмір та інші атрибути за необхідності."

    # feature loop
    - title: "Видалення підписів"
      content: "Видаляйте непотрібні підписи без зусиль. Різні типи підписів, включаючи цифрові сертифікати, можуть бути видалені з документів програмно."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Як налаштувати згенерований QR-код"
      content: |
        Використовуйте цей приклад, щоб дізнатися, як розмістити новий QR-код на сторінці PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Отримайте документ, який потрібно підписати, і передайте його до Signature
          Signature signature = new Signature("input.pptx");

          // Використовуйте параметри QR-коду для надання тексту з потрібною інформацією
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // Встановіть відносну позицію QR-коду на сторінці
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // Встановіть відступ для підпису
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Вкажіть колір QR-коду
          signOptions.setForeColor(Color.RED);

          // Визначте параметри шрифту для повідомлення
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Налаштуйте колір фону QR-коду та пензля
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Додайте QR-код до документа
          SignResult signResult = signature.sign("output.pptx", signOptions);
          ```
        platform: "java"
        copy_title: "Копіювати"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "натисніть для копіювання"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.pptx"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Спробуйте можливості GroupDocs.Signature безкоштовно або запросіть ліцензію"
  items:
    #  loop
    - title: "Завантаження Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Ознайомтеся з нашими ключовими пропозиціями"
    exclude: "qrcode"
    description: "Ми пропонуємо різноманітний вибір функцій підпису та розширених операцій."
    items: 
          
        # operation loop 1
        - name: "Електронні підписи"
          operation: "esign"
          link: "/signature/java/esign/pptx/"
          description: "Додавайте різні типи підписів до підтримуваних форматів файлів"

        # operation loop 2
        - name: "Додати текст до документів"
          operation: "text"
          link: "/signature/java/text/pptx/"
          description: "Збагачуйте вміст документів настроювальними текстовими підписами"

        # operation loop 3
        - name: "Зображення підписів"
          operation: "image"
          link: "/signature/java/image/pptx/"
          description: "Розміщуйте будь-яке зображення у будь-якому місці документа"

        # operation loop 4
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/signature/java/barcode/pptx/"
          description: "Створюйте та вставляйте різні штрих-коди у підтримувані документи"

        # operation loop 5
        - name: "Генерувати QR-коди"
          operation: "qrcode"
          link: "/signature/java/qrcode/pptx/"
          description: "Генеруйте QR-коди для підписання документів"
          
        # operation loop 6
        - name: "Цифрові сертифікати"
          operation: "digital"
          link: "/signature/java/digital/pptx/"
          description: "Захистіть бізнес і підписуйте документи за допомогою цифрових сертифікатів"

        # operation loop 7
        - name: "Печатки підписів"
          operation: "stamp"
          link: "/signature/java/stamp/pptx/"
          description: "Використовуйте Конструктор печаток для створення індивідуальних круглих або квадратних печаток"
          
        # operation loop 8
        - name: "Шукати підписи"
          operation: "search"
          link: "/signature/java/search/pptx/"
          description: "Знаходьте будь-які попередньо додані підписи в документі"
          
        # operation loop 9
        - name: "Перевірка підписів"
          operation: "verify"
          link: "/signature/java/verify/pptx/"
          description: "Перевіряйте автентичність підписів після їхнього застосування"
          
        # operation loop 10
        - name: "Змінювати підписи"
          operation: "modify"
          link: "/signature/java/modify/pptx/"
          description: "Редагуйте різноманітні підписи в документі"
          
        # operation loop 11
        - name: "Видалити підписи"
          operation: "delete"
          link: "/signature/java/delete/pptx/"
          description: "Видаляйте широкий спектр раніше застосованих підписів"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Генеруйте QR-коди для додаткових форматів файлів"
    exclude: "PPTX"
    description: "Покращіть усі популярні формати файлів створеними QR-кодами, використовуючи API Java. Додавайте дані 2D штрих-коду для легкого сканування та обробки."
    items: 
          
        # format loop 1
        - name: "QR-Код для PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Адріс фільмування документів Adobe"
          
        # format loop 2
        - name: "QR-Код для DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Код для JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "Зображення JPEG"
          
        # format loop 4
        - name: "QR-Код для PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Код для XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---