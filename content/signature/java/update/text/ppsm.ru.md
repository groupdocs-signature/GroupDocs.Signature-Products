---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Ppsm
productName: Java
lang: ru
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Ppsm for Java

############################# Head ############################
head_title: "Обновите подписи Text, размещенные в файлах Ppsm, с помощью Java"
head_description: "Используйте простой и понятный код Java для обновления подписей Text в подписанных документах Ppsm."

############################# Header ############################
title: "Редактировать и обновлять подписи Text, размещенные в файлах Ppsm"
description: "API для Java предоставляет функциональные возможности для обновления подписей Text в документах Ppsm. Быстро и легко обновляйте электронные подписи внутри ваших документов Ppsm с помощью пары строк кода Java."
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
    title_left: "Как изменить подписи Text в документе Ppsm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) содержит полезные функции, такие как обновление подписей Text, размещенных в документах Ppsm. Это позволяет изменять функции подписи без дополнительного кода.
        
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
                
        // Set up input Ppsm file
        String filePath = "input.ppsm";
        // Set up output file
        String outputFilePath = "output.ppsm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        TextSignature signatureToUpdate = new TextSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(130);
        // specify signature height
        signatureToUpdate.setHeight(20);
        // set left position
        signatureToUpdate.setLeft(40);
        // set top position
        signatureToUpdate.setTop(50);
        // set up new text
        signatureToUpdate.setText("Mr. John Smith");

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
    title: "Подписание с помощью подписей Text Live Demo"
    content: |
       Добавьте различные электронные подписи в файл Ppsm прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Обновите различные подписи Text через Java"
    content: |
        "Редактирование цифровых подписей, размещенных в различных форматах документов. Обновление данных подписей без дополнительного кода."
    format: 
       
       
back_to_top:
    enable: true
---