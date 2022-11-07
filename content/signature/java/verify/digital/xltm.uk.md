---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Xltm
productName: Java
lang: uk
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xltm for Java

############################# Head ############################
head_title: "Перевірка підписів Digital для файлів Xltm через Java"
head_description: "Використовуйте лише кілька рядків коду Java, щоб перевірити документи Xltm та їхні підписи Digital."

############################# Header ############################
title: "Перевірка підписів Digital для файлів Xltm"
description: "API для Java надає можливість перевіряти підписи Digital у документах Xltm. Перевірку електронних підписів у ваших документах Xltm можна виконати швидко та легко."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Відкрийте для себе нові функції API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API надає широкий спектр способів обробки багатьох форматів документів за допомогою електронних підписів. Підтримується багато типів цифрових підписів, таких як тексти, зображення, цифрові сертифікати, штрих-коди, QR-коди, штампи або метадані. Клієнти можуть додавати, видаляти, редагувати, перевіряти або шукати цифрові підписи в PDF-файлах, документах MS Word, робочих книгах MS Excel, презентаціях MS PowerPoint, файлах Adobe Photoshop і різних форматах зображень. Доступна вражаюча кількість додаткових функцій і налаштувань.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Як перевірити підписи Digital у вашому документі Xltm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) містить такі корисні функції, як перевірка підписів Digital, розміщених у документах Xltm. Скористайтеся цією можливістю без впровадження додаткового коду.
        
        * По-перше, створіть екземпляр класу підпису, надавши як шлях параметра конструктора до документа, який має бути перевірений.
        * По-друге, створіть новий об’єкт VerifyOptions і налаштуйте всі необхідні властивості.
        * Нарешті, викликайте метод Verify об’єкта Signature, передаючи екземпляр VerifyOptions.
        * Потім обробіть результати перевірки.

    title_right: "Системні вимоги"
    content_right: |
        GroupDocs.Signature for Java підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.

        * Операційні системи: Microsoft Windows, Linux, MacOS
        * Середовища розробки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Завантажте останню версію GroupDocs.Signature for Java з [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xltm file
        String filePath = "input.xltm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Підписання за допомогою підписів Digital Демо"
    content: |
       Додайте різні електронні підписи до файлу Xltm просто зараз, відвідавши веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Перевірте інші підписи Digital за допомогою Java"
    content: |
        "Перевірка електронного підпису в різних документах. Перевірте якість підписів у популярних форматах файлів, як показано нижче."
    format: 
       
       
back_to_top:
    enable: true
---