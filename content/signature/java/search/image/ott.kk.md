---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Ott
productName: Java
lang: kk
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Ott with Java

############################# Head ############################
head_title: "Image қолтаңбаларды Java ішіндегі Ott файлынан іздеңіз"
head_description: "Кодтың бірнеше жолын пайдаланып Ott файлдарында Image қолтаңбаларын іздеу үшін Java пайдаланыңыз."

############################# Header ############################
title: "Ott файлынан Image қолтаңбаларын іздеңіз"
description: "Java жергілікті API бұрыннан қол қойылған Ott файлдарындағы Image қолтаңбаларын іздеуге мүмкіндік береді. Кодтың бірнеше жолын пайдаланып {{Файл пішімі}} құжаттарыңызда кеңейтілген электрондық қолтаңбаны іздеуді орындаңыз."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java API туралы"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) мәтіндер, кескіндер, сандық сертификаттар, штрих-кодтар, QR-кодтар, мөрлер немесе метадеректер сияқты әртүрлі қолтаңба түрлерін пайдаланып құжаттарды өңдеуге арналған Java API ұсынады. Пайдаланушылар қажет болған жағдайда қолтаңбалар сипаттарын теңшеуге қосымша қолдау көрсете отырып, PDF файлдары, MS Word құжаттары, MS Excel жұмыс кітаптары, MS PowerPoint презентациялары, Adobe Photoshop файлдары және әртүрлі кескін пішімдері ішінде электрондық қолтаңбаларды қоса алады, жояды, жаңартады, тексере алады немесе іздей алады.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Ott ішінде Image қолтаңбаларын қалай іздеу керек"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) Java әзірлеушілеріне бірнеше оңай қадамдарды орындау арқылы қолданбаларынан Ott файлдарындағы Image қолтаңбаларды іздеуді жеңілдетеді.
        
        * Signature сыныбының жаңа данасын жасаңыз және бастапқы құжат жолын конструктор параметрі ретінде өткізіңіз.
        * Талаптарыңызға сәйкес SearchOptions нысанын жасаңыз және іздеу опцияларын көрсетіңіз.
        * Signature класының данасы іздеу әдісіне қоңырау шалыңыз және оған SearchOptions өткізіңіз.
        * Сіздің сұраныстарыңызға сәйкес іздеу нәтижелерін өңдеңіз.

    title_right: "Жүйе талаптары"
    content_right: |
        GroupDocs.Signature for Java барлық негізгі платформалар мен операциялық жүйелерде қолдау көрсетеді. Төмендегі кодты орындамас бұрын, жүйеде келесі алғышарттар орнатылғанына көз жеткізіңіз.

        * Операциялық жүйелер: Microsoft Windows, Linux, MacOS
        * Әзірлеу орталары: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * GroupDocs.Signature for Java соңғы нұсқасын [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) ішінен жүктеп алыңыз.
         
    code: |
        ```java    
                
        // Set up input Ott file
        String filePath = "input.ott";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        ImageSearchOptions options = new ImageSearchOptions();

        // set minimum size if needed 
        options.setMinContentSize(100);
        // set maximum image size if needed
        options.setMaxContentSize(2000);
        // return images for processing
        options.setReturnContent(true);
        // set up type of returned images
        options.setReturnContentType(FileType.PNG);

        // search for Image signatures in Ott document
        List<ImageSignature> signatures = signature.search(ImageSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Image электрондық қолтаңбаларды Live Demo іздеңіз"
    content: |
       Дәл қазір [GroupDocs.Signature қолданбасы](https://products.groupdocs.app/signature/family) веб-сайтына кіру арқылы Ott файлдарына әртүрлі электрондық қолтаңбаларды құжаттан іздеңіз.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Java арқылы басқа Image қолтаңбаларын іздеңіз"
    content: |
        "Электрондық қолтаңбалар әртүрлі құжаттарда іздейді. Төменде көрсетілгендей танымал файл пішімдерінің бірінен қолтаңбаларды табыңыз."
    format: 
           
       
back_to_top:
    enable: true
---