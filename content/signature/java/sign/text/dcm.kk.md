---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Dcm
productName: Java
lang: kk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Dcm for Java

############################# Head ############################
head_title: "Java көмегімен Dcm файлына мәтіндік электрондық қолтаңба жасау"
head_description: "Кодтың бірнеше жолын пайдаланып Java үшін Text eSignature Dcm файлына қойыңыз. Ондаған файл пішіміне қол қою үшін GroupDocs Document Signature API пайдаланыңыз."

############################# Header ############################
title: "Dcm файлдарға Java жүйесінде Text қолтаңбаларымен қол қойыңыз"
description: "Text Java кодының бірнеше жолы бар қолтаңбаны қалай қосуға болады"
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
    title: "GroupDocs.Signature for Java API туралы"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) — цифрлық құжаттарға электрондық қол қоюға арналған танымал API. Мәтіндер, суреттер, цифрлық сертификаттар, штрих-кодтар, QR-кодтар, мөрлер немесе метадеректер сияқты қолтаңбалар бар. Қолтаңбалар PDF файлдарына, MS Word құжаттарына, MS Excel жұмыс кітаптарына, MS PowerPoint презентацияларына, Adobe Photoshop файлдарына және әртүрлі кескін пішімдеріне қойылуы мүмкін. Тұтынушылар өз құжатына қол қоя алады және сол құжаттарға қойылған электрондық қолтаңбаларды жаңартуға, іздеуге, тексеруге, жоюға немесе алдын ала қарауға болады. Сонымен қатар, қолтаңбаларды теңшеуге арналған көптеген мүмкіндіктер қарастырылған.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java жүйесінде Text арқылы Dcm файлына қол қою қадамдары"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) Dcm құжаттарға Text қолтаңбаларымен жылдам және оңай қол қою мүмкіндігін береді.
        
        * Жол немесе жад ағыны ретінде қол қойылатын Dcm файлын қамтамасыз ететін Signature класының данасын жасаңыз
        * SignOptions сыныбын жасаңыз және барлық қажетті деректерді орнатыңыз.
        * Dcm шығыс файлын немесе жад ағынын беретін Signature.Sign() әдісін шақырыңыз

    title_right: " Жүйе талаптары"
    content_right: |
        GroupDocs.Signature for Java барлық негізгі платформалар мен операциялық жүйелерде қолдау көрсетеді. Төмендегі кодты орындамас бұрын, жүйеде келесі алғышарттар орнатылғанына көз жеткізіңіз.

        * Операциялық жүйелер: Microsoft Windows, Linux, MacOS
        * Әзірлеу орталары: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Ең соңғы GroupDocs.Signature for Java нұсқасын [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) алыңыз.
         
    code: |
        ```java    
                
        // Set up input Dcm file
        String filePath = "input.dcm";
        // Set up output file
        String outputFilePath = "output.dcm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Dcm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Dcm құжаттарға Text тікелей көрсетілімі арқылы қол қою"
    content: |
       Дәл қазір [GroupDocs.Signature қолданбасы](https://products.groupdocs.app/signature/family) веб-сайтына кіру арқылы әртүрлі қолтаңбалармен Dcm файлына қол қойыңыз. Тегін онлайн демонстрация сізді күтуде.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java үшін басқа қолдау көрсетілетін Text қолтаңбалары"
    content: |
        "Dcm қолтаңбасының басқа түрлерімен де қол қоюға болады. Төмендегі тізімді қараңыз."
    format: 
       
       
back_to_top:
    enable: true
---