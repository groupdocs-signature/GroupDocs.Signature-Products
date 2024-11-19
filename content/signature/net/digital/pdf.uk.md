



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:18
draft: false
lang: uk
format: Pdf
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Додавання цифрових електронних підписів до файлів PDF за допомогою C#"
head_description: "Додайте цифровий підпис на файл PDF за допомогою C# всього за кілька рядків коду. Використовуйте GroupDocs.Signature for .NET для підписання численних форматів файлів."

############################# Header ############################
title: "eSign PDF з цифровими підписами" 
description: "Захистіть цілісність ваших бізнес-документів, запечатуючи їх цифровими сертифікатами, використовуючи надійні можливості GroupDocs.Signature for .NET. Ми пропонуємо універсальні рішення для маркування і безпеки ваших документів."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити безкоштовно"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Про GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Дізнатися більше"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) є складним рішенням для підписання, яке полегшує виконання широкого спектра завдань обробки документів. Він дозволяє встраювати текст, зображення, цифрові сертифікати та штампи у файли більше ніж 60 форматів, включаючи PDF, MS Office, зображення, ZIP файли та інші основні бізнес-формати. Крім того, підписані документи можуть бути легко пошуковані, перевірені, змінені або видалені за необхідності.

############################# Steps ############################
steps:
    enable: true
    title: "Як захистити PDF цифровими сертифікатами в C#"
    content: |
      [GroupDocs.Signature](/signature/net/) надає розробникам .NET можливість захистити документи PDF від змін за допомогою цифрових підписів. Покращте свої бізнес-додатки потужними можливостями захисту даних.
      
      1. Передайте документ PDF в конструктор класу Signature.
      2. Використовуйте цифровий сертифікат та його пароль для захисту документа.
      3. За бажанням, додайте візуальне представлення цифрового підпису на сторінки документа.
      4. Підпишіть документ, щоб забезпечити його незмінність.
   
    code:
      platform: "net"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Приклад підписів"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "натисніть для копіювання"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Використовуйте Signature для цифрового підписання документа
        using (Signature signature = new Signature("input.pdf"))
        {
            // Надайте цифровий сертифікат та відповідний пароль
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // Налаштуйте візуальне представлення за потреби
                PageNumber = 1,
                Left = 50,
                Top = 50
            };

            // Захистіть документ за допомогою цифрового сертифіката
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Покращте або захистіть вміст документа за допомогою підписів"
  description: "Бібліотека GroupDocs.Signature for .NET розроблена для підписання всіх поширених форматів файлів. Оптимізуйте ваші бізнес-процеси, додаючи, змінюючи, перевіряючи чи видаляючи різноманітні підписи."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Ключові Особливості GroupDocs.Signature"
  features:
    # feature loop
    - title: "Включайте підписи в документи"
      content: "Точно вбудовуйте підписи тексту, зображень, штрих-кодів, QR-кодів або штампів на будь-якій сторінці будь-якого підтримуваного документа. Ви також можете додавати або редагувати приховану метадані, такі як EXIF, в зображеннях та більшості типів файлів. Забезпечте цілісність вмісту вашого документа за допомогою цифрових підписів."

    # feature loop
    - title: "Пошук та перевірка підписів"
      content: "Обробка після підпису надає численні можливості. Перевірте, що ваші підписані документи були оброблені коректно. Для більшого контролю ви можете отримати повний список усіх підписів за допомогою функції пошуку."

    # feature loop
    - title: "Зміна підписів"
      content: "Більшість типів підписів повністю редаговані. Ви маєте можливість налаштовувати текст, переміщати елементи, змінювати кольори, змінювати розмір і багато іншого."

    # feature loop
    - title: "Видалення зайвих підписів"
      content: "Наше рішення надає повні CRUD-операції для підписів. За потреби ви можете видалити різні типи підписів, включаючи цифрові сертифікати, з вашого документа."
      
  code_samples:
    # code sample loop
    - title: "Захистіть документи за допомогою цифрових підписів"
      content: |
        Дізнайтеся, як запобігти модифікації документа за допомогою цифрових підписів.
        {{< landing/code title="C#">}}
        ```csharp {style=abap}
        // Надайте документ, що підписується
        using (Signature signature = new Signature("input.pdf"))
        {
            // Використовуйте дійсний цифровий сертифікат з відповідним паролем
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                Password = "1234567890",

                // Вкажіть будь-яку додаткову текстову інформацію
                Reason = "Security issue",
                Contact = "John Smith",
                Location = "Office D.W.",

                // Включте зображення та інші параметри для візуального представлення
                ImageFilePath = "image.png",
                AllPages = true,
                VerticalAlignment = VerticalAlignment.Center,
                HorizontalAlignment = HorizontalAlignment.Left,
                Width = 60,
                Height = 80,

                Margin = new Padding() {  Bottom = 10, Right = 10 }
            };

            // Збережіть захищений документ у визначеному місці
            SignResult result = signature.Sign("output.pdf", options);
        }
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Спробуйте можливості GroupDocs.Signature безкоштовно або запросіть ліцензію"
  items:
    #  loop
    - title: "Завантаження Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Ознайомтеся з нашими видатними функціями"
    exclude: "digital"
    description: "Ми пропонуємо багатий вибір форматів підписів та потужних операцій."
    items: 
          
        # operation loop 1
        - name: "Електронні підписи"
          operation: "esign"
          link: "/signature/net/esign/pdf/"
          description: "Додавайте різні типи підписів до підтримуваних форматів файлів"

        # operation loop 2
        - name: "Додати текст до документів"
          operation: "text"
          link: "/signature/net/text/pdf/"
          description: "Збагачуйте вміст документів настроювальними текстовими підписами"

        # operation loop 3
        - name: "Зображення підписів"
          operation: "image"
          link: "/signature/net/image/pdf/"
          description: "Розміщуйте будь-яке зображення у будь-якому місці документа"

        # operation loop 4
        - name: "Генерувати штрих-коди"
          operation: "barcode"
          link: "/signature/net/barcode/pdf/"
          description: "Створюйте та вставляйте різні штрих-коди у підтримувані документи"

        # operation loop 5
        - name: "Генерувати QR-коди"
          operation: "qrcode"
          link: "/signature/net/qrcode/pdf/"
          description: "Генеруйте QR-коди для підписання документів"
          
        # operation loop 6
        - name: "Цифрові сертифікати"
          operation: "digital"
          link: "/signature/net/digital/pdf/"
          description: "Захистіть бізнес і підписуйте документи за допомогою цифрових сертифікатів"

        # operation loop 7
        - name: "Печатки підписів"
          operation: "stamp"
          link: "/signature/net/stamp/pdf/"
          description: "Використовуйте Конструктор печаток для створення індивідуальних круглих або квадратних печаток"
          
        # operation loop 8
        - name: "Шукати підписи"
          operation: "search"
          link: "/signature/net/search/pdf/"
          description: "Знаходьте будь-які попередньо додані підписи в документі"
          
        # operation loop 9
        - name: "Перевірка підписів"
          operation: "verify"
          link: "/signature/net/verify/pdf/"
          description: "Перевіряйте автентичність підписів після їхнього застосування"
          
        # operation loop 10
        - name: "Змінювати підписи"
          operation: "modify"
          link: "/signature/net/modify/pdf/"
          description: "Редагуйте різноманітні підписи в документі"
          
        # operation loop 11
        - name: "Видалити підписи"
          operation: "delete"
          link: "/signature/net/delete/pdf/"
          description: "Видаляйте широкий спектр раніше застосованих підписів"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Підписуйте документи в різних форматах"
    exclude: "PDF"
    description: "API .NET надає можливість обробки понад 60 різних форматів. Ви можете безперешкодно створювати та вбудовувати різноманітні підписи на будь-якій сторінці, застосовувати цифрові сертифікати для безпеки вмісту та ефективно керувати існуючими підписами в документі."
    items: 
          
        # format loop 1
        - name: "Захистити PDF"
          format: "PDF"
          link: "/signature/net/digital/pdf/"
          description: "Адріс фільмування документів Adobe"
          
        # format loop 2
        - name: "Захистити DOCX"
          format: "DOCX"
          link: "/signature/net/digital/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 3
        - name: "Захистити PPTX"
          format: "PPTX"
          link: "/signature/net/digital/pptx/"
          description: "Презентація PowerPoint Open XML"
          
        # format loop 4
        - name: "Захистити XLSX"
          format: "XLSX"
          link: "/signature/net/digital/xlsx/"
          description: "Електронна таблиця Microsoft Excel Open XML"


          

---