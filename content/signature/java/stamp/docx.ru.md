



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:04
draft: false
lang: ru
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Добавьте штампы к DOCX с использованием Java"
head_description: "Используйте GroupDocs.Signature и Java для создания пользовательских штампов и размещения их на любой странице документов DOCX."

############################# Header ############################
title: "Добавьте пользовательские штампы к DOCX" 
description: "Создавайте и применяйте круглые или квадратные штампы к любой части ваших документов с помощью GroupDocs.Signature for Java. Наше решение предоставляет обширные возможности настройки для удовлетворения всех ваших бизнес-потребностей."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать бесплатно"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "О GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Узнать больше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) — это мощный инструмент, который позволяет добавлять различные штамповые подписи к документам. Он поддерживает более 60 различных форматов файлов, включая PDF, Word, Excel, изображения и ZIP-файлы. Вы можете применять текстовые, изображенческие, штриховые коды, метаданные, цифровые сертификаты и штамповые подписи. Кроме добавления подписей, вы можете их искать, проверять, изменять и удалять.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги по добавлению штампов к DOCX с помощью Java"
    content: |
      [GroupDocs.Signature](/signature/java/) предоставляет конструктор штампов, который может быть весьма полезен для приложений Java. Используйте его для создания хорошо настроенных штампов для страниц ваших документов.
      
      1. Предоставьте документ DOCX, к которому нужно добавить штамп.
      2. Используйте StampSignOptions, чтобы настроить все необходимые параметры.
      3. Добавьте необходимое количество строк.
      4. Примените штамп и сохраните документ.
   
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
        // Используйте путь к документу с объектом Signature
        Signature signature = new Signature("input.docx");

        // Создайте экземпляр StampSignOptions с требуемым текстом подписи
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Добавьте одну или несколько строк штампа
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Сохраните документ со штампом
        SignResult result = signature.sign("output.docx", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "Защитите содержимое вашего документа с помощью подписей"
  description: "Библиотека GroupDocs.Signature for Java предназначена для подписания и управления подписями в популярных форматах файлов. Легко добавляйте, изменяйте, проверяйте или удаляйте штампы и другие типы подписей."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Штамповые подписи с GroupDocs.Signature"
  features:
    # feature loop
    - title: "Подписывайте ваши документы"
      content: "Применяйте настраиваемые подписи к любой части вашего документа. Выбирайте из различных типов подписей, включая текст, изображения, штриховые коды, QR-коды и штампы. Дополнительно можно добавлять или изменять скрытые метаданные для повышения безопасности документа."

    # feature loop
    - title: "Ищите и проверяйте подписи"
      content: "После подписания документа используйте наши инструменты проверки, чтобы убедиться, что содержимое подписи действительно. Искать и получать список всех подписей для дальнейшей обработки."

    # feature loop
    - title: "Обновляйте подписи по мере необходимости"
      content: "Изменяйте разнообразные подписи, примененные к документу. Обновляйте такие свойства, как размер, цвет, позиция, содержание и многое другое."

    # feature loop
    - title: "Удаляйте подписи"
      content: "Нужно удалить подписи из документа? Наш API полностью поддерживает удаление подписей, позволяя эффективно управлять вашими документами."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Добавьте пользовательские штампы к документам с помощью специальных подписей"
      content: |
        Узнайте, как сгенерировать и добавить пользовательские штампы с важной текстовой информацией к вашим документам.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Предоставьте документ для штамповки
          Signature signature = new Signature("input.docx");

          // Создайте объект параметров штампа
          StampSignOptions options = new StampSignOptions();

          // Установите размер и позицию на странице
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // Добавьте одну или несколько внешних круглых линий с текстом
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Добавьте одну или несколько внутренних квадратных линий
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // Сохраните документ со штампом
          SignResult result = signature.sign("output.docx", options);
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
            link: "/examples/signature/formats/signature_stamp.docx"
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
    title: "Изучите наши основные функции"
    exclude: "stamp"
    description: "Используйте широкий спектр опций для добавления, управления и удаления подписей."
    items: 
          
        # operation loop 1
        - name: "Электронные подписи"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "Добавляйте различные типы подписей к поддерживаемым форматам файлов"

        # operation loop 2
        - name: "Добавить текст в документы"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "Усовершенствуйте содержимое документа настраиваемыми текстовыми подписями"

        # operation loop 3
        - name: "Подписи изображений"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "Размещайте любое изображение в любом месте документа"

        # operation loop 4
        - name: "Генерация штрихкодов"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "Создавайте и вставляйте различные штрихкоды в поддерживаемые документы"

        # operation loop 5
        - name: "Генерация QR-кодов"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "Генерируйте QR-коды для подписания документов"
          
        # operation loop 6
        - name: "Цифровые сертификаты"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "Защищайте документы и подписывайте их с помощью цифровых сертификатов"

        # operation loop 7
        - name: "Штамповые подписи"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "Используйте Конструктор штампов для создания настраиваемых круглых или квадратных штампов"
          
        # operation loop 8
        - name: "Поиск подписей"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "Находите любые ранее добавленные подписи в документе"
          
        # operation loop 9
        - name: "Проверка подписи"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "Подтверждайте подлинность подписей после их применения"
          
        # operation loop 10
        - name: "Изменение подписей"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "Редактируйте разнообразные подписи в документе"
          
        # operation loop 11
        - name: "Удаление подписей"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "Удаляйте широкий спектр ранее примененных подписей"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Добавьте штампы для нескольких форматов файлов"
    exclude: "DOCX"
    description: "API GroupDocs.Signature поддерживает добавление штампов в более чем 60 форматах. Размещайте штампы на любой странице или области для улучшения управления документами и настройки."
    items: 
          
        # format loop 1
        - name: "Штамповать PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "Формат документа, независимый от аппаратных средств Adobe"
          
        # format loop 2
        - name: "Штамповать DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Штамповать JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "Изображение JPEG"
          
        # format loop 4
        - name: "Штамповать PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 5
        - name: "Штамповать XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---