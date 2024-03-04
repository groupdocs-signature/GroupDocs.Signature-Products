---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: bg
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
head_title: ".NET, Java, облачни API и онлайн приложения за подписване на документи"
head_description: "Вземете цялостно решение за електронен подпис на документи за .NET, Java и базирани на облак приложения. Подписвайте обичайните формати на документи онлайн с помощта на проста функция за плъзгане и пускане"

############################# Header ############################
title: "Подписвайте документи<br>с Node.js API"
description: "Подписвайте цифрови документи и изображения на всяка платформа, като използвате нашите гъвкави API и базирани на приложения решения за програмисти и крайни потребители."
words:
  for: "за"

actions:
  main: "Изтеглете от NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Лицензиране"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Готови ли сте да започнете?"
  description: "Изпробвайте функциите на GroupDocs.Signature безплатно или поискайте лиценз"

release:
  title: "Пусната е версия {0}"
  notes: "Вижте какво ново"
  downloads: "Изтегляния"

code:
  title: "Подписване на PDF файлове от Node.js"
  more: "Още примери"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // Изберете PDF документ
    let signature = new Signature("sample.pdf");
    
    // Въведете текст
    let options = new TextSignOptions("John Smith");
    
    // Задайте цвят
    options.ForeColor = Color.Red;
    
    // Подпишете документа и го запазете във файл
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Преглед на GroupDocs.Signature"
  description: "Библиотека за подписване на документи, готова за използване в приложения Node.js"
  features:
    # feature loop
    - title: "Решение за цифрови подписи за бизнес документи с Node.js"
      content: "GroupDocs.Signature for Node.js via Java предлага изчерпателен набор от опции за цифров подпис за PDF, Office документи и изображения. Налични са текст, баркодове, изображения, цифрови сертификати и метаданни. Рационализираната обработка на документи гарантира ефективност."

    # feature loop
    - title: "Разширено манипулиране на подписани документи"
      content: "GroupDocs.Signature ви дава възможност да обработвате подписани документи. Търсете и валидирайте подписи, като използвате различни критерии. Освен това извличайте подробна информация за документа или генерирайте изображения за визуализация на страници."

    # feature loop
    - title: "Разнообразни изходни формати"
      content: "Нашето решение осигурява широк контрол върху изходния формат на подписаните документи. Прецизно позиционирайте подписите на всяка страница и персонализирайте външния им вид. Запазете подписани документи в многобройни поддържани формати и по желание ги защитете с пароли."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимост на платформата"
  description: "GroupDocs.Signature for Node.js via Java извършва обработка на документи с различни операционни системи"
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
    GroupDocs.Signature for Node.js via Java улеснява операциите за [популярните файлови формати](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Характеристики на GroupDocs.Signature"
  description: "Подписвайте PDF файлове, документи на Office и изображения с цифрови подписи"

  items:
    # feature loop
    - icon: "sign"
      title: "Бизнес подписи"
      content: "Използвайте различни типове подписи, за да подписвате документи. Поставете цифрови подписи прецизно на всяка страница."

    # feature loop
    - icon: "custom"
      title: "Персонализиране на външния вид на подписа"
      content: "Персонализирайте визуалните аспекти на подписите, като коригирате цвят, шрифт, граници, ротация и други, за да постигнете желания резултат."

    # feature loop
    - icon: "password"
      title: "Защитени с парола документи"
      content: "За много поддържани формати на документи защитавайте подписаните документи с парола за допълнителна сигурност."

    # feature loop
    - icon: "protect"
      title: "Предотвратяване на неоторизирани модификации"
      content: "Защитете важни бизнес документи, подписани с цифрови сертификати, от неразрешени промени."

    # feature loop
    - icon: "convert"
      title: "Желани изходни формати"
      content: "Получете без усилие подписани документи във всеки поддържан формат. Конвертирайте документи на MS Word в PDF формат с лекота."

    # feature loop
    - icon: "preview"
      title: "Преглед на документи"
      content: "Запазете отделни страници на документи като изображения за бъдещи нужди."

    # feature loop
    - icon: "search"
      title: "Търсене на подпис"
      content: "Извлечете информация за добавени преди това подписи във вашите документи."

    # feature loop
    - icon: "validate"
      title: "Валидиране на документ"
      content: "Проверете автентичността на подписите, представени във всеки документ."

    # feature loop
    - icon: "update"
      title: "Управление на подписите"
      content: "Изтрийте, преместете или модифицирайте всички подписи, поставени на всяка страница на документ."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примерни кодове"
  description: "Илюстративни примери, демонстриращи типични операции на GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Маркирайте PDF с QR кодове"
      content: |
        Включването на [баркодове](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) в конкретни страници на PDF документи може да рационализира бизнес процесите. Този раздел предоставя пример за добавяне на QR код с помощта на GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Как да поставите QR код в PDF.">}}
        ```javascript {style=abap}
        // Заредете документа за подпис
        let signature = new Signature("file_to_sign.pdf");
        
        // Създайте опции за QR код с предварително дефиниран текст
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Конфигурирайте типа и позицията на кодиране на QR код на страницата
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Подпишете документа и го запазете като файл с резултати
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Защита на DOCX с цифров подпис"
      content: |
        [Защитете вашите документи](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) чрез подписи, базирани на цифрови сертификати. Цифровият подпис защитава вашите бизнес документи срещу промяна на съдържанието.
        {{< landing/code title="Ето как да гарантирате целостта на документа.">}}
        ```javascript {style=abap}   
        // Заредете документа за цифров подпис
        let signature = new Signature("file_to_sign.pdf");
        
        // Посочете опциите за цифрово подписване и предоставете пътя до файла със сертификата
        let options = new DigitalSignOptions("certificate.pfx");

        // Задайте парола за сертификата
        options.Password = "1234567890";

        // Подпишете документа и го запазете в желания път
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
