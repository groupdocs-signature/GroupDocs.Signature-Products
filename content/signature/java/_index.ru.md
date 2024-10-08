---
############################# Static ############################
layout: "landing"
date: 2024-09-25T12:45:24
draft: false

lang: ru
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java" 
    # supported_platforms loop
    - title: "Python"
      tag: "python-net" 

############################# Head ############################
head_title: "Библиотека цифровых подписей Java — GroupDocs.Signature"
head_description: "Расширьте возможности Java-приложений с помощью электронных подписей с помощью GroupDocs.Signature. Подписывайте деловые документы быстро и легко."

############################# Header ############################
title: "Подписывать документы через Java API"
description: "Подписывайте цифровые документы и изображения на любой платформе, используя наши гибкие API и решения на базе приложений для программистов и конечных пользователей."
words:
  for: "для"

actions:
  main: "Бесплатная загрузка Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Signature бесплатно или запросите лицензию."

release:
  title: "Версия {0} выпущена"
  notes: "Посмотрите, что нового"
  downloads: "Загрузки"

code:
  title: "Подписание PDF-файлов на Java"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Выберите PDF-документ
    Signature signature = new Signature("sample.pdf");
    
    // Предоставить текст
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Подписать документ и сохранить в файл
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Обзор GroupDocs.Signature"
  description: "API для подписания документов и связанных с ним операций в приложениях Java"
  features:
    # feature loop
    - title: "Улучшенные деловые документы с цифровыми подписями на Java."
      content: "Быстрое и настраиваемое подписание: GroupDocs.Signature для Java предлагает широкий спектр вариантов цифровой подписи для PDF-файлов, изображений и документов Office. Вы можете использовать текст, штрих-коды, QR-коды, цифровые сертификаты, изображения или скрытые метаданные. Обработка документов происходит быстро и эффективно."

    # feature loop
    - title: "Манипулирование подписанными документами"
      content: "Расширенная обработка документов включает в себя мощные операции с подписанными документами с использованием GroupDocs.Signature для Java. Вы можете искать и проверять подписи, добавленные в деловые документы, используя различные полезные критерии. Кроме того, вы можете получить доступ к подробной информации о документе или получить изображения для предварительного просмотра его страниц."

    # feature loop
    - title: "Разнообразие вариантов вывода"
      content: "Надежные параметры подписи позволяют настраивать вывод документов, подписанных с помощью GroupDocs.Signature для Java. Вы можете точно расположить любую подпись на любой странице документа и настроить ее внешний вид различными способами. Java API поддерживает сохранение подписанных деловых документов во многих поддерживаемых форматах и ​​предоставляет возможности для их защиты с помощью паролей."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимость от платформы"
  description: "GroupDocs.Signature для Java поддерживает следующие операционные системы, платформы и менеджеры пакетов."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Поддерживаемые форматы файлов"
  description: |
    GroupDocs.Signature для Java поддерживает операции со следующими [форматами файлов](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Форматы Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Изображения и другие форматы
        * **Портативный:** PDF
        * **Изображений:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Другие форматы офисов:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Другие форматы
        * **Интернет:** HTML, MHTML
        * **Архивы:** ZIP, TAR, 7Z
        * **Сертификаты:** PFX

############################# Features ############################
features:
  enable: true
  title: "Возможности GroupDocs.Signature"
  description: "Подписание PDF-файлов, документов Office и изображений с помощью цифровых подписей"

  items:
    # feature loop
    - icon: "sign"
      title: "Добавление подписей"
      content: "Подпишите документ, используя различные поддерживаемые типы подписей, разместив цифровую подпись точно в любом месте на любой странице."

    # feature loop
    - icon: "custom"
      title: "Настройка результатов"
      content: "Настройте внешний вид подписи, настроив цвет, шрифт, рамку, поворот и другие функции для достижения желаемого результата."

    # feature loop
    - icon: "password"
      title: "Защита документов паролем"
      content: "Для многих поддерживаемых типов документов вы можете защитить подписанный документ паролем."

    # feature loop
    - icon: "protect"
      title: "Предотвращение несанкционированных изменений"
      content: "Защитите важные деловые документы, подписанные цифровым сертификатом, от несанкционированных изменений."

    # feature loop
    - icon: "convert"
      title: "Получение результатов в желаемых форматах"
      content: "Легко получайте подписанные файлы результатов в любом поддерживаемом формате. Вы также можете легко конвертировать документы MS Word в PDF."

    # feature loop
    - icon: "preview"
      title: "Предварительный просмотр документа"
      content: "Сохраните любую страницу документа как изображение для дальнейшей обработки."

    # feature loop
    - icon: "search"
      title: "Ищем подписи"
      content: "Есть возможность получить информацию о ранее добавленных подписях в конкретных документах."

    # feature loop
    - icon: "validate"
      title: "Проверка документов"
      content: "Проверка правильности подписей на любом подписанном документе."

    # feature loop
    - icon: "update"
      title: "Управление подписями"
      content: "После размещения подписи на странице документа ее можно удалить, переместить или обновить по мере необходимости."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "Некоторые варианты использования типичных операций GroupDocs.Signature для Java"
  items:
    # code sample loop
    - title: "Улучшите PDF-документ с помощью QR-кода"
      content: |
        Улучшение бизнес-процессов путем добавления [QR-кодов](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) на определенные страницы PDF-документов может оказаться полезным. Ниже приведен пример добавления QR-кода с помощью GroupDocs.Signature для Java.
        {{< landing/code title="Улучшите PDF-документ с помощью QR-кода">}}
        ```java {style=abap}
        // Загрузите документ для подписи
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Создание вариантов QR-кода с заранее заданным текстом
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Настройте тип и положение кодировки QR-кода на странице.
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Подпишите документ и сохраните его как файл результатов.
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Используйте цифровую подпись для защиты DOCX"
      content: |
        Вы можете [защитить документ](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/), используя личные или корпоративные подписи, хранящиеся в виде цифровых сертификатов. Документы, защищенные сертификатом, не могут быть изменены без признания подписи недействительной.
        {{< landing/code title="Используйте цифровую подпись для защиты DOCX">}}
        ```java {style=abap}   
        // Загрузите документ для цифровой подписи
        Signature signature = new Signature("file_to_sign.docx");
        
        // Укажите параметры цифровой подписи и укажите путь к файлу сертификата.
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Установите пароль сертификата
        options.setPassword("1234567890");

        // Подпишите документ и сохраните его по нужному пути.
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---