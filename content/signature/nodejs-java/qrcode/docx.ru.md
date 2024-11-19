



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:21
draft: false
lang: ru
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Генерация QR-кодов в документах DOCX с помощью JavaScript"
head_description: "Используйте API GroupDocs.Signature для создания и интеграции 2D штрих-кодов в файлы DOCX. Легко размещайте QR-коды на любой странице документа."

############################# Header ############################
title: "Создание QR-кодов для DOCX" 
description: "Создавайте и встраивайте 2D штрих-коды с настраиваемым содержимым, включая текст и числовые данные, в различные типы документов, такие как PDF, Word, Excel и изображения с использованием GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Попробовать бесплатно"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Изучите возможности GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) предлагает передовые инструменты для улучшения документов, позволяя создавать и встраивать различные типы подписей, включая QR-коды, в популярные форматы файлов. Подписывайте и защищайте PDF, документы Word, таблицы Excel, презентации PowerPoint и изображения с помощью текстовых, графических, штрих-кодов, QR-кодов, метаданных, цифровых и печатных подписей.

############################# Steps ############################
steps:
    enable: true
    title: "Руководство по генерации и встраиванию QR-кода в любом месте DOCX"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) позволяет создавать QR-коды в различных широко используемых форматах и интегрировать их в страницы DOCX. Поддерживая более 10 различных типов QR-кодов, наше решение может быть seamlessly incorporated в приложения Node.js via Java, обогащая их возможностями подписания QR-кодом.
      
      1. Предоставьте файл или поток DOCX для подписания QR-кода.
      2. Введите желаемый текст в экземпляр QrCodeSignOptions.
      3. Настройте визуальные параметры, такие как цвет, позиционирование, размер и т.д.
      4. Сохраните документ с содержащим QR-код.
   
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

        // Создайте экземпляр Signature и передайте путь к документу
        const signature = new signatureLib.Signature('input.docx');

        // Используйте QrCodeSignOptions для вставки QR-кода в документ
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // Определите тип подписи и размещение на странице
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // Сохраните документ с новым QR-кодом
        signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Всеобъемлющая интеграция подписей и QR-кодов"
  description: "С помощью API GroupDocs.Signature for Node.js via Java вы можете управлять полным спектром подписей. Генерируйте, настраивайте, проверяйте, ищите и удаляйте подписи без усилий в различных типах документов, предоставляя непревзойденную гибкость для ваших рабочих процессов."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Функции подписи и QR-кода"
  features:
    # feature loop
    - title: "Подписание документов в нескольких форматах"
      content: "Добавляйте различные типы подписей, включая текстовые, графические, штрих-коды, QR-коды и печати, в любой поддерживаемый формат документа. Размещайте их на любой странице и управляйте метаданными документа. Обеспечьте безопасность документа с помощью цифровых сертификатов для предотвращения несанкционированных изменений."

    # feature loop
    - title: "Эффективная проверка подписи"
      content: "Проверяйте все подписи в документе, чтобы убедиться, что они соответствуют необходимым стандартам. Легко получайте и просматривайте подписи с помощью встроенной функции поиска."

    # feature loop
    - title: "Гибкое редактирование подписей"
      content: "Обновляйте или изменяйте существующие подписи, настраивая такие параметры, как содержание, расположение, размер и цвет, в соответствии с потребностями вашего документа после первоначальной подписи."

    # feature loop
    - title: "Простое удаление подписей"
      content: "Удаляйте любые нежелательные или устаревшие подписи, включая цифровые сертификаты, без усилий. Полный контроль над управлением подписями обеспечивает чистый и организованный документ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Настройка сгенерированного QR-кода"
      content: |
        Этот пример описывает процесс добавления настраиваемого QR-кода на страницу DOCX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Получите документ для подписи и передайте его в Signature
          const signature = new signatureLib.Signature('input.docx');

          // Настройте параметры QR-кода с необходимым текстом
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // Определите позицию QR-кода на странице
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Укажите отступ для подписи
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Выберите цвет QR-кода
          signOptions.setForeColor(signatureLib.Color.RED);

          // Определите параметры шрифта для сопровождающего сообщения
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Настройте цвет фона и кисть для QR-кода
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Вставьте QR-код в документ
          signature.sign('output.docx', signOptions);
          ```
        platform: "nodejs-java"
        copy_title: "Копировать"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "щелкните, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.docx"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


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
    title: "Понять наши основные возможности"
    exclude: "qrcode"
    description: "Мы предлагаем широкий выбор форматов подписей и операций, адаптированных к вашим потребностям."
    items: 
          
        # operation loop 1
        - name: "Электронные подписи"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Добавляйте различные типы подписей к поддерживаемым форматам файлов"

        # operation loop 2
        - name: "Добавить текст в документы"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "Усовершенствуйте содержимое документа настраиваемыми текстовыми подписями"

        # operation loop 3
        - name: "Подписи изображений"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "Размещайте любое изображение в любом месте документа"

        # operation loop 4
        - name: "Генерация штрихкодов"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Создавайте и вставляйте различные штрихкоды в поддерживаемые документы"

        # operation loop 5
        - name: "Генерация QR-кодов"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Генерируйте QR-коды для подписания документов"
          
        # operation loop 6
        - name: "Цифровые сертификаты"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Защищайте документы и подписывайте их с помощью цифровых сертификатов"

        # operation loop 7
        - name: "Штамповые подписи"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Используйте Конструктор штампов для создания настраиваемых круглых или квадратных штампов"
          
        # operation loop 8
        - name: "Поиск подписей"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "Находите любые ранее добавленные подписи в документе"
          
        # operation loop 9
        - name: "Проверка подписи"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "Подтверждайте подлинность подписей после их применения"
          
        # operation loop 10
        - name: "Изменение подписей"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "Редактируйте разнообразные подписи в документе"
          
        # operation loop 11
        - name: "Удаление подписей"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "Удаляйте широкий спектр ранее примененных подписей"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Интеграция QR-кодов с различными форматами файлов"
    exclude: "DOCX"
    description: "Используйте API Node.js via Java для генерации QR-кодов и их встраивания в широкий спектр широко используемых форматов файлов. Инкапсулируйте важные данные в этих штрих-кодах для бесшовной интеграции и дальнейшего извлечения."
    items: 
          
        # format loop 1
        - name: "QR-код для PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Формат документа, независимый от аппаратных средств Adobe"
          
        # format loop 2
        - name: "QR-код для DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-код для JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Изображение JPEG"
          
        # format loop 4
        - name: "QR-код для PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-код для XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---