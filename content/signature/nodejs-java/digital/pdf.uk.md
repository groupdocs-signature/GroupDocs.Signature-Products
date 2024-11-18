



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:59
draft: false
lang: uk
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Додавання цифрових електронних підписів до файлів PDF з JavaScript"
head_description: "Поставте цифровий підпис на файл PDF за допомогою JavaScript всього за кілька рядків коду. Використовуйте GroupDocs.Signature for Node.js via Java для підписання численних форматів файлів."

############################# Header ############################
title: "Захистіть PDF за допомогою цифрових сертифікатів" 
description: "Забезпечте безпеку ваших бізнес-документів, впроваджуючи цифрові сертифікати за допомогою розширених можливостей GroupDocs.Signature for Node.js via Java. Ми пропонуємо гнучкі варіанти для захисту та автентифікації ваших документів."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити безкоштовно"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Про GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) є комплексним рішенням для підписання, що призначене для задоволення різноманітних потреб обробки документів. Воно дозволяє вам додавати текст, зображення, цифрові сертифікати та штампи у понад 60 різних форматів файлів, включаючи PDF, MS Office, зображення та ZIP файли. Крім того, підписані документи можна легко шукати, перевіряти, редагувати або видаляти за потреби.

############################# Steps ############################
steps:
    enable: true
    title: "Інструкції для захисту PDF за допомогою цифрових сертифікатів у JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) дозволяє розробникам Node.js via Java захищати документи PDF від змін, використовуючи цифрові підписи. Покращте свої бізнес-додатки комплексними функціями захисту даних.
      
      1. Передайте документ PDF до конструктора класу Signature.
      2. Застосуйте цифровий сертифікат та відповідний пароль для забезпечення документа.
      3. За бажанням, додайте візуальне представлення цифрового підпису на сторінках документа.
      4. Підпишіть документ, щоб запобігти будь-яким майбутнім змінам.
   
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

        // Використовуйте Signature для застосування цифрового підпису до документа.
        const signature = new signatureLib.Signature('input.pdf');

        // Надайте необхідний цифровий сертифікат і пароль.
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Налаштуйте візуальні налаштування підпису за потреби.
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // Зашифруйте документ, використовуючи цифровий сертифікат.
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Оптимізуйте або захистіть вміст документа за допомогою підписів"
  description: "GroupDocs.Signature for Node.js via Java створено для підписання всіх основних форматів файлів, пропонуючи вам можливість додавати, коригувати, перевіряти або видаляти різні типи підписів."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Ключові можливості GroupDocs.Signature"
  features:
    # feature loop
    - title: "Додавайте підписи до своїх документів"
      content: "Легко розміщуйте текстові, зображеневі, штрих-кодові, QR-кодові або штамповані підписи на будь-якій сторінці підтримуваних документів. Ви також можете вставити або редагувати приховані метадані, такі як EXIF у зображеннях. Захищайте зміст вашого документа від несанкціонованих змін за допомогою цифрових сертифікатів."

    # feature loop
    - title: "Знаходьте та перевіряйте підписи"
      content: "Після підписання ваш документ може проходити кілька перевірок. Підтверджуйте цілісність підписаного вмісту або проведіть детальний пошук, щоб перерахувати всі існуючі підписи."

    # feature loop
    - title: "Редагуйте наявні підписи"
      content: "Більшість типів підписів дозволяють редагувати після створення. Ви можете легко змінювати текст, пересувати елементи, коригувати кольори, змінювати розмір і вносити інші необхідні зміни."

    # feature loop
    - title: "Видаляйте непотрібні підписи"
      content: "Наше рішення забезпечує повну функціональність CRUD для підписів. У разі потреби ви можете видаляти різні типи підписів, включаючи цифрові сертифікати, з ваших документів."
      
  code_samples:
    # code sample loop
    - title: "Захист документів цифровими підписами"
      content: |
        Дізнайтеся, як заблокувати документ від змін за допомогою цифрових підписів.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Надайте документ, який потрібно підписати.
        const signature = new signatureLib.Signature('input.pdf');

        // Використовуйте відповідний цифровий сертифікат і його пароль.
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Додайте будь-яку додаткову текстову інформацію.
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // Додайте візуальні елементи, такі як зображення для представлення підпису.
        options.setImageFilePath('image.png');
        options.setAllPages(true);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        const padding = new signatureLib.Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        
        // Збережіть цифрово захищений документ у зазначеному місці.
        const result = signature.sign('output.pdf', options);
        ```
        {{< /landing/code >}}


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
    title: "Ознайомтеся з нашими основними функціями"
    exclude: "digital"
    description: "Ми з гордістю підтримуємо широкий спектр варіантів підпису та функціональностей."
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
    title: "Підписуйте документи в різних форматах"
    exclude: "PDF"
    description: "API Node.js via Java підтримує понад 60 форматів, дозволяючи вам застосовувати різноманітні підписи на будь-якій сторінці, забезпечувати безпеку вмісту з допомогою цифрових сертифікатів та ефективно керувати підписами у документі."
    items: 
          
        # format loop 1
        - name: "Захистити PDF"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Адріс фільмування документів Adobe"
          
        # format loop 2
        - name: "Захистити DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Захистити PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Захистити XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---