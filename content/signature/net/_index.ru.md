---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:01
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: ru
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

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
title: "Подписывать документы<br>через .NET API"
description: "Подписывайте цифровые документы и изображения на любой платформе, используя наши гибкие API и решения на базе приложений для программистов и конечных пользователей."
words:
  for: "для"

actions:
  main: "Бесплатная загрузка NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Signature бесплатно или запросите лицензию."

release:
  title: "Версия {0} выпущена"
  notes: "Посмотрите, что нового"
  downloads: "Загрузки"

code:
  title: "Подписание PDF-файлов на C#"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Выберите PDF-документ
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Предоставить текст
        var options = new TextSignOptions("John Smith")
        {
            // Установить цвет
            ForeColor = Color.Red
        };
        // Подписать документ и сохранить в файл
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Обзор GroupDocs.Signature"
  description: "API для подписания документов и связанных с ним операций в приложениях .NET."
  features:
    # feature loop
    - title: "Добавление подписей к деловым документам в C#"
      content: "Подписание документов. С помощью GroupDocs.Signature для .NET вы можете добавлять в документы PDF и Office различные типы подписей, такие как текст, изображения, штрих-коды и цифровые сертификаты. Этот API позволяет подписывать документы практически с любым типом данных, включая скрытые метаданные."

    # feature loop
    - title: "Обработка подписанных документов"
      content: "Дополнительная обработка. Вы можете выполнять мощные операции с подписанными документами, используя GroupDocs.Signature. Это включает в себя поиск существующих подписей в деловых документах и ​​их проверку по определенным критериям. Кроме того, вы можете получать информацию о документе и просматривать страницы с помощью этого .NET API."

    # feature loop
    - title: "Настройка результатов"
      content: "GroupDocs.Signature для .NET предлагает широкие возможности настройки. Вы можете точно расположить подписи в любом месте страницы документа и настроить их внешний вид, используя различные настройки. Кроме того, этот API поддерживает сохранение обработанных документов в широком диапазоне поддерживаемых форматов."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимость от платформы"
  description: "GroupDocs.Signature для .NET поддерживает следующие операционные системы, платформы и менеджеры пакетов."
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
    GroupDocs.Signature для .NET поддерживает операции со следующими [форматами файлов](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Подписание PDF-файлов, документов Office и изображений быстро и точно"

  items:
    # feature loop
    - icon: "sign"
      title: "Подписание документов"
      content: "Точно добавляйте один или несколько поддерживаемых типов подписей в любом указанном месте деловых документов."

    # feature loop
    - icon: "custom"
      title: "Настройка подписей"
      content: "Используйте такие функции, как цвет, шрифт, граница, поворот и т. д., чтобы настроить внешний вид подписей."

    # feature loop
    - icon: "password"
      title: "Защита документа паролем"
      content: "Защитите определенные типы документов, установив пароль после подписания."

    # feature loop
    - icon: "protect"
      title: "Защита от изменений"
      content: "Предотвратите изменение важных деловых документов после добавления подписи с помощью цифрового сертификата."

    # feature loop
    - icon: "convert"
      title: "Конвертируйте подписанные файлы в другие форматы"
      content: "Преобразуйте подписанные файлы в нужные форматы, например сохраняя документ Word в формате PDF."

    # feature loop
    - icon: "preview"
      title: "Извлечение превью страниц"
      content: "Извлекайте страницы из подписанных документов как отдельные изображения для дальнейшей обработки."

    # feature loop
    - icon: "search"
      title: "Поиск подписи в документах"
      content: "Получить информацию о ранее добавленных подписях в определенных документах."

    # feature loop
    - icon: "validate"
      title: "Проверка подписанных документов"
      content: "Проверьте правильность подписания документов, используя функции проверки."

    # feature loop
    - icon: "update"
      title: "Обновить или удалить подписи"
      content: "Легко перемещайте определенные подписи на странице, изменяйте их текст или удаляйте их без каких-либо проблем."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "Некоторые варианты использования типичных операций GroupDocs.Signature для .NET"
  items:
    # code sample loop
    - title: "Добавить QR-код в PDF"
      content: |
        Добавление [QR-кодов](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) на определенные страницы PDF-документов может улучшить бизнес-процессы. Ниже приведен пример добавления QR-кода с помощью GroupDocs.Signature.
        {{< landing/code title="Как вставить QR-код в PDF.">}}
        ```csharp {style=abap}
        // Загрузите документ для подписи
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Создание вариантов QR-кода с заранее заданным текстом
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Настройте тип и положение кодировки QR-кода на странице.
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Подпишите документ и сохраните его как файл результатов.
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Защита документа DOCX с помощью цифрового сертификата"
      content: |
        Вы можете [защитить документ](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/), используя личные или корпоративные подписи, хранящиеся в виде цифровых сертификатов. Такие защищенные документы не могут быть изменены без аннулирования подписи.
        {{< landing/code title="Вот как обеспечить целостность документа.">}}
        ```csharp {style=abap}   
        // Загрузите документ для цифровой подписи
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Укажите параметры цифровой подписи и укажите путь к файлу сертификата.
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Установите пароль сертификата
                Password = "1234567890"
            };
            // Подпишите документ и сохраните его по нужному пути.
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
