



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:01
draft: false
lang: ru
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Создание QR-кода для XLSX с помощью Java"
head_description: "API GroupDocs.Signature позволяет генерировать QR-коды для файлов XLSX. Создавайте QR-коды из вашего контента и размещайте их на любом странице."

############################# Header ############################
title: "Создание QR-кодов для XLSX" 
description: "Создавайте 2D штрихкоды с текстом и числовыми данными и размещайте их на любых страницах различных документов, используя GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Бесплатная пробная версия"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Узнайте больше о GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Узнать больше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) предлагает широкий спектр возможностей для генерации и встраивания различных типов подписей во все основные форматы документов. Он поддерживает PDF, документы Word, электронные таблицы Excel, презентации PowerPoint и изображения. Улучшайте ваши документы с помощью текстовых, изображенческих, штриховых, QR-кодов, метаданных, цифровых и штамповых подписей.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги для генерации и размещения QR-кода в любом месте XLSX"
    content: |
      [GroupDocs.Signature](/signature/java/) может генерировать QR-коды во множестве популярных форматов и размещать их на страницах XLSX. Поддерживается более 10 типов QR-кодов, которые можно быстро интегрировать в приложения Java. Используйте наш продукт для подписания документов с генерируемыми QR-кодами.
      
      1. Получите файл или поток XLSX, который необходимо подписать с QR-кодом.
      2. Предоставьте текст для QrCodeSignOptions.
      3. Настройте визуальные параметры, такие как цвет, положение, размер и т.д.
      4. Сохраните файл с QR-кодом.
   
    code:
      platform: "java"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Примеры подписей"
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
        copy_tip: "щелкните, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // Передайте документ в новый экземпляр Signature
        Signature signature = new Signature("input.xlsx");

        // Используйте QrCodeSignOptions, чтобы добавить QR-код в документ
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // Укажите тип и позицию подписи на странице
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // Сохраните файл с добавленным QR-кодом
        signature.sign("output.xlsx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Добавление подписей к вашим документам"
  description: "API GroupDocs.Signature for Java поддерживает подпись всех популярных форматов файлов. Генерируйте, изменяйте, ищите, проверяйте и удаляйте различные типы подписей."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Ключевые возможности GroupDocs.Signature"
  features:
    # feature loop
    - title: "Подписание документов"
      content: "GroupDocs.Signature поддерживает подпись с помощью текстовых, изображенческих, штриховых, QR-кодов и штамповых подписей. Размещайте их на любой странице любого поддерживаемого формата документа. Управляйте метаданными документов с помощью подписей метаданных и защищайте содержимое от несанкционированных изменений, используя цифровые сертификаты."

    # feature loop
    - title: "Поиск и проверка"
      content: "Убедитесь, что все подписи в документе действительны с помощью процедуры проверки. Получайте полный список подписей в документе с помощью встроенной функции поиска."

    # feature loop
    - title: "Изменение подписей"
      content: "Изменяйте свойства подписей после их создания. Корректируйте содержимое, позицию, цвет, размер и другие атрибуты по мере необходимости."

    # feature loop
    - title: "Удаление подписей"
      content: "Удаляйте ненужные подписи без труда. Различные типы подписей, включая цифровые сертификаты, могут быть удалены из документов программным способом."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Как настроить сгенерированный QR-код"
      content: |
        Используйте этот пример, чтобы узнать, как разместить новый QR-код на странице XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Получите документ, который нужно подписать, и передайте его в Signature
          Signature signature = new Signature("input.xlsx");

          // Используйте параметры QR-кода, чтобы предоставить текст с необходимой информацией
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // Установите относительное положение QR-кода на странице
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // Установите отступ для подписи
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Укажите цвет QR-кода
          signOptions.setForeColor(Color.RED);

          // Определите параметры шрифта для сообщения
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Настройте цвет фона QR-кода и его границы
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Добавьте QR-код в документ
          SignResult signResult = signature.sign("output.xlsx", signOptions);
          ```
        platform: "java"
        copy_title: "Копировать"
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
          copy_tip: "щелкните, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.xlsx"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Используйте функции GroupDocs.Signature бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачивание Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Изучите наши ключевые предложения"
    exclude: "qrcode"
    description: "Мы предлагаем разнообразный выбор функций подписей и продвинутых операций."
    items: 
          
        # operation loop 1
        - name: "Электронные подписи"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "Добавляйте различные типы подписей к поддерживаемым форматам файлов"

        # operation loop 2
        - name: "Добавить текст в документы"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "Усовершенствуйте содержимое документа настраиваемыми текстовыми подписями"

        # operation loop 3
        - name: "Подписи изображений"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "Размещайте любое изображение в любом месте документа"

        # operation loop 4
        - name: "Генерация штрихкодов"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "Создавайте и вставляйте различные штрихкоды в поддерживаемые документы"

        # operation loop 5
        - name: "Генерация QR-кодов"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "Генерируйте QR-коды для подписания документов"
          
        # operation loop 6
        - name: "Цифровые сертификаты"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "Защищайте документы и подписывайте их с помощью цифровых сертификатов"

        # operation loop 7
        - name: "Штамповые подписи"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "Используйте Конструктор штампов для создания настраиваемых круглых или квадратных штампов"
          
        # operation loop 8
        - name: "Поиск подписей"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "Находите любые ранее добавленные подписи в документе"
          
        # operation loop 9
        - name: "Проверка подписи"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "Подтверждайте подлинность подписей после их применения"
          
        # operation loop 10
        - name: "Изменение подписей"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "Редактируйте разнообразные подписи в документе"
          
        # operation loop 11
        - name: "Удаление подписей"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "Удаляйте широкий спектр ранее примененных подписей"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Генерация QR-кодов для дополнительных форматов файлов"
    exclude: "XLSX"
    description: "Улучшайте все популярные форматы файлов с помощью генерируемых QR-кодов, используя API Java. Добавляйте данные 2D штрихкода для удобного сканирования и обработки."
    items: 
          
        # format loop 1
        - name: "QR-код для PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "Формат документа, независимый от аппаратных средств Adobe"
          
        # format loop 2
        - name: "QR-код для DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-код для JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "Изображение JPEG"
          
        # format loop 4
        - name: "QR-код для PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-код для XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---