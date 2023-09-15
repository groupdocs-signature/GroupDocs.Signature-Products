---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:23
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, хмарні API та онлайн-додатки для підпису документів"
head_description: "Отримайте комплексне рішення електронного підпису документів для .NET, Java і хмарних програм. Підписуйте стандартні формати документів онлайн за допомогою простої функції перетягування"

############################# Header ############################
title: "Підписувати документи<br>через .NET API"
description: "Підписуйте цифрові документи та зображення на будь-якій платформі за допомогою наших гнучких API та рішень на основі програм для програмістів і кінцевих користувачів."
words:
  for: "для"

actions:
  main: "Безкоштовне завантаження NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Готові почати?"
  description: "Спробуйте функції GroupDocs.Signature безкоштовно або подайте запит на ліцензію"

release:
  title: "Випущено версію {0}"
  notes: "Подивіться, що нового"
  downloads: "Завантаження"

code:
  title: "Підписуйте PDF-файли на C#"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Виберіть документ PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Надайте текст
        var options = new TextSignOptions("John Smith")
        {
            // Встановити колір
            ForeColor = Color.Red
        };
        // Підпишіть документ і збережіть його у файлі
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Огляд GroupDocs.Signature"
  description: "API для підписання документів і пов’язаних операцій у програмах .NET"
  features:
    # feature loop
    - title: "Додавання підписів до ділових документів на C#"
      content: "Підпис документів: за допомогою GroupDocs.Signature для .NET ви можете додавати різні типи підписів, як-от текст, зображення, штрих-коди та цифрові сертифікати, до документів PDF і Office. Цей API дозволяє підписувати документи майже будь-яким типом даних, у тому числі прихованими метаданими."

    # feature loop
    - title: "Оформлення підписаних документів"
      content: "Додаткова обробка: ви можете виконувати потужні операції з підписаними документами за допомогою GroupDocs.Signature. Це включає пошук наявних підписів у бізнес-документах та їх перевірку за певними критеріями. Крім того, ви можете отримувати інформацію про документ і переглядати сторінки за допомогою цього API .NET."

    # feature loop
    - title: "Налаштування результатів"
      content: "GroupDocs.Signature для .NET пропонує широкі можливості налаштування. Ви можете точно розташувати підписи будь-де на сторінці документа та налаштувати їх зовнішній вигляд за допомогою різноманітних параметрів. Крім того, цей API підтримує збереження оброблених документів у широкому діапазоні підтримуваних форматів."

############################# Platforms ############################
platforms:
  enable: true
  title: "Незалежність від платформи"
  description: "GroupDocs.Signature для .NET підтримує такі операційні системи, фреймворки та менеджери пакетів"
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
    GroupDocs.Signature для .NET підтримує операції з такими [форматами файлів](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Підписуйте PDF-файли, документи Office і зображення швидко й точно"

  items:
    # feature loop
    - icon: "sign"
      title: "Підписання документа"
      content: "Точно додайте один або кілька підтримуваних типів підписів у будь-яку вказану позицію ділових документів."

    # feature loop
    - icon: "custom"
      title: "Налаштувати підписи"
      content: "Використовуйте такі функції, як колір, шрифт, рамка, поворот тощо, щоб налаштувати вигляд підписів."

    # feature loop
    - icon: "password"
      title: "Захист документів паролем"
      content: "Захистіть певні типи документів, встановивши пароль після підписання."

    # feature loop
    - icon: "protect"
      title: "Захист від змін"
      content: "Запобігайте змінам важливих ділових документів після додавання підпису за допомогою цифрового сертифіката."

    # feature loop
    - icon: "convert"
      title: "Перетворення підписаних файлів в інші формати"
      content: "Перетворіть підписані файли у потрібні формати, наприклад збережіть документ Word у форматі PDF."

    # feature loop
    - icon: "preview"
      title: "Витягти попередній перегляд сторінки"
      content: "Витягуйте сторінки з підписаних документів як окремі зображення для подальшої обробки."

    # feature loop
    - icon: "search"
      title: "Пошук підпису в документах"
      content: "Отримати інформацію про раніше додані підписи в певних документах."

    # feature loop
    - icon: "validate"
      title: "Перевірте підписані документи"
      content: "Перевірте належне підписання документів за допомогою функцій перевірки."

    # feature loop
    - icon: "update"
      title: "Оновіть або видаліть підписи"
      content: "Легко змінюйте розташування певних підписів на сторінці, змінюйте їхній текст або видаляйте їх без проблем."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Зразки коду"
  description: "Деякі випадки використання типових GroupDocs.Signature для операцій .NET"
  items:
    # code sample loop
    - title: "Додати QR-код до PDF"
      content: |
        Додавання [QR-кодів](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) до певних сторінок PDF-документів може покращити бізнес-процеси. Нижче наведено приклад того, як додати QR-код за допомогою GroupDocs.Signature.
        {{< landing/code title="Як вставити QR-код у PDF.">}}
        ```csharp {style=abap}
        // Завантажте документ для підпису
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Створіть параметри QR-коду з попередньо визначеним текстом
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Налаштуйте тип кодування QR-коду та положення на сторінці
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Підпишіть документ і збережіть його як файл результату
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Захист документа DOCX за допомогою цифрового сертифіката"
      content: |
        Ви можете [захистити документ](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) за допомогою особистих або корпоративних підписів, які зберігаються як цифрові сертифікати. Такі захищені документи не можна змінити без визнання підпису недійсним.
        {{< landing/code title="Ось як забезпечити цілісність документа.">}}
        ```csharp {style=abap}   
        // Завантажте документ для цифрового підпису
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Укажіть параметри цифрового підпису та вкажіть шлях до файлу сертифіката
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Встановіть пароль сертифіката
                Password = "1234567890"
            };
            // Підпишіть документ і збережіть його в потрібному місці
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
