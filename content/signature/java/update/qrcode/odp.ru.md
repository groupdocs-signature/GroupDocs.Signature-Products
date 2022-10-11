---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Qrcode
fileformat: Odp
productName: Java
lang: ru
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Odp for Java

############################# Head ############################
head_title: "Обновите подписи Qrcode, размещенные в файлах Odp, с помощью Java"
head_description: "Используйте простой и понятный код Java для обновления подписей Qrcode в подписанных документах Odp."

############################# Header ############################
title: "Редактировать и обновлять подписи Qrcode, размещенные в файлах Odp"
description: "API для Java предоставляет функциональные возможности для обновления подписей Qrcode в документах Odp. Быстро и легко обновляйте электронные подписи внутри ваших документов Odp с помощью пары строк кода Java."
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
    title: "Узнайте о возможностях API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) Функциональность API содержит широкий выбор средств для обработки востребованных форматов документов с использованием электронных подписей. Поддерживается широкий спектр электронных подписей, таких как тексты, изображения, цифровые сертификаты, штрих-коды, QR-коды, штампы или метаданные. Клиенты могут добавлять, удалять, редактировать, проверять или искать цифровые подписи в PDF-файлах, документах MS Word, книгах MS Excel, презентациях MS PowerPoint, файлах Adobe Photoshop и различных форматах изображений. Доступны многочисленные полезные функции и настройки.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Как изменить подписи Qrcode в документе Odp"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) содержит полезные функции, такие как обновление подписей Qrcode, размещенных в документах Odp. Это позволяет изменять функции подписи без дополнительного кода.
        
        * Для начала создайте объект Signature, передав в качестве параметра конструктора путь к документу, который предполагается обновить.
        * Затем создайте экземпляр соответствующего конкретного объекта подписи и настройте его идентификатор и свойства, которые необходимо изменить.
        * Наконец, вызовите метод Update подписи, передав конкретный объект подписи.
        * Обработайте результаты обновления до вашего уведомления.

    title_right: "Системные Требования"
    content_right: |
        GroupDocs.Signature for Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.

        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Загрузите последнюю версию GroupDocs.Signature for Java из [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Odp file
        String filePath = "input.odp";
        // Set up output file
        String outputFilePath = "output.odp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        QrCodeSignature signatureToUpdate = new QrCodeSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(200);
        // specify signature height
        signatureToUpdate.setHeight(200);
        // set left position
        signatureToUpdate.setLeft(120);
        // set top position
        signatureToUpdate.setTop(160);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Обновление подписей Qrcode на страницах документа — интерактивная демонстрация"
    content: |
       Редактируйте различные электронные подписи документа Odp прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Обновите различные подписи Qrcode через Java"
    content: |
        "Редактирование цифровых подписей, размещенных в различных форматах документов. Обновление данных подписей без дополнительного кода."
    format: 
       
       
back_to_top:
    enable: true
---