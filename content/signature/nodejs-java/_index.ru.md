---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: ru
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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

############################# Head ############################
head_title: ".NET, Java, облачные API и онлайн-приложения для подписи документов"
head_description: "Получите универсальное решение для электронной подписи документов для .NET, Java и облачных приложений. Подписывайте распространенные форматы документов онлайн с помощью простой функции перетаскивания"

############################# Header ############################
title: "Подписывать документы<br>с API Node.js"
description: "Подписывайте цифровые документы и изображения на любой платформе, используя наши гибкие API и решения на базе приложений для программистов и конечных пользователей."
words:
  for: "для"

actions:
  main: "Скачать с НПМ"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Signature бесплатно или запросите лицензию."

release:
  title: "Версия {0} выпущена"
  notes: "Посмотрите, что нового"
  downloads: "Загрузки"

code:
  title: "Подписание PDF-файлов с помощью Node.js"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // Выберите PDF-документ
    let signature = new Signature("sample.pdf");
    
    // Предоставить текст
    let options = new TextSignOptions("John Smith");
    
    // Установить цвет
    options.ForeColor = Color.Red;
    
    // Подписать документ и сохранить в файл
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Обзор GroupDocs.Signature"
  description: "Библиотека подписи документов, готовая к использованию в приложениях Node.js."
  features:
    # feature loop
    - title: "Решение для цифровых подписей для деловых документов с помощью Node.js"
      content: "GroupDocs.Signature for Node.js via Java предлагает полный набор вариантов цифровой подписи для документов PDF, Office и изображений. Доступны текст, штрих-коды, изображения, цифровые сертификаты и метаданные. Оптимизированная обработка документов обеспечивает эффективность."

    # feature loop
    - title: "Расширенное управление подписанными документами"
      content: "GroupDocs.Signature позволяет вам обрабатывать подписанные документы. Поиск и проверка подписей по различным критериям. Кроме того, извлекайте подробную информацию о документе или создавайте изображения предварительного просмотра страниц."

    # feature loop
    - title: "Разнообразные форматы вывода"
      content: "Наше решение обеспечивает широкий контроль над выходным форматом подписанных документов. Точно размещайте подписи на любой странице и настраивайте их внешний вид. Сохраняйте подписанные документы в различных поддерживаемых форматах и ​​при необходимости защищайте их паролями."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимость от платформы"
  description: "GroupDocs.Signature for Node.js via Java выполняет обработку документов в различных операционных системах."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Поддерживаемые форматы файлов"
  description: |
    GroupDocs.Signature for Node.js via Java упрощает операции с [популярными форматами файлов](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  description: "Подписывайте PDF-файлы, документы Office и изображения цифровыми подписями."

  items:
    # feature loop
    - icon: "sign"
      title: "Деловые подписи"
      content: "Используйте различные типы подписей для подписания документов. Размещайте цифровые подписи точно в любом месте страницы."

    # feature loop
    - icon: "custom"
      title: "Настройка внешнего вида подписи"
      content: "Настройте визуальные аспекты подписей, регулируя цвет, шрифт, границы, поворот и многое другое для достижения желаемого результата."

    # feature loop
    - icon: "password"
      title: "Документы, защищенные паролем"
      content: "Для многих поддерживаемых форматов документов защитите подписанные документы паролем для дополнительной безопасности."

    # feature loop
    - icon: "protect"
      title: "Предотвращение несанкционированных изменений"
      content: "Защитите важные деловые документы, подписанные цифровыми сертификатами, от несанкционированных изменений."

    # feature loop
    - icon: "convert"
      title: "Желаемые форматы вывода"
      content: "Легко получайте подписанные документы в любом поддерживаемом формате. С легкостью конвертируйте документы MS Word в формат PDF."

    # feature loop
    - icon: "preview"
      title: "Предварительный просмотр документов"
      content: "Сохраняйте отдельные страницы документа в виде изображений для будущих нужд."

    # feature loop
    - icon: "search"
      title: "Поиск по подписи"
      content: "Получите информацию о ранее добавленных подписях в ваших документах."

    # feature loop
    - icon: "validate"
      title: "Проверка документов"
      content: "Проверьте подлинность подписей, представленных в любом документе."

    # feature loop
    - icon: "update"
      title: "Управление подписями"
      content: "Удалите, переместите или измените любые подписи, размещенные на любой странице документа."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "Наглядные примеры, демонстрирующие типичные операции GroupDocs.Signature for Node.js via Java."
  items:
    # code sample loop
    - title: "Отметьте PDF с помощью QR-кодов"
      content: |
        Включение [штрих-кодов](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) в определенные страницы PDF-документа может упростить бизнес-процессы. В этом разделе приведен пример добавления QR-кода с помощью GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Как вставить QR-код в PDF.">}}
        ```javascript {style=abap}
        // Загрузите документ для подписи
        let signature = new Signature("file_to_sign.pdf");
        
        // Создание вариантов QR-кода с заранее заданным текстом
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Настройте тип и положение кодировки QR-кода на странице.
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Подпишите документ и сохраните его как файл результатов.
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Защита DOCX с помощью цифровой подписи"
      content: |
        [Защитите свои документы](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) с помощью подписей на основе цифровых сертификатов. Цифровая подпись защитит ваши деловые документы от изменения содержания.
        {{< landing/code title="Вот как обеспечить целостность документа.">}}
        ```javascript {style=abap}   
        // Загрузите документ для цифровой подписи
        let signature = new Signature("file_to_sign.pdf");
        
        // Укажите параметры цифровой подписи и укажите путь к файлу сертификата.
        let options = new DigitalSignOptions("certificate.pfx");

        // Установите пароль сертификата
        options.Password = "1234567890";

        // Подпишите документ и сохраните его по нужному пути.
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
