---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API цифрового підпису Java, додайте електронний підпис до PDF-файлу Word Excel Image"
head_description: "API цифрового підпису Java. Бібліотека електронних підписів для цифрового підпису PDF, Microsoft Word, електронних таблиць Excel, презентацій PowerPoint і форматів документів із зображеннями."

############################# Header ############################
title: "Java API для керування цифровими підписами"
description: "Керуйте електронним підписом зображень, QR-кодів, штрих-кодів, метаданих, тексту та типів печаток у програмах Java для підписання зображень і форматів файлів цифрових документів."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

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
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Ціноутворення"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API допомагає розробляти Java-додатки з функціями електронних підписів для підпису цифрових документів підтримуваних форматів без інсталяції зовнішнього програмного забезпечення. Він підтримує маніпуляції та керування різними типами електронних підписів, такими як зображення, штрих-код, QR-код, штамп, текст, оптичні та метадані. Усі ваші електронні ділові документи, такі як Microsoft Office Word, презентації PowerPoint, електронні таблиці Excel, зображення та PDF-файли, можна підписати цифровим підписом, налаштувавши властивості підпису, наприклад. тінь, розміри, вирівнювання тощо відповідно до ваших вимог. Бібліотека цифрового підпису проста та легка, складається з одного файлу DLL, який можна легко інтегрувати в нову або існуючу програму Java.  

      За допомогою GroupDocs.Signature for Java API ви можете завантажити всі зареєстровані сертифікати з системи або знайти існуючі підписи за допомогою простого та розширеного пошуку. Параметри роботи із захищеними паролем документами, визначення загальних властивостей підпису (розмір тексту, непрозорість, обертання, перевірка, властивості шрифту, параметри кольору, номер сторінки, ширина, верх, ліворуч тощо) і підтримка реалізації різних типів електронного підпису роблять його надійним Рішення для керування електронними підписами для цифрових документів.  

      GroupDocs.Signature для Java сумісний з усіма версіями Java і підтримує популярні операційні системи (Windows, Linux, MacOS), які можуть запускати середовище виконання Java
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ось огляд функцій GroupDocs.Signature для Java:
      
        right:
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
            * Поле форми Підпис
      
      ## TAB TWO ##
      tab_two:
        description: |
          API електронного підпису Java підтримує різні формати файлів документів, перелічені нижче. [Підтримувані формати документів.](https://docs.groupdocs.com/signature/java/supported-document-formats/)

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
          GroupDocs.Signature для Java підтримує наступні операційні системи, фреймворки та менеджери пакетів:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операційні системи"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Підтримувані фреймворки"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Середовища розробки"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Інструмент автоматизації збірки"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature for Java Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Створюйте, читайте, змінюйте, приховуйте та видаляйте електронні підписи з підтримуваних форматів документів"

      # feature loop
      - icon: "fas fa-eye"
        content: "Доступ до підписаного документа з потоку, відносного або абсолютного шляху"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Застосуйте текстовий підпис до документів, електронних таблиць, презентацій, зображень і PDF-файлів"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Додайте текстовий підпис як анотацію, наклейку, зображення до PDF-файлів, а також налаштуйте стиль і колір"

      # feature loop
      - icon: "fas fa-code"
        content: "Підпишіть PDF-документ, файл зображення та отримайте вихідні дані в іншому форматі файлу"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Цифровий підпис зображень за допомогою текстового підпису як водяного знака та додавання прозорості, обертання до електронного підпису"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Шукайте сертифікати та підписуйте документи Microsoft Word, Excel і PDF цифровими сертифікатами"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Підписуйте формати документів для обробки тексту водяними знаками рідного тексту"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Використовуйте QR-код, штрих-код для підпису Word, Slide, Cell, PDF і файлів зображень"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Налаштуйте та застосовуйте підписи печаток для захисту підтримуваних форматів файлів"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Налаштування та призначення підписів зображень документам, електронним таблицям, презентаціям, зображенням і PDF-файлам"

      # feature loop
      - icon: "fas fa-columns"
        content: "Налаштуйте властивості підпису, наприклад, зовнішній вигляд, поля, вирівнювання тощо."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Застосувати цифровий підпис до захищеного паролем документа"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Виконайте перевірку тексту PDF-документів за допомогою обробника підписів"

      # feature loop
      - icon: "fas fa-print"
        content: "Цифрова перевірка документів Word, Cell, PDF за допомогою контейнерів сертифікатів .CER і .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Укажіть різні типи одиниць вимірювання (наприклад, міліметри, пікселі тощо) для текстових підписів PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Отримайте інформацію про документ за допомогою файлу чи URL-адреси – додайте підписи полів форми до PDF-документів"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Додайте користувацький об’єкт даних, вбудовану візитну картку, електронну пошту, EPC, MeCard або об’єкт події до QR-коду"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Застосування різних стилів пензля до підписів, наприклад, градієнта, радіального, суцільного та текстурного пензля"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Підпишіть документ, розташований на FTP або в хмарному сховищі Azure"

      # feature loop
      - icon: "fas fa-heading"
        content: "Встановіть вирівнювання тексту всередині фігур для документів, слайдів, зображень і PDF-файлів"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Пошук, перевірка та цифровий підпис у документах презентацій PowerPoint"

      # feature loop
      - icon: "fas fa-cube"
        content: "Розміщення підпису за допомогою пікселів у документах клітинок і позиціонування тексту для підписів печаток"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Реалізуйте прямокутний штамповий підпис із закругленими кутами"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Розширте підписи штрих-кодів і QR-кодів вмістом даних зображення"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Додайте зашифровані підписи метаданих під час роботи з параметрами підпису та пошуку"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Вбудовуйте спеціальні об’єкти в підписи метаданих у Word, Excel і презентаціях"

    more_feature:
      # more_feature_loop
      - title: "Легко налаштовуйте та застосовуйте електронні підписи"
        content: |
          GroupDocs.Signature for Java API дозволяє налаштовувати та додавати електронні підписи до підтримуваних форматів документів. Нижче наведено приклад коду, який показує, як просто застосувати текстовий підпис до файлу PDF:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // встановити позицію підпису
          options.setLeft(100);
          options.setTop(100);
          
          // встановити прямокутник підпису
          options.setWidth(100);
          options.setHeight(30);

          // встановити колір тексту та шрифт
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // підписати документ у файл
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Підтримувані типи кодування штрих-коду для електронного підпису"
        content: |
          Використовуючи GroupDocs.Signature для Java API, ви можете застосовувати штрих-коди та підписи QR-кодів до підтримуваних форматів файлів. GroupDocs.Signature для Java підтримує величезну кількість типів кодування штрих-кодів, щоб задовольнити більшість вимог. Підтримувані типи кодування штрих-кодів: Code 11, Code 128, Code 16K/32, Databar codes, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard та Code39 Розширений.

          Подібним чином GroupDocs.Signature для Java API дозволяє використовувати типи QR-кодів, такі як QR, Aztec і Data Matrix. Підтримувані типи кодування QR-коду включають Aztec, DataMatrix, GS1 DataMatrix і GS1 QR.

      # more_feature_loop
      - title: "Пошук підписів і сертифікатів"
        content: |
          За допомогою GroupDocs.Signature for Java API ви можете шукати підписи QR-коду та штрих-коду в будь-якому документі, презентації, електронній таблиці, зображенні, а також PDF-файлі та отримувати результати пошуку. Ви також можете шукати спеціальний об’єкт даних у документах, підписаних QR-кодом, а також шукати стандартні VCard та об’єкт електронної пошти в документах, підписаних QR-кодом. Також підтримується перевірка зашифрованого тексту підписів QR-коду, а також пошук підпису метаданих у документах PDF. Застосуйте додаткові критерії пошуку для цифрових підписів документів Words & Cells.  

          Опція пошуку також доступна для підпису метаданих для документів Word, слайдів і електронних таблиць, тоді як пошук по полю форми доступний для документів PDF.

      # more_feature_loop
      - title: "Налаштуйте властивості електронного підпису"
        content: |
          Щоб покращити UX кінцевих користувачів, GroupDocs.Signature for Java API надає багато властивостей, які можна досить легко налаштувати. Ви можете встановити параметри шрифту та кольору (Колір фону, Колір переднього плану, Напівжирний, Курсив, Підкреслення, Сімейство шрифтів, Розмір шрифту тощо), Параметри фону та рамки (Колір фону, Прозорість фону, Колір рамки, Стиль тире на рамці, Товщина рамки, Прозорість меж тощо), поля підпису (ліве, верхнє, ширина, висота, відступ тощо), а також налаштування області підпису зображення та вирівнювання підпису (горизонтальне вирівнювання, вертикальне вирівнювання тощо).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature пропонує API для підпису документів для інших популярних середовищ розробки"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---