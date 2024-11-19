



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:22
draft: false
lang: uk
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Генерація QR-кодів у файлах XLSX з допомогою JavaScript"
head_description: "Використовуйте API GroupDocs.Signature для створення та інтеграції 2D-штрих-кодів у файли XLSX. Легко розміщуйте QR-коди на будь-якій сторінці документа."

############################# Header ############################
title: "Створення QR-кодів для XLSX" 
description: "Створюйте та вбудовуйте 2D-штрих-коди з налаштовуваним вмістом, включаючи текст і числові дані, у різні типи документів, такі як PDF, Word, Excel та зображення з GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Спробуйте безкоштовно"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Досліджуйте можливості GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) пропонує розширені інструменти для покращення документів, що дозволяє генерувати та вбудовувати декілька типів підписів, включаючи QR-коди, у популярні формати файлів. Підписуйте та захищайте PDF-документи, документи Word, електронні таблиці Excel, презентації PowerPoint та зображення з допомогою підписів тексту, зображень, штрих-кодів, QR-кодів, метаданих, цифрових та штампованих підписів.

############################# Steps ############################
steps:
    enable: true
    title: "Довідник зі створення та вбудовування QR-коду в будь-яке місце в XLSX"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) дозволяє створювати QR-коди в різних широко використовуваних форматах та їх інтеграцію на сторінки XLSX. Підтримуючи понад 10 різних типів QR-кодів, наше рішення можна безперешкодно впроваджувати у програми Node.js via Java, збагачуючи їх можливостями підписування QR-кодів.
      
      1. Надайте файл XLSX або потік для підписання QR-коду.
      2. Введіть бажаний текст у екземпляр QrCodeSignOptions.
      3. Відкоригуйте візуальні параметри, такі як колір, розташування, розмір тощо.
      4. Збережіть документ, що містить QR-код.
   
    code:
      platform: "nodejs-java"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Приклад підписів"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "натисніть для копіювання"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Створіть екземпляр Signature та передайте шлях до документа
        const signature = new signatureLib.Signature('input.xlsx');

        // Використовуйте QrCodeSignOptions для вставки QR-коду у документ
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // Визначте тип підпису та його розташування на сторінці
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // Збережіть документ з новоствореним QR-кодом
        signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Комплексна інтеграція підписів та QR-кодів"
  description: "З API GroupDocs.Signature for Node.js via Java ви можете керувати повним спектром підписів. Генеруйте, налаштовуйте, перевіряйте, шукайте та видаляйте підписи без зусиль у різних типах документів, що забезпечує неперевершену гнучкість для ваших робочих процесів."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Функції підписів та QR-кодів"
  features:
    # feature loop
    - title: "Підписування документів у декількох форматах"
      content: "Додавайте кілька типів підписів, включаючи підписи тексту, зображень, штрих-кодів, QR-кодів та штампів, до будь-якого підтримуваного формату документа. Розміщуйте їх на будь-якій сторінці та керуйте метаданими документа. Забезпечте безпеку документа за допомогою цифрових сертифікатів для запобігання несанкціонованим змінам."

    # feature loop
    - title: "Ефективна перевірка підписів"
      content: "Перевіряйте всі підписи у документі, аби забезпечити їх відповідність встановленим стандартам. Легко знаходьте та переглядайте підписи за допомогою вбудованої функції пошуку."

    # feature loop
    - title: "Гнучке редагування підписів"
      content: "Оновлюйте або модифікуйте існуючі підписи, коригуючи такі аспекти, як вміст, розташування, розмір та колір, відповідно до потреб вашого документа після початкового підписування."

    # feature loop
    - title: "Легке видалення підписів"
      content: "Видаляйте будь-які небажані або застарілі підписи, включаючи цифрові сертифікати, без труднощів. Повний контроль над управлінням підписами забезпечує чистий та добре організований документ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Налаштування згенерованого QR-коду"
      content: |
        Цей приклад деталізує процес додавання кастомізованого QR-коду на сторінку XLSX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Отримайте документ, що підписується, та передайте його у Signature
          const signature = new signatureLib.Signature('input.xlsx');

          // Налаштуйте параметри QR-коду з необхідним текстом
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // Визначте позицію QR-коду на сторінці
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Вкажіть відступ підпису
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Виберіть колір QR-коду
          signOptions.setForeColor(signatureLib.Color.RED);

          // Визначте параметри шрифту для супровідного повідомлення
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Налаштуйте фон та кисть для QR-коду
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Вбудуйте QR-код у документ
          signature.sign('output.xlsx', signOptions);
          ```
        platform: "nodejs-java"
        copy_title: "Копіювати"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "натисніть для копіювання"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.xlsx"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Спробуйте можливості GroupDocs.Signature безкоштовно або запросіть ліцензію"
  items:
    #  loop
    - title: "Завантаження NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Зрозумійте наші основні можливості"
    exclude: "qrcode"
    description: "Ми пропонуємо широкий вибір форматів підписів та операцій, адаптованих до ваших потреб."
    items: 
          
        # operation loop 1
        - name: "Електронні підписи"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Додавайте різні типи підписів до підтримуваних форматів файлів"

        # operation loop 2
        - name: "Додати текст до документів"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Збагачуйте вміст документів настроювальними текстовими підписами"

        # operation loop 3
        - name: "Зображення підписів"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Розміщуйте будь-яке зображення у будь-якому місці документа"

        # operation loop 4
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Створюйте та вставляйте різні штрих-коди у підтримувані документи"

        # operation loop 5
        - name: "Генерувати QR-коди"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Генеруйте QR-коди для підписання документів"
          
        # operation loop 6
        - name: "Цифрові сертифікати"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Захистіть бізнес і підписуйте документи за допомогою цифрових сертифікатів"

        # operation loop 7
        - name: "Печатки підписів"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Використовуйте Конструктор печаток для створення індивідуальних круглих або квадратних печаток"
          
        # operation loop 8
        - name: "Шукати підписи"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Знаходьте будь-які попередньо додані підписи в документі"
          
        # operation loop 9
        - name: "Перевірка підписів"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Перевіряйте автентичність підписів після їхнього застосування"
          
        # operation loop 10
        - name: "Змінювати підписи"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "Редагуйте різноманітні підписи в документі"
          
        # operation loop 11
        - name: "Видалити підписи"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Видаляйте широкий спектр раніше застосованих підписів"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Інтеграція QR-кодів з різними формами файлів"
    exclude: "XLSX"
    description: "Скористайтеся API Node.js via Java для генерації QR-кодів та вбудовуйте їх у різноманітні широко використовувані формати файлів. Оточте важливі дані цими штрих-кодами для безперешкодної інтеграції та подальшого отримання."
    items: 
          
        # format loop 1
        - name: "QR-Код для PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Адріс фільмування документів Adobe"
          
        # format loop 2
        - name: "QR-Код для DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Код для JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Зображення JPEG"
          
        # format loop 4
        - name: "QR-Код для PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Код для XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---