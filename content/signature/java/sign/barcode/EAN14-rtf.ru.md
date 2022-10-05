---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: E A N14
fileformat: Rtf
productName: Java
lang: ru
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Rtf for Java

############################# Head ############################
head_title: "eSign Rtf документ со штрих-кодом E A N14 в Java"
head_description: "Создайте подпись штрих-кода E A N14 и поместите ее в документ Rtf с Java, используя пару строк кода. Используйте API подписи документов GroupDocs для подписи файлов различных форматов."

############################# Header ############################
title: "Создайте подпись штрих-кода E A N14 для документа Rtf в Java"
description: "Подпишите свои бизнес-документы Rtf с помощью штрих-кода E A N14. Быстро и легко создавайте подпись штрих-кода с помощью нескольких строк кода для настройки параметров подписи."
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
    title: "{barcode-about.title}"
    content: |
        {barcode-about.content}
    

############################# Steps ############################
steps:
    enable: true
    title_left: "{barcode-steps.title}"
    content_left: |
        {barcode-steps.content.description}
        
        * {barcode-steps.content.step_1}
        * {barcode-steps.content.step_2}
        * {barcode-steps.content.step_3}

    title_right: " {system-requirements.title}"
    content_right: |
        {system-requirements.content.description}

        * {system-requirements.content.step_1}
        * {system-requirements.content.step_2}
        * Java runtime: J2SE 6.0 and above
        * {system-requirements.content.step_3}
         
    code: |
        ```java    
                
        // Set up input Rtf file
        String filePath = "input.rtf";
        // Set up output file
        String outputFilePath = "output.rtf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.E A N14);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Rtf document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Подписание Rtf документов с помощью Barcode Live Demo"
    content: |
       Подпишите файл Rtf с различными подписями прямо сейчас, посетив веб-сайт [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Бесплатная онлайн-демонстрация ждет вас.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About E A N14 Barcode"
          content: |
            Европейский номер статьи или EAN — это стандарт, описывающий символику штрих-кода и систему нумерации, используемую в мировой торговле для идентификации определенного типа розничного продукта в конкретной конфигурации упаковки от конкретного производителя.
          characterset: |
             Числовые цифры (0-9) и специальные символы.
          textcapacity: |
             Ровно 14 цифр.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Другие поддерживаемые подписи Barcode для Java"
    content: |
        "Вы также можете подписать Rtf другими типами подписи. См. список ниже."
    format: 
        
       
back_to_top:
    enable: true
---