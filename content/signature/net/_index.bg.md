---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:22
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: bg
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, облачни API и онлайн приложения за подписване на документи"
head_description: "Вземете цялостно решение за електронен подпис на документи за .NET, Java и базирани на облак приложения. Подписвайте обичайните формати на документи онлайн с помощта на проста функция за плъзгане и пускане"

############################# Header ############################
title: "Подписвайте документи<br>чрез .NET API"
description: "Подписвайте цифрови документи и изображения на всяка платформа, като използвате нашите гъвкави API и базирани на приложения решения за програмисти и крайни потребители."
words:
  for: "за"

actions:
  main: "Безплатно изтегляне на NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Лицензиране"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Готови ли сте да започнете?"
  description: "Изпробвайте функциите на GroupDocs.Signature безплатно или поискайте лиценз"

release:
  title: "Пусната е версия {0}"
  notes: "Вижте какво ново"
  downloads: "Изтегляния"

code:
  title: "Подписвайте PDF файлове в C#"
  more: "Още примери"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Изберете PDF документ
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Въведете текст
        var options = new TextSignOptions("John Smith")
        {
            // Задайте цвят
            ForeColor = Color.Red
        };
        // Подпишете документа и го запазете във файл
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Преглед на GroupDocs.Signature"
  description: "API за извършване на подписване на документи и свързани операции в .NET приложения"
  features:
    # feature loop
    - title: "Добавяне на подписи към бизнес документи в C#"
      content: "Подписване на документи: С GroupDocs.Signature за .NET можете да добавяте различни типове подписи, като текст, изображения, баркодове и цифрови сертификати, към PDF и Office документи. Този API ви позволява да подписвате вашите документи с почти всеки тип данни, включително скрити метаданни."

    # feature loop
    - title: "Обработка на подписани документи"
      content: "Допълнителна обработка: Можете да извършвате мощни операции върху подписани документи с помощта на GroupDocs.Signature. Това включва търсене на съществуващи подписи в бизнес документи и проверката им с помощта на специфични критерии. Освен това можете да извличате информация за документа и да визуализирате страници чрез този .NET API."

    # feature loop
    - title: "Персонализиране на резултатите"
      content: "GroupDocs.Signature за .NET предлага обширни опции за персонализиране. Можете прецизно да позиционирате подписите навсякъде на страницата на документа и да коригирате външния им вид с помощта на различни настройки. Освен това този API поддържа запазване на обработени документи в широка гама от поддържани формати."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимост на платформата"
  description: "GroupDocs.Signature за .NET поддържа следните операционни системи, рамки и мениджъри на пакети"
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
  title: "Поддържани файлови формати"
  description: |
    GroupDocs.Signature за .NET поддържа операции със следните [файлови формати](https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office формати
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Изображения и други формати
        * **Преносим:** PDF
        * **Изображения:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Други офис формати:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Други формати
        * **Мрежа:** HTML, MHTML
        * **Архив:** ZIP, TAR, 7Z
        * **Сертификати:** PFX

############################# Features ############################
features:
  enable: true
  title: "Функции на GroupDocs.Signature"
  description: "Подписвайте PDF файлове, Office документи и изображения бързо и точно"

  items:
    # feature loop
    - icon: "sign"
      title: "Подписване на документ"
      content: "Добавете един или няколко поддържани типа подписи точно на всяка определена позиция в бизнес документи."

    # feature loop
    - icon: "custom"
      title: "Персонализиране на подписите"
      content: "Използвайте функции като цвят, шрифт, рамка, ротация и т.н., за да конфигурирате външния вид на подписите."

    # feature loop
    - icon: "password"
      title: "Защита на документа с парола"
      content: "Защитете определени типове документи, като зададете парола след подписване."

    # feature loop
    - icon: "protect"
      title: "Защита от промени"
      content: "Предотвратете промени във важни бизнес документи след добавяне на подпис с цифров сертификат."

    # feature loop
    - icon: "convert"
      title: "Конвертирайте подписани файлове в други формати"
      content: "Конвертирайте подписани файлове в желани формати, като например запазване на Word документ като PDF."

    # feature loop
    - icon: "preview"
      title: "Извличане на визуализации на страници"
      content: "Извличайте страници от подписани документи като отделни изображения за бъдеща обработка."

    # feature loop
    - icon: "search"
      title: "Търсене на подпис в документи"
      content: "Извличане на информация за добавени преди това подписи в конкретни документи."

    # feature loop
    - icon: "validate"
      title: "Валидирайте подписаните документи"
      content: "Проверете правилното подписване на документи с помощта на функции за валидиране."

    # feature loop
    - icon: "update"
      title: "Актуализирайте или изтрийте подписи"
      content: "Лесно препозиционирайте конкретни подписи на страница, модифицирайте техния текст или ги изтрийте без никакви проблеми."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примерни кодове"
  description: "Някои случаи на употреба на типични GroupDocs.Signature за .NET операции"
  items:
    # code sample loop
    - title: "Добавете QR-код към PDF"
      content: |
        Добавянето на [QR-кодове](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) към конкретни страници с PDF документи може да подобри бизнес процесите. По-долу е даден пример как да добавите QR код с помощта на GroupDocs.Signature.
        {{< landing/code title="Как да поставите QR код в PDF.">}}
        ```csharp {style=abap}
        // Заредете документа за подпис
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Създайте опции за QR код с предварително дефиниран текст
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Конфигурирайте типа и позицията на кодиране на QR код на страницата
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Подпишете документа и го запазете като файл с резултати
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Защита на DOCX документ с помощта на цифров сертификат"
      content: |
        Можете да [защитете документ](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/), като използвате лични или корпоративни подписи, съхранени като цифрови сертификати. Такива защитени документи не могат да бъдат модифицирани без обезсилване на подписа.
        {{< landing/code title="Ето как да гарантирате целостта на документа.">}}
        ```csharp {style=abap}   
        // Заредете документа за цифров подпис
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Посочете опциите за цифрово подписване и предоставете пътя до файла със сертификата
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Задайте парола за сертификата
                Password = "1234567890"
            };
            // Подпишете документа и го запазете в желания път
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
