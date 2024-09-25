---
############################# Static ############################
layout: "landing"
date: 2024-09-25T12:45:24
draft: false

lang: uk
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
head_title: "Бібліотека цифрових підписів Java - GroupDocs.Signature"
head_description: "Розширюйте можливості програм Java за допомогою електронних підписів за допомогою GroupDocs.Signature. Підписуйте ділові документи швидко та без зусиль."

############################# Header ############################
title: "Підписувати документи через Java API"
description: "Підписуйте цифрові документи та зображення на будь-якій платформі за допомогою наших гнучких API та рішень на основі програм для програмістів і кінцевих користувачів."
words:
  for: "для"

actions:
  main: "Безкоштовне завантаження Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Готові почати?"
  description: "Спробуйте функції GroupDocs.Signature безкоштовно або подайте запит на ліцензію"

release:
  title: "Випущено версію {0}"
  notes: "Подивіться, що нового"
  downloads: "Завантаження"

code:
  title: "Підписуйте PDF-файли в Java"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Виберіть документ PDF
    Signature signature = new Signature("sample.pdf");
    
    // Надайте текст
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Підпишіть документ і збережіть його у файлі
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Огляд GroupDocs.Signature"
  description: "API для виконання підписів документів і пов’язаних операцій у програмах Java"
  features:
    # feature loop
    - title: "Покращено ділові документи з цифровими підписами в Java"
      content: "Швидкий і настроюваний підпис: GroupDocs.Signature для Java пропонує широкий вибір цифрових підписів для PDF-файлів, зображень і документів Office. Ви можете використовувати текст, штрих-коди, QR-коди, цифрові сертифікати, зображення або приховані метадані. Оформлення документів відбувається швидко та ефективно."

    # feature loop
    - title: "Маніпулювання підписаними документами"
      content: "Розширена обробка документів передбачає потужні операції над підписаними документами за допомогою GroupDocs.Signature для Java. Ви можете шукати та перевіряти підписи, додані до ділових документів, використовуючи різні корисні критерії. Крім того, ви можете отримати доступ до детальної інформації про документ або отримати попередні зображення його сторінок."

    # feature loop
    - title: "Різноманітність варіантів виходу"
      content: "Надійні параметри підпису дозволяють налаштовувати вихід для документів, підписаних за допомогою GroupDocs.Signature для Java. Ви можете точно розмістити будь-який підпис на будь-якій сторінці документа та різними способами налаштувати його вигляд. Java API підтримує збереження підписаних бізнес-документів у численних підтримуваних форматах і надає параметри для їх захисту паролями."

############################# Platforms ############################
platforms:
  enable: true
  title: "Незалежність від платформи"
  description: "GroupDocs.Signature для Java підтримує такі операційні системи, фреймворки та менеджери пакетів"
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
  title: "Підтримувані формати файлів"
  description: |
    GroupDocs.Signature для Java підтримує операції з такими [форматами файлів](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Функції GroupDocs.Signature"
  description: "Підписування PDF-файлів, документів Office і зображень за допомогою цифрових підписів"

  items:
    # feature loop
    - icon: "sign"
      title: "Додавання підписів"
      content: "Підпишіть документ за допомогою різних підтримуваних типів підписів, розмістивши цифровий підпис точно в будь-якому місці на будь-якій сторінці."

    # feature loop
    - icon: "custom"
      title: "Налаштування результатів"
      content: "Налаштуйте зовнішній вигляд підпису, налаштувавши колір, шрифт, рамку, поворот та інші функції, щоб досягти бажаного результату."

    # feature loop
    - icon: "password"
      title: "Захист документів паролем"
      content: "Для багатьох підтримуваних типів документів ви можете захистити підписаний документ паролем."

    # feature loop
    - icon: "protect"
      title: "Запобігання несанкціонованим змінам"
      content: "Захистіть важливі ділові документи, підписані цифровим сертифікатом, від несанкціонованих змін."

    # feature loop
    - icon: "convert"
      title: "Отримання результатів у бажаних форматах"
      content: "Легко отримуйте підписані файли результатів у будь-якому підтримуваному форматі. Ви також можете легко конвертувати документи MS Word у PDF."

    # feature loop
    - icon: "preview"
      title: "Попередній перегляд документа"
      content: "Збережіть будь-яку сторінку документа як зображення для подальшої обробки."

    # feature loop
    - icon: "search"
      title: "Пошук підписів"
      content: "Є можливість отримати інформацію про раніше додані підписи в окремих документах."

    # feature loop
    - icon: "validate"
      title: "Перевірка документів"
      content: "Перевірте правильність підписів на будь-якому підписаному документі."

    # feature loop
    - icon: "update"
      title: "Управління підписами"
      content: "Після розміщення підпису на сторінці документа його можна видалити, перемістити або оновити за потреби."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Зразки коду"
  description: "Деякі випадки використання типових операцій GroupDocs.Signature для Java"
  items:
    # code sample loop
    - title: "Доповніть PDF-документ QR-кодом"
      content: |
        Покращення бізнес-процесів шляхом додавання [QR-кодів](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) до певних сторінок PDF-документів може бути цінним. Є приклад того, як додати QR-код за допомогою GroupDocs.Signature для Java.
        {{< landing/code title="Доповніть PDF-документ QR-кодом">}}
        ```java {style=abap}
        // Завантажте документ для підпису
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Створіть параметри QR-коду з попередньо визначеним текстом
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Налаштуйте тип кодування QR-коду та положення на сторінці
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Підпишіть документ і збережіть його як файл результату
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Використовуйте цифровий підпис для захисту DOCX"
      content: |
        Ви можете [захистити документ](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) за допомогою особистих або корпоративних підписів, які зберігаються як цифрові сертифікати. Документи, закріплені сертифікатом, не можуть бути змінені без втрати підпису.
        {{< landing/code title="Використовуйте цифровий підпис для захисту DOCX">}}
        ```java {style=abap}   
        // Завантажте документ для цифрового підпису
        Signature signature = new Signature("file_to_sign.docx");
        
        // Укажіть параметри цифрового підпису та вкажіть шлях до файлу сертифіката
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Встановіть пароль сертифіката
        options.setPassword("1234567890");

        // Підпишіть документ і збережіть його в потрібному місці
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---