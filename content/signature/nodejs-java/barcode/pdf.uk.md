



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:07
draft: false
lang: uk
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Генерація штрих-коду для PDF за допомогою JavaScript додатків"
head_description: "Швидке генерування та вбудовування підпису штрих-коду в документ PDF за допомогою JavaScript лише за кілька рядків коду. GroupDocs.Signature підтримує підписування в різних форматах файлів."

############################# Header ############################
title: "Генеруйте та додавайте штрих-коди в PDF" 
description: "Використовуйте GroupDocs.Signature for Node.js via Java для додавання штрих-кодів у ваші бізнес-документи, точно розміщуючи їх у потрібних місцях. Наше рішення пропонує широкий вибір можливостей налаштування для адаптації підписів штрих-кодів до ваших потреб."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити зараз – безкоштовно!"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Ознайомлення з GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) – це потужний інструмент підписання документів, який підтримує різноманітні типи підписів, такі як текст, зображення, штрих-коди, цифрові сертифікати та штампи. За допомогою підтримки більше 60 форматів файлів, таких як PDF, файли MS Office, зображення та ZIP-архіви, ви зможете здійснювати всебічне управління документами. Підписи в документах можуть бути пошуковані, перевірені, змінені чи видалені за потребою.

############################# Steps ############################
steps:
    enable: true
    title: "Як згенерувати та вбудувати штрих-коди в файл PDF"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) дозволяє генерувати та розміщувати штрих-коди в різних популярних форматах на сторінках PDF. Підтримуючи понад 60 типів штрих-кодів, додатки Node.js via Java можуть бути легко розширені можливостями підпису штрих-кодів за допомогою інтеграції нашої бібліотеки.
      
      1. Надайте файл або потік PDF для обробки.
      2. Передайте текст штрих-коду до екземпляра BarcodeSignOptions.
      3. Налаштуйте параметри штрих-коду, такі як положення, розмір тощо.
      4. Збережіть документ з новим доданим штрих-кодом.
   
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

        // Інстанціюйте об'єкт Signature з шляхом до документа
        const signature = new signatureLib.Signature('input.pdf');

        // Використовуйте BarcodeSignOptions для вбудовування штрих-коду в документ
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // Налаштуйте тип штрих-коду та додаткові параметри
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // Збережіть підписаний документ
        signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Розширте та захистіть ваші документи за допомогою розширених можливостей підпису"
  description: "Бібліотека GroupDocs.Signature for Node.js via Java розроблена для спрощення підписання та подальшого управління популярними форматами документів. Швидко та ефективно додавайте, змінюйте, перевіряйте чи видаляйте широкий спектр підписів."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Ключові функціональні можливості GroupDocs.Signature"
  features:
    # feature loop
    - title: "Динамічне підписання документів"
      content: "Підписуйте будь-яку сторінку вашого документа за допомогою різноманітних типів підписів, включаючи текст, зображення, штрих-коди, QR-коди та штампи. Додатково ви можете вбудовувати приховану метадані, такі як EXIF-дані в зображеннях, або захистити документ від несанкціонованих змін за допомогою цифрових сертифікатів."

    # feature loop
    - title: "Надійна перевірка підпису та пошук"
      content: "Наше рішення надає широкий набір інструментів для управління підписаними документами. Перевіряйте автентичність підписів, щоб забезпечити цілісність документа, та використовуйте функцію пошуку для відображення всіх підписів, вбудованих у документ."

    # feature loop
    - title: "Зручне редагування підписів"
      content: "Більшість підписів, доданих раніше, можна легко змінити. Оновіть текст, змініть положення чи вигляд підпису відповідно до ваших потреб."

    # feature loop
    - title: "Спрощене видалення підписів"
      content: "З комплексною підтримкою операцій CRUD наш інструмент дозволяє ефективно видаляти підписи з ваших документів, забезпечуючи наявність лише найбільш актуальних підписів."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Як застосувати підпис штрих-коду"
      content: |
        Цей приклад ілюструє, як вбудувати індивідуальний штрих-код на сторінки документа PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Надайте документ, який потрібно підписати
          const signature = new signatureLib.Signature('input.pdf');

          // Використовуйте BarcodeSignOptions для вбудовування штрих-коду в документ
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // Налаштуйте тип штрих-коду та додаткові параметри
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // Визначте відстань між штрих-кодом та краєм сторінки
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Оберіть колір штрихів
          signOptions.setForeColor(signatureLib.Color.RED);

          // Вкажіть стиль шрифту для повідомлення
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // Вкажіть позицію повідомлення
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // Підпишіть і збережіть документ
          signature.sign('output.pdf', signOptions);

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
            link: "/examples/signature/formats/signature_barcode.pdf"
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
    title: "Зануртесь у наші основні функції"
    exclude: "barcode"
    description: "Відчуйте широкий спектр типів підписів та інструментів, які ми надаємо."
    items: 
          
        # operation loop 1
        - name: "Електронні підписи"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Додавайте різні типи підписів до підтримуваних форматів файлів"

        # operation loop 2
        - name: "Додати текст до документів"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Збагачуйте вміст документів настроювальними текстовими підписами"

        # operation loop 3
        - name: "Зображення підписів"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Розміщуйте будь-яке зображення у будь-якому місці документа"

        # operation loop 4
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Створюйте та вставляйте різні штрих-коди у підтримувані документи"

        # operation loop 5
        - name: "Генерувати QR-коди"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Генеруйте QR-коди для підписання документів"
          
        # operation loop 6
        - name: "Цифрові сертифікати"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Захистіть бізнес і підписуйте документи за допомогою цифрових сертифікатів"

        # operation loop 7
        - name: "Печатки підписів"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Використовуйте Конструктор печаток для створення індивідуальних круглих або квадратних печаток"
          
        # operation loop 8
        - name: "Шукати підписи"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Знаходьте будь-які попередньо додані підписи в документі"
          
        # operation loop 9
        - name: "Перевірка підписів"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Перевіряйте автентичність підписів після їхнього застосування"
          
        # operation loop 10
        - name: "Змінювати підписи"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Редагуйте різноманітні підписи в документі"
          
        # operation loop 11
        - name: "Видалити підписи"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Видаляйте широкий спектр раніше застосованих підписів"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Підписуйте в різних форматах документів"
    exclude: "PDF"
    description: "API Node.js via Java дає змогу підписувати понад 60 різних форматів. Незалежно від того, чи потрібно додати підписи до конкретних сторінок, чи точно їх розташувати, наш інструмент робить підписання різних типів підписів зручним."
    items: 
          
        # format loop 1
        - name: "Додати штрих-код до PDF"
          format: "PDF"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Адріс фільмування документів Adobe"
          
        # format loop 2
        - name: "Додати штрих-код до DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Додати штрих-код до JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "Зображення JPEG"
          
        # format loop 4
        - name: "Додати штрих-код до PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 5
        - name: "Додати штрих-код до XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---