---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Ods
productName: .NET
lang: kk
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Ods for C#

############################# Head ############################
head_title: "C# арқылы Ods құжаттарына метадеректер электрондық қолтаңбаларын қосыңыз"
head_description: "Метадеректерді C# кодының бірнеше жолын пайдаланып Ods құжаттарыңыздың ішінде жасырын электрондық қолтаңба ретінде пайдаланыңыз. Метадеректер ақпаратымен іскери құжаттар мен файлдарға электрондық қол қою үшін GroupDocs құжат қолтаңбасының API интерфейсін пайдаланыңыз."

############################# Header ############################
title: ".NET арқылы Ods құжатына арналған метадеректер электрондық қолтаңбалары қарапайым және пайдалану оңай!"
description: "Жасырын метадеректер жазбалары бар Ods құжаттарыңыз бен келісім-шарттарыңызға esign. PDF файлдары, MS Word құжаттары, MS Excel жұмыс кітаптары, MS PowerPoint көрсетілімдері және әртүрлі кескін пішімдері үшін еш қиындықсыз және қосымша кодтаусыз метадеректер жасаңыз."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET метадеректер қолтаңбалары API туралы"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) — цифрлық құжаттарға электрондық қол қоюға арналған танымал API. Мәтіндер, суреттер, цифрлық сертификаттар, штрих-кодтар, QR-кодтар, мөрлер немесе метадеректер сияқты қолтаңбалар бар. Қолтаңбалар PDF файлдарына, MS Word құжаттарына, MS Excel жұмыс кітаптарына, MS PowerPoint презентацияларына, Adobe Photoshop файлдарына және әртүрлі кескін пішімдеріне қойылуы мүмкін. Тұтынушылар өз құжатына қол қоя алады және сол құжаттарға қойылған электрондық қолтаңбаларды жаңартуға, іздеуге, тексеруге, жоюға немесе алдын ала қарауға болады. Сонымен қатар, қолтаңбаларды теңшеуге арналған көптеген мүмкіндіктер қарастырылған.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# жүйесінде Metadata арқылы Ods файлына қол қою қадамдары"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) Ods құжаттарға Metadata қолтаңбаларымен жылдам және оңай қол қою мүмкіндігін береді.
        
        * Жол немесе жад ағыны ретінде қол қойылатын Ods файлын қамтамасыз ететін Signature класының данасын жасаңыз
        * SignOptions сыныбын жасаңыз және барлық қажетті деректерді орнатыңыз.
        * Ods шығыс файлын немесе жад ағынын беретін Signature.Sign() әдісін шақырыңыз

    title_right: " Жүйе талаптары"
    content_right: |
        GroupDocs.Signature for .NET барлық негізгі платформалар мен операциялық жүйелерде қолдау көрсетеді. Төмендегі кодты орындамас бұрын, жүйеде келесі алғышарттар орнатылғанына көз жеткізіңіз.

        * Операциялық жүйелер: Microsoft Windows, Linux, MacOS
        * Әзірлеу орталары: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ең соңғы GroupDocs.Signature for .NET нұсқасын [Nuget](https://www.nuget.org/packages/groupdocs.signature) алыңыз.
         
    code: |
        ```csharp    
        
        // Set up input Ods file
        string filePath = "input.ods";
        // Set up output file
        string outputFilePath = "output.ods";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Ods document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ods құжаттарға Metadata тікелей көрсетілімі арқылы қол қою"
    content: |
       Дәл қазір [GroupDocs.Signature қолданбасы](https://products.groupdocs.app/signature/family) веб-сайтына кіру арқылы әртүрлі қолтаңбалармен Ods файлына қол қойыңыз. Тегін онлайн демонстрация сізді күтуде.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# үшін басқа қолдау көрсетілетін Metadata қолтаңбалары"
    content: |
        "{{Файл пішімі}} қолтаңбасының басқа түрлерімен де қол қоюға болады. Төмендегі тізімді қараңыз."
    format: 
       
       
back_to_top:
    enable: true
---