



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:59
draft: false
lang: ru
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Добавление цифровых электронных подписей в файл PDF с помощью JavaScript"
head_description: "Установите цифровую подпись на файл PDF с помощью JavaScript всего за несколько строк кода. Используйте GroupDocs.Signature for Node.js via Java для подписи множества форматов файлов."

############################# Header ############################
title: "Защитите PDF с помощью цифровых сертификатов" 
description: "Обеспечьте безопасность ваших бизнес-документов, встраивая цифровые сертификаты, используя расширенные возможности GroupDocs.Signature for Node.js via Java. Мы предлагаем гибкие варианты для защиты и аутентификации ваших документов."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать бесплатно"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "О GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) - это комплексное решение для подписания, разработанное для удовлетворения различных потребностей обработки документов. Оно позволяет вам включать текст, изображения, цифровые сертификаты и печати в более чем 60 различных форматов файлов, включая PDF, MS Office, изображения и ZIP файлы. Кроме того, подписанные документы могут быть легко найдены, проверены, изменены или удалены при необходимости.

############################# Steps ############################
steps:
    enable: true
    title: "Руководство по защите PDF с помощью цифровых сертификатов на JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) позволяет разработчикам Node.js via Java защищать документы PDF от изменений с помощью цифровых подписей. Улучшите свои бизнес-приложения с помощью комплексных функций безопасности данных.
      
      1. Передайте документ PDF в конструктор класса Signature.
      2. Примените цифровой сертификат и соответствующий пароль для защиты документа.
      3. При желании добавьте визуальное представление цифровой подписи на страницы документа.
      4. Подпишите документ, чтобы предотвратить любые будущие изменения.
   
    code:
      platform: "nodejs-java"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Примеры подписей"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "щелкните, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Используйте Signature для применения цифровой подписи к документу
        const signature = new signatureLib.Signature('input.pdf');

        // Предоставьте необходимый цифровой сертификат и пароль
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // При необходимости настройте параметры визуальной подписи
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // Зашифруйте документ, используя цифровой сертификат
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Оптимизация или защита содержания документов с помощью подписей"
  description: "GroupDocs.Signature for Node.js via Java разработан для подписи всех основных форматов файлов, предоставляя вам возможность добавлять, корректировать, проверять или удалять различные типы подписей."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Ключевые функции GroupDocs.Signature"
  features:
    # feature loop
    - title: "Добавьте подписи к вашим документам"
      content: "Легко размещайте текстовые, изображенческие, штрих-кодовые, QR-кодовые или печатные подписи на любой странице поддерживаемых документов. Также вы можете вставлять или редактировать скрытые метаданные, такие как EXIF в изображениях. Защитите содержание вашего документа от несанкционированных изменений с помощью цифровых сертификатов."

    # feature loop
    - title: "Найдите и проверьте подписи"
      content: "После подписания ваш документ может подвергаться множественным проверкам. Подтвердите целостность подписанного содержимого или проведите детальный поиск для перечисления всех существующих подписей."

    # feature loop
    - title: "Измените существующие подписи"
      content: "Большинство типов подписей допускают редактирование после создания. Вы можете легко изменить текст, изменить расположение элементов, скорректировать цвета, изменить размер и внести другие необходимые изменения."

    # feature loop
    - title: "Устраните ненужные подписи"
      content: "Наше решение позволяет выполнять полные операции CRUD для подписей. При необходимости вы можете удалить различные типы подписей, включая цифровые сертификаты, из вашего документа."
      
  code_samples:
    # code sample loop
    - title: "Защитите документы с помощью цифровых подписей"
      content: |
        Узнайте, как заблокировать документ от изменений с использованием цифровых подписей.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // Предоставьте документ, который требует подписи
        const signature = new signatureLib.Signature('input.pdf');

        // Используйте соответствующий цифровой сертификат и его пароль
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Включите любую дополнительную текстовую информацию
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // Добавьте визуальные элементы, такие как изображения для представления подписи
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
        
        // Сохраните цифровым образом защищенный документ в указанном месте
        const result = signature.sign('output.pdf', options);
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Используйте функции GroupDocs.Signature бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачивание NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Познакомьтесь с нашими основными функциями"
    exclude: "digital"
    description: "С гордостью поддерживаем комплексный набор опций и функциональности для подписей"
    items: 
          
        # operation loop 1
        - name: "Электронные подписи"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Добавляйте различные типы подписей к поддерживаемым форматам файлов"

        # operation loop 2
        - name: "Добавить текст в документы"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Усовершенствуйте содержимое документа настраиваемыми текстовыми подписями"

        # operation loop 3
        - name: "Подписи изображений"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Размещайте любое изображение в любом месте документа"

        # operation loop 4
        - name: "Генерация штрихкодов"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Создавайте и вставляйте различные штрихкоды в поддерживаемые документы"

        # operation loop 5
        - name: "Генерация QR-кодов"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Генерируйте QR-коды для подписания документов"
          
        # operation loop 6
        - name: "Цифровые сертификаты"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Защищайте документы и подписывайте их с помощью цифровых сертификатов"

        # operation loop 7
        - name: "Штамповые подписи"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Используйте Конструктор штампов для создания настраиваемых круглых или квадратных штампов"
          
        # operation loop 8
        - name: "Поиск подписей"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Находите любые ранее добавленные подписи в документе"
          
        # operation loop 9
        - name: "Проверка подписи"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Подтверждайте подлинность подписей после их применения"
          
        # operation loop 10
        - name: "Изменение подписей"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Редактируйте разнообразные подписи в документе"
          
        # operation loop 11
        - name: "Удаление подписей"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Удаляйте широкий спектр ранее примененных подписей"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Подписывайте документы в различных форматах"
    exclude: "PDF"
    description: "API Node.js via Java поддерживает более 60 форматов, позволяя вам применять различные подписи на любой странице, обеспечивать безопасность содержания с помощью цифровых сертификатов и эффективно управлять подписями внутри документа."
    items: 
          
        # format loop 1
        - name: "Защитить PDF"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Формат документа, независимый от аппаратных средств Adobe"
          
        # format loop 2
        - name: "Защитить DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Защитить PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Защитить XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---