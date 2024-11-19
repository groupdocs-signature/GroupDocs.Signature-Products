



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:32
draft: false
lang: ru
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Поиск цифровой подписи в PDF с помощью Java"
head_description: "Используйте API GroupDocs.Signature for Java для поиска подписей в файлах PDF. Найдите подписи в PDF, Word, Excel, Презентациях и Изображениях."

############################# Header ############################
title: "Поиск цифровых подписей в PDF" 
description: "Получите полный список электронных подписей, встроенных в файлы PDF, Word, Excel, Презентации или Изображения, используя GroupDocs.Signature for Java."
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
       [GroupDocs.Signature for Java](/signature/java/) предлагает мощные возможности для подписания документов. Он поддерживает добавление текста, изображений, штрих-кодов, цифровых сертификатов и штампов в файлы более чем 60 форматов, включая PDF, документы MS Office, Изображения, ZIP файлы и другие распространенные бизнес-форматы. Кроме того, вы можете искать, проверять, изменять или удалять подписи в любое время.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги для поиска подписей PDF с помощью Java"
    content: |
      [GroupDocs.Signature](/signature/java/) предоставляет мощный движок для поиска цифровых подписей в файлах PDF. Разработчики Java могут улучшить свои приложения с помощью нашего решения.
      
      1. Укажите путь к файлу PDF для поиска подписей.
      2. Используйте SearchOptions для уточнения результатов поиска.
      3. Выполните метод поиска, чтобы получить результаты.
      4. Анализируйте список найденных подписей.
   
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

        // Создайте экземпляр Signature с путем к документу
        final Signature signature = new Signature("input.pdf");

        // Создайте экземпляр TextSearchOptions для охвата всех страниц
        TextSearchOptions options = new TextSearchOptions();
        options.setAllPages(true);

        // Ищите текстовые подписи в документе
        List<TextSignature> signatures = signature.search(TextSignature.class, options);
        System.out.print("\nSource document contains following text signature(s).");

        // Перечислите найденные подписи для дальнейшего анализа
        for (TextSignature textSignature : signatures) {
            System.out.print("Found Text signature at page " + textSignature.getPageNumber() 
                + " with type [" + textSignature.getSignatureImplementation() + "] and 
                text '" + textSignature.getText() + "'.");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Комплексное решение для подписания документов"
  description: "Мы рады представить наше решение для подписания документов, совместимое со всеми основными форматами документов. Добавляйте широкий спектр подписей для улучшения ваших документов или защиты их содержимого."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Поиск подписи"
  features:
    # feature loop
    - title: "Подписывать бизнес-документы"
      content: "Вставляйте цифровые подписи в любое место на любой странице документа. Используйте различные типы подписей, такие как текст, изображения, штрих-коды, метаданные, штампы или цифровые сертификаты."

    # feature loop
    - title: "Управлять подписями"
      content: "После подписания документы могут требовать дальнейшей обработки. Ищите все доступные подписи и обновляйте или удаляйте их по мере необходимости."

    # feature loop
    - title: "Защита содержимого документа"
      content: "Управляйте скрытыми метаданными, встроенными в документ. Добавляйте новые метаданные или удаляйте существующие записи. Используйте корпоративные цифровые сертификаты для защиты содержимого документа от несанкционированных изменений."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Поиск изображений-подписей"
      content: |
        Этот пример демонстрирует, как найти изображение-подпись в конкретном документе.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Передайте исходный документ в качестве параметра конструктора
          final Signature signature = new Signature("input.pdf");

          // Ищите любые подписи с текстовым типом
          List<ImageSignature> signatures = signature.search(ImageSignature.class, SignatureType.Image);
          System.out.print("\nSource document contains following image signature(s).");

          // Отобразите результаты с параметрами найденных подписей
          for (ImageSignature imageSignature : signatures)
          {
              System.out.print("Image signature found at page "+imageSignature.getPageNumber()+
                    " with size "+imageSignature.getSize()+". Created "+imageSignature.getCreatedOn()+
                    ", modified "+imageSignature.getModifiedOn());
          }
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
    title: "Поддерживаемые операции"
    exclude: "search"
    description: "Наш продукт предлагает гибкий API для подписания документов и управления подписями после подписания."
    items: 
          
        # operation loop 1
        - name: "Электронные подписи"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "Добавляйте различные типы подписей к поддерживаемым форматам файлов"

        # operation loop 2
        - name: "Добавить текст в документы"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "Усовершенствуйте содержимое документа настраиваемыми текстовыми подписями"

        # operation loop 3
        - name: "Подписи изображений"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "Размещайте любое изображение в любом месте документа"

        # operation loop 4
        - name: "Генерация штрихкодов"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "Создавайте и вставляйте различные штрихкоды в поддерживаемые документы"

        # operation loop 5
        - name: "Генерация QR-кодов"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "Генерируйте QR-коды для подписания документов"
          
        # operation loop 6
        - name: "Цифровые сертификаты"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Защищайте документы и подписывайте их с помощью цифровых сертификатов"

        # operation loop 7
        - name: "Штамповые подписи"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "Используйте Конструктор штампов для создания настраиваемых круглых или квадратных штампов"
          
        # operation loop 8
        - name: "Поиск подписей"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "Находите любые ранее добавленные подписи в документе"
          
        # operation loop 9
        - name: "Проверка подписи"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "Подтверждайте подлинность подписей после их применения"
          
        # operation loop 10
        - name: "Изменение подписей"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "Редактируйте разнообразные подписи в документе"
          
        # operation loop 11
        - name: "Удаление подписей"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "Удаляйте широкий спектр ранее примененных подписей"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск подписей в различных форматах файлов"
    exclude: "PDF"
    description: "API GroupDocs.Signature for Java позволяет вам получать список подписей из любого подписанного файла. Извлекайте подписи из популярных форматов файлов для дальнейшей обработки."
    items: 
          
        # format loop 1
        - name: "Поиск подписей в PDF"
          format: "PDF"
          link: "/signature/java/search/pdf/"
          description: "Формат документа, независимый от аппаратных средств Adobe"
          
        # format loop 2
        - name: "Найти подписи в DOCX"
          format: "DOCX"
          link: "/signature/java/search/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Найти подписи в PPTX"
          format: "PPTX"
          link: "/signature/java/search/pptx/"
          description: "Презентация PowerPoint Open XML"
          
        # format loop 4
        - name: "Поиск подписей в XLSX"
          format: "XLSX"
          link: "/signature/java/search/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"


          

---