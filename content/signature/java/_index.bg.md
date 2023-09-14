---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:21
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
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, облачни API и онлайн приложения за подписване на документи"
head_description: "Вземете цялостно решение за електронен подпис на документи за .NET, Java и базирани на облак приложения. Подписвайте обичайните формати на документи онлайн с помощта на проста функция за плъзгане и пускане"

############################# Header ############################
title: "Подписвайте документи<br>чрез Java API"
description: "Подписвайте цифрови документи и изображения на всяка платформа, като използвате нашите гъвкави API и базирани на приложения решения за програмисти и крайни потребители."
words:
  for: "за"

actions:
  main: "Безплатно изтегляне на Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Лицензиране"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Готови ли сте да започнете?"
  description: "Изпробвайте функциите на GroupDocs.Signature безплатно или поискайте лиценз"

release:
  title: "Пусната е версия {0}"
  notes: "Вижте какво ново"
  downloads: "Изтегляния"

code:
  title: "Подписвайте PDF файлове в Java"
  more: "Още примери"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Изберете PDF документ
    Signature signature = new Signature("sample.pdf");
    
    // Въведете текст
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Подпишете документа и го запазете във файл
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Преглед на GroupDocs.Signature"
  description: "API за извършване на подписване на документи и свързани операции в Java приложения"
  features:
    # feature loop
    - title: "Подобрени бизнес документи с цифрови подписи в Java"
      content: "Бързо подписване с възможност за персонализиране: GroupDocs.Signature за Java предлага широка гама от опции за цифров подпис за PDF файлове, изображения и документи на Office. Можете да използвате текст, баркодове, QR-кодове, цифрови сертификати, снимки или скрити метаданни. Обработката на документи е бърза и ефективна."

    # feature loop
    - title: "Манипулиране на подписани документи"
      content: "Разширената обработка на документи включва мощни операции върху подписани документи с помощта на GroupDocs.Signature за Java. Можете да търсите и валидирате подписи, които са добавени към бизнес документи, като използвате различни полезни критерии. Освен това можете да получите достъп до подробна информация за документа или да получите изображения за визуализация на страниците му."

    # feature loop
    - title: "Разнообразие от възможности за избор на изход"
      content: "Стабилните опции за подписване ви позволяват да персонализирате изхода за документи, подписани с GroupDocs.Signature за Java. Можете точно да позиционирате всеки подпис на всяка страница на документ и да конфигурирате външния му вид по различни начини. Java API поддържа запазване на подписани бизнес документи в множество поддържани формати и предоставя опции за защитата им с пароли."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимост на платформата"
  description: "GroupDocs.Signature за Java поддържа следните операционни системи, рамки и мениджъри на пакети"
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
  title: "Поддържани файлови формати"
  description: |
    GroupDocs.Signature за Java поддържа операции със следните [файлови формати](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  description: "Подписване на PDF файлове, Office документи и изображения с цифрови подписи"

  items:
    # feature loop
    - icon: "sign"
      title: "Добавяне на подписи"
      content: "Подпишете документ, като използвате различни поддържани типове подписи, като поставите цифров подпис точно на всяка позиция на всяка страница."

    # feature loop
    - icon: "custom"
      title: "Персонализиране на резултатите"
      content: "Персонализирайте външния вид на подписа, като коригирате цвят, шрифт, рамка, ротация и други функции, за да постигнете желания резултат."

    # feature loop
    - icon: "password"
      title: "Защита на документи с парола"
      content: "За много поддържани типове документи можете да защитите подписания документ с парола."

    # feature loop
    - icon: "protect"
      title: "Предотвратяване на неоторизирани промени"
      content: "Защитете важни бизнес документи, подписани с цифров сертификат, от неоторизирани модификации."

    # feature loop
    - icon: "convert"
      title: "Получаване на резултати в желани формати"
      content: "Получавайте лесно подписани файлове с резултати във всеки поддържан формат. Можете също така да конвертирате MS Word документи в PDF без усилие."

    # feature loop
    - icon: "preview"
      title: "Визуализация на документа"
      content: "Запазете всяка страница от документ като изображение за бъдеща обработка."

    # feature loop
    - icon: "search"
      title: "Търсене на подписи"
      content: "Възможно е да получите информация за предварително добавени подписи в конкретни документи."

    # feature loop
    - icon: "validate"
      title: "Валидиране на документи"
      content: "Потвърдете правилността на подписите върху всеки подписан документ."

    # feature loop
    - icon: "update"
      title: "Управление на подписи"
      content: "След като подписът е поставен върху страница на документ, той може да бъде изтрит, преместен или актуализиран, ако е необходимо."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примерни кодове"
  description: "Някои случаи на употреба на типични операции на GroupDocs.Signature за Java"
  items:
    # code sample loop
    - title: "Подобрете PDF документ с QR-код"
      content: |
        Подобряването на бизнес процесите чрез добавяне на [QR-кодове](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) към конкретни страници с PDF документи може да бъде ценно. Има пример как да добавите QR код с помощта на GroupDocs.Signature за Java.
        {{< landing/code title="Подобрете PDF документ с QR-код">}}
        ```java {style=abap}
        // Заредете документа за подпис
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Създайте опции за QR код с предварително дефиниран текст
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Конфигурирайте типа и позицията на кодиране на QR код на страницата
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Подпишете документа и го запазете като файл с резултати
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Използвайте цифров подпис, за да защитите DOCX"
      content: |
        Можете да [защитете документ](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/), като използвате лични или корпоративни подписи, съхранени като цифрови сертификати. Документите, защитени със сертификат, не могат да бъдат променяни без анулиране на подписа.
        {{< landing/code title="Използвайте цифров подпис, за да защитите DOCX">}}
        ```java {style=abap}   
        // Заредете документа за цифров подпис
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Посочете опциите за цифрово подписване и предоставете пътя до файла със сертификата
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Задайте парола за сертификата
        options.setPassword("1234567890");

        // Подпишете документа и го запазете в желания път
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
