---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Image
fileformat: Zip
productName: .NET
lang: kk
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Image signatures at Zip with C#

############################# Head ############################
head_title: "Image қолтаңбаларды C# ішіндегі Zip файлынан іздеңіз"
head_description: "Кодтың бірнеше жолын пайдаланып Zip файлдарында Image қолтаңбаларын іздеу үшін .NET пайдаланыңыз."

############################# Header ############################
title: "Zip файлынан Image қолтаңбаларын іздеңіз"
description: ".NET жергілікті API бұрыннан қол қойылған Zip файлдарындағы Image қолтаңбаларын іздеуге мүмкіндік береді. Кодтың бірнеше жолын пайдаланып Zip құжаттарыңызда кеңейтілген электрондық қолтаңбаны іздеуді орындаңыз."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET API туралы"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) мәтіндер, кескіндер, сандық сертификаттар, штрих-кодтар, QR-кодтар, мөрлер немесе метадеректер сияқты әртүрлі қолтаңба түрлерін пайдаланып құжаттарды өңдеуге арналған .NET API ұсынады. Пайдаланушылар қажет болған жағдайда қолтаңбалар сипаттарын теңшеуге қосымша қолдау көрсете отырып, PDF файлдары, MS Word құжаттары, MS Excel жұмыс кітаптары, MS PowerPoint презентациялары, Adobe Photoshop файлдары және әртүрлі кескін пішімдері ішінде электрондық қолтаңбаларды қоса алады, жояды, жаңартады, тексере алады немесе іздей алады.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Zip ішінде Image қолтаңбаларын қалай іздеу керек"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) .NET әзірлеушілеріне бірнеше оңай қадамдарды орындау арқылы қолданбаларынан Zip файлдарындағы Image қолтаңбаларды іздеуді жеңілдетеді.
        
        * Signature сыныбының жаңа данасын жасаңыз және бастапқы құжат жолын конструктор параметрі ретінде өткізіңіз.
        * Талаптарыңызға сәйкес SearchOptions нысанын жасаңыз және іздеу опцияларын көрсетіңіз.
        * Signature класының данасы іздеу әдісіне қоңырау шалыңыз және оған SearchOptions өткізіңіз.
        * Сіздің сұраныстарыңызға сәйкес іздеу нәтижелерін өңдеңіз.

    title_right: "Жүйе талаптары"
    content_right: |
        GroupDocs.Signature for .NET барлық негізгі платформалар мен операциялық жүйелерде қолдау көрсетеді. Төмендегі кодты орындамас бұрын, жүйеде келесі алғышарттар орнатылғанына көз жеткізіңіз.

        * Операциялық жүйелер: Microsoft Windows, Linux, MacOS
        * Әзірлеу орталары: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * GroupDocs.Signature for .NET соңғы нұсқасын [Nuget](https://www.nuget.org/packages/groupdocs.signature) ішінен жүктеп алыңыз.
         
    code: |
        ```csharp    
                
        // Set up input Zip file
        string filePath = "input.zip";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                ImageSearchOptions options = new ImageSearchOptions()
                {
                    // set minimum size if needed
                    MinContentSize = 100,
                    // set maximum image size if needed
                    MaxContentSize = 2000,                    
                    // return  Image images for processing
                    ReturnContent = true,
                    // set up type of returned  Image images
                    ReturnContentType = FileType.PNG                                 
                };

                // search for Image signatures in Zip document
                List<ImageSignature> signatures = signature.Search<ImageSignature>(options);

                // process signatures which were found                
                foreach (ImageSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Image электрондық қолтаңбаларды Live Demo іздеңіз"
    content: |
       Дәл қазір [GroupDocs.Signature қолданбасы](https://products.groupdocs.app/signature/family) веб-сайтына кіру арқылы Zip файлдарына әртүрлі электрондық қолтаңбаларды құжаттан іздеңіз.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "C# арқылы басқа Image қолтаңбаларын іздеңіз"
    content: |
        "Электрондық қолтаңбалар әртүрлі құжаттарда іздейді. Төменде көрсетілгендей танымал файл пішімдерінің бірінен қолтаңбаларды табыңыз."
    format: 
           
       
back_to_top:
    enable: true
---