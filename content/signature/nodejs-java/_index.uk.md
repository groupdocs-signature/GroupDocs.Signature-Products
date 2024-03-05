---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: uk
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
head_title: ".NET, Java, хмарні API та онлайн-додатки для підпису документів"
head_description: "Отримайте комплексне рішення електронного підпису документів для .NET, Java і хмарних програм. Підписуйте стандартні формати документів онлайн за допомогою простої функції перетягування"

############################# Header ############################
title: "Підписувати документи<br>з API Node.js"
description: "Підписуйте цифрові документи та зображення на будь-якій платформі за допомогою наших гнучких API та рішень на основі програм для програмістів і кінцевих користувачів."
words:
  for: "для"

actions:
  main: "Завантажити з NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Готові почати?"
  description: "Спробуйте функції GroupDocs.Signature безкоштовно або подайте запит на ліцензію"

release:
  title: "Випущено версію {0}"
  notes: "Подивіться, що нового"
  downloads: "Завантаження"

code:
  title: "Підпис PDF-файлів за допомогою Node.js"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Виберіть документ PDF
    let signature = new Signature("sample.pdf");
    
    // Надайте текст
    let options = new TextSignOptions("John Smith");
    
    // Встановити колір
    options.ForeColor = Color.Red;
    
    // Підпишіть документ і збережіть його у файлі
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Огляд GroupDocs.Signature"
  description: "Бібліотека для підписання документів, готова до використання в програмах Node.js"
  features:
    # feature loop
    - title: "Рішення для цифрових підписів для бізнес-документів із Node.js"
      content: "GroupDocs.Signature for Node.js via Java пропонує повний набір параметрів цифрового підпису для PDF, документів Office і зображень. Доступні текст, штрих-коди, зображення, цифрові сертифікати та метадані. Впорядкована обробка документів забезпечує ефективність."

    # feature loop
    - title: "Розширене маніпулювання підписаними документами"
      content: "GroupDocs.Signature дає вам змогу обробляти підписані документи. Шукайте та перевіряйте підписи за різними критеріями. Крім того, витягніть детальну інформацію про документ або створіть попередні зображення сторінок."

    # feature loop
    - title: "Різноманітні вихідні формати"
      content: "Наше рішення забезпечує широкий контроль над вихідним форматом підписаних документів. Точне розташування підписів на будь-якій сторінці та налаштування їх зовнішнього вигляду. Зберігайте підписані документи в численних підтримуваних форматах і додатково захищайте їх паролями."

############################# Platforms ############################
platforms:
  enable: true
  title: "Незалежність від платформи"
  description: "GroupDocs.Signature for Node.js via Java виконує обробку документів за допомогою різних операційних систем"
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
  title: "Підтримувані формати файлів"
  description: |
    GroupDocs.Signature for Node.js via Java полегшує роботу з [популярними форматами файлів](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Формати Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Зображення та інші формати
        * **Портативний:** PDF
        * **Зображення:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Інші офісні формати:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Інші формати
        * **Інтернет:** HTML, MHTML
        * **Архіви:** ZIP, TAR, 7Z
        * **Сертифікати:** PFX

############################# Features ############################
features:
  enable: true
  title: "Особливості GroupDocs.Signature"
  description: "Підписуйте PDF-файли, документи Office і зображення цифровими підписами"

  items:
    # feature loop
    - icon: "sign"
      title: "Ділові підписи"
      content: "Використовуйте різні типи підписів для підпису документів. Точне розміщення цифрових підписів на будь-якій сторінці."

    # feature loop
    - icon: "custom"
      title: "Налаштування зовнішнього вигляду підпису"
      content: "Налаштуйте візуальні аспекти підписів, налаштувавши колір, шрифт, межі, обертання тощо, щоб досягти бажаного результату."

    # feature loop
    - icon: "password"
      title: "Документи, захищені паролем"
      content: "Для багатьох підтримуваних форматів документів захищайте підписані документи паролем для додаткової безпеки."

    # feature loop
    - icon: "protect"
      title: "Запобігання неавторизованим змінам"
      content: "Захистіть важливі ділові документи, підписані цифровими сертифікатами, від несанкціонованих змін."

    # feature loop
    - icon: "convert"
      title: "Бажані вихідні формати"
      content: "Без зусиль отримуйте підписані документи в будь-якому підтримуваному форматі. Легко конвертуйте документи MS Word у формат PDF."

    # feature loop
    - icon: "preview"
      title: "Попередній перегляд документів"
      content: "Збережіть окремі сторінки документа як зображення для майбутніх потреб."

    # feature loop
    - icon: "search"
      title: "Пошук підпису"
      content: "Отримайте інформацію про раніше додані підписи у своїх документах."

    # feature loop
    - icon: "validate"
      title: "Перевірка документів"
      content: "Перевірити справжність підписів на будь-якому документі."

    # feature loop
    - icon: "update"
      title: "Керування підписами"
      content: "Видаліть, перемістіть або змініть будь-які підписи, розміщені на будь-якій сторінці документа."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Зразки коду"
  description: "Ілюстративні приклади, що демонструють типові операції GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Позначте PDF QR-кодами"
      content: |
        Додавання [штрих-кодів](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) до конкретних сторінок документа PDF може оптимізувати бізнес-процеси. У цьому розділі наведено приклад додавання QR-коду за допомогою GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Як вставити QR-код у PDF.">}}
        ```javascript {style=abap}
        // Завантажте документ для підпису
        let signature = new Signature("file_to_sign.pdf");
        
        // Створіть параметри QR-коду з попередньо визначеним текстом
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Налаштуйте тип кодування QR-коду та положення на сторінці
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Підпишіть документ і збережіть його як файл результату
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Захист DOCX за допомогою цифрового підпису"
      content: |
        [Захистіть свої документи](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) за допомогою підписів на основі цифрових сертифікатів. Цифровий підпис захистить ваші ділові документи від зміни вмісту.
        {{< landing/code title="Ось як забезпечити цілісність документа.">}}
        ```javascript {style=abap}   
        // Завантажте документ для цифрового підпису
        let signature = new Signature("file_to_sign.docx");
        
        // Укажіть параметри цифрового підпису та вкажіть шлях до файлу сертифіката
        let options = new DigitalSignOptions("certificate.pfx");

        // Встановіть пароль сертифіката
        options.Password = "1234567890";

        // Підпишіть документ і збережіть його в потрібному місці
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
