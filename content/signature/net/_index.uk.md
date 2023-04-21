---
############################# Static ############################
layout: "product"
date: 2022-03-01T15:12:22
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: uk
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET Digital Signature API – електронний підпис PDF Word Excel зображення"
head_description: "API цифрового підпису C# .NET, бібліотека електронного підпису для електронного підпису PDF, Word, електронних таблиць Excel, PowerPoint, зображень і графічних форматів документів."

############################# Header ############################
title: "Власний .NET API для електронних підписів"
description: "Додайте цифрові підписи до форматів документів і реалізуйте популярні типи електронних підписів (текст, зображення, QR-код, штрих-код, штамп і метадані) у програмах .NET."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Огляд"

            # button loop
            - link: "#features"
              text: "особливості"

            # button loop
            - link: "#support"
              text: "Підтримка"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Жива демо"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/net"
              text: "Ціноутворення"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      Використовуйте GroupDocs.Signature for .NET API для створення програм на C#, ASP.NET та інших технологіях на основі .NET, які дозволяють підписувати цифрові бізнес-документи, такі як PDF, Microsoft Word, електронні таблиці Excel, презентації PowerPoint, зображення, OpenDocument і інші галузеві стандартні формати файлів без необхідності встановлення додаткового програмного забезпечення. З цією бібліотекою електронних підписів легко працювати, а розробники .NET можуть легко додавати розширені функції цифрового підпису у свої програми, надаючи користувачам змогу безпечно підписувати, шукати та перевіряти електронні підписи в популярних форматах документів. Він підтримує реалізацію різноманітних типів підписів, таких як текст, зображення, штрих-код, QR-код, поле форми, штамп і метадані.  

      API підпису документа надає вам прості та розширені параметри пошуку, щоб миттєво знаходити необхідні підписи в документі. Параметри застосування стилю підпису, керування зовнішнім виглядом і налаштування властивостей підпису, таких як розміри, тінь, вирівнювання тощо, також доступні за допомогою цього багатофункціонального API підпису документів.  

      GroupDocs.Signature для .NET можна використовувати в будь-якому середовищі розробки, яке підтримує платформу .NET. Він сумісний з усіма мовами на основі .NET і підтримує популярні операційні системи (Windows, Linux, MacOS), де можна встановити фреймворки Mono або .NET (включаючи .NET Core).
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Нижче наведено огляд GroupDocs.Signature для .NET:
      
        left:
          enable: true
          icon: "fab fa-html5"
          title: "Типи підписів"
          content: |
            * Текстовий підпис
            * Підпис зображення
            * Цифрові підписи
            * Підпис QR-коду
            * Підпис штрих-коду
            * Печатка Підпис
            * Підпис метаданих
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Signature для .NET підтримує підписування всіх популярних форматів документів. За допомогою лише кількох рядків коду додайте підпис PDF, Microsoft Office Word, електронну таблицю Excel, зображення, HTML, електронну пошту Outlook, OneNote, Project і можливості підпису графіки у своїх програмах .NET. [Підтримувані формати документів.](https://docs.groupdocs.com/signature/net/supported-document-formats/)

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **Зображення**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Метафайли**: EMF, WMF, CMX
                * **Портативний**: PDF
                * **Масштабована векторна графіка**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **інші**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature для .NET підтримує такі операційні системи, фреймворки та менеджери пакетів:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операційні системи"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Підтримувані фреймворки"
              content: |
                * .NET Framework 2.0 or higher
                * Mono Framework 1.2 or higher
                * .NET Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Менеджер пакетів"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Середовища розробки"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature для функцій .NET"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Створення, пошук, оновлення, приховування, перевірка та видалення електронних підписів із підтримуваних форматів документів"

      # feature loop
      - icon: "fas fa-eye"
        content: "Укажіть розширені електронні підписи XML (XAdES) для електронних таблиць Excel"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Отримання вмісту зображень із документів, підписаних QR-кодом, штрих-кодом і підписами зображень"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Установіть висоту, ширину, поля та вирівнювання для тексту або підпису зображення та розміщення на певній сторінці"

      # feature loop
      - icon: "fas fa-code"
        content: "Пошук, перевірка та цифровий підпис у документах презентацій PowerPoint"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Підписуйте формати документів для обробки тексту водяними знаками рідного тексту"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Підтримує заокруглені кути для прямокутних типів підписів"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Застосуйте текстовий або графічний підпис на певному аркуші Excel або встановіть електронний підпис на всіх аркушах"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Укажіть певний номер рядка та стовпця, щоб розмістити текст або підпис зображення на аркуші Excel"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Застосуйте тінь до текстового підпису в Microsoft PowerPoint і налаштуйте його колір, кут і прозорість"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Налаштування стилів рамок і параметрів шрифту текстового підпису для аркушів Excel"

      # feature loop
      - icon: "fas fa-columns"
        content: "Установіть тип підпису зображення, напр. Круглі або квадратні та налаштуйте поля, колір шрифту, поворот"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Застосуйте цифрові сертифікати до документів, електронних таблиць і файлів PDF із лінією підпису"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Виконайте налаштування кольору, застосуйте прозорість і обертання до текстового підпису"

      # feature loop
      - icon: "fas fa-print"
        content: "Налаштуйте параметри яскравості та відтінків сірого та вкажіть відступ для підпису зображення на зображенні"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Вбудовувати користувацькі об’єкти, серіалізувати, а також шифрувати та розшифровувати значення підпису метаданих PDF-документа"

      # feature loop
      - icon: "fas fa-lock"
        content: "Приховати, видалити або налаштувати вигляд цифрових підписів із PDF-документів"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Підписуйте PDF-документи за допомогою поля цифрової форми та текстового підпису як зображення, анотації, наклейки або водяного знака"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Поставте текстовий підпис у поля форми документів MS Word і PDF"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Укажіть довільні сторінки документів для обробки підпису або розширеної перевірки електронного підпису для файлів Word"

      # feature loop
      - icon: "fas fa-heading"
        content: "Збережіть підписаний файл зображення в іншому форматі та експортуйте підписану електронну таблицю як зображення або багатосторінковий TIFF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Призначення, зміна та видалення пароля для підписаних файлів і застосування електронного підпису до захищених паролем файлів"

      # feature loop
      - icon: "fas fa-cube"
        content: "Робочі аркуші eSign, слайди PowerPoint, документи Word і зображення з настроюваними об’єктами в метаданих"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Налаштуйте характерні стилі пензля: суцільний, текстурний, лінійний градієнт і радіальний градієнт"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Підписуйте документи спеціальним зашифрованим текстом або даними QR-коду"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Пошук і підпис файлів у форматі DjVu як документ із зображенням"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Отримайте інформацію про документ, наприклад, кількість сторінок, за допомогою URL-адреси файлу"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Пошук, підпис і перевірка файлів CorelDraw як документів із зображеннями"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Зберігайте інформацію про історію оброблених або видалених підписів, що зберігається в метаданих"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Додайте користувацький об’єкт даних, VCard або об’єкт електронної пошти до QR-коду та перевірте зашифрований QR-код у файлах PDF"

    more_feature:
      # more_feature_loop
      - title: "Легко додавайте цифрові підписи"
        content: |
          GroupDocs.Signature for .NET API дозволяє додавати різні типи підписів до підтримуваних форматів файлів. За допомогою GroupDocs.Signature для .NET можна застосовувати такі типи підписів, як текст, зображення, цифровий підпис, штамп, QR-код, штрих-код і метадані. У наведеному нижче прикладі коду показано, як застосувати текстовий підпис до документа PDF:

          ```cs
          using (Signature signature = new Signature("D:\\sample.pdf"))
          {
          TextSignOptions options = new TextSignOptions("John Smith")
          {
          // встановити колір тексту
          ForeColor = Color.Red
          };
          // підписати документ у файл
          signature.Sign("D:\\signed.pdf", options);
          }
          ```

      # more_feature_loop
      - title: "Підтримувані типи підпису штрих-коду"
        content: |
          Наш API для обробки підписів пропонує вам функцію застосування підписів штрих-кодів до підтримуваних форматів документів. GroupDocs.Signature для .NET підтримує різні типи штрих-кодів, як-от Code128, Code39Extended, Code39Standard, EAN14, EAN8, ITF14, UPCA та UPCE. Також надається статичний об’єкт під назвою «AllTypes» для підтримки всіх зареєстрованих типів штрих-кодів.

      # more_feature_loop
      - title: "Пошук підписів і сертифікатів"
        content: |
          GroupDocs.Signature for .NET API дозволяє шукати цифрові сертифікати в документах Word, електронних таблицях Excel і PDF-файлах. Ви також можете отримати всі цифрові сертифікати, зареєстровані в системі. Підписи метаданих також можна шукати в документах Word, електронних таблицях Excel, зображеннях і PDF-файлах за допомогою GroupDocs.Signature for .NET API.  

          За допомогою GroupDocs.Signature for .NET API ви можете шукати QR-код і підписи штрих-коду в будь-якому документі, презентації, електронній таблиці, зображенні, а також PDF-файлі та переглядати хід пошуку. Ви також можете шукати спеціальний об’єкт даних у документах, підписаних QR-Code Signature.

      # more_feature_loop
      - title: "Параметри розширеного пошуку для штрих-коду"
        content: |
          Ви можете дуже легко шукати та знаходити необхідний штрих-код за допомогою GroupDocs.Signature for.NET API, оскільки наш API підпису пропонує розширені параметри пошуку. Вони дозволяють шукати штрих-код на певній сторінці, шукати в документі, вказувати різні сторінки для пошуку (перша, остання, парна, непарна), шукати штрих-код певного типу кодування, шукати штрих-код на основі певного текстового рядка або шукати штрих-код на основі рядка з параметром «містить».

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature пропонує API для підпису документів для інших популярних середовищ розробки"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
          product: "GroupDocs.Signature"
          platform: "Java"
          link: "/signature/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---