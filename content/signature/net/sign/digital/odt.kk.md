---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Odt
productName: .NET
lang: kk
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Odt for C#

############################# Head ############################
head_title: "C# көмегімен Odt файлына сандық электрондық қолтаңбаларды қосу"
head_description: "Кодтың бірнеше жолын пайдаланып, .NET үшін Odt файлына Цифрлық қолтаңба қойыңыз. Ондаған файл пішіміне қол қою үшін GroupDocs Document Signature API пайдаланыңыз."

############################# Header ############################
title: "C# жүйесінде Digital қолтаңбалары бар eSign Odt файлдары"
description: ".NET кодының бірнеше жолы бар Digital қолтаңбасын қалай қосуға болады"
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
    title: "GroupDocs.Signature for .NET Сандық қолтаңбалар API туралы"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) — цифрлық электрондық қолтаңбасы бар құжаттарды цифрлық сертификаттармен ресімдеуге арналған танымал API. Сандық қолтаңбалар үшін API құпия сөзбен қорғалған жеке және ашық кілттермен құжатты жасау үшін PFX сертификат файлдарын пайдаланады. Сандық қолтаңбалар eSign PDF арнайы бетімен іскери құжаттарды куәландыру, Words, Excel, Powerpoint файлдары және Open Office құжаттары сияқты бүкіл Microsoft Office құжаттарын куәландыру үшін пайдаланылуы мүмкін. Тұтынушылар қолтаңбаларды өңдеу, жою немесе реттеу сияқты оңай басқара алады. API қолтаңбаларды іздеу және тексеру жолын қамтамасыз етеді. Сонымен қатар, қолтаңбаларды теңшеуге арналған көптеген мүмкіндіктер қарастырылған.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# жүйесінде Digital арқылы Odt файлына қол қою қадамдары"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) Odt құжаттарға Digital қолтаңбаларымен жылдам және оңай қол қою мүмкіндігін береді.
        
        * Жол немесе жад ағыны ретінде қол қойылатын Odt файлын қамтамасыз ететін Signature класының данасын жасаңыз
        * SignOptions сыныбын жасаңыз және барлық қажетті деректерді орнатыңыз.
        * Odt шығыс файлын немесе жад ағынын беретін Signature.Sign() әдісін шақырыңыз

    title_right: " Жүйе талаптары"
    content_right: |
        GroupDocs.Signature for .NET барлық негізгі платформалар мен операциялық жүйелерде қолдау көрсетеді. Төмендегі кодты орындамас бұрын, жүйеде келесі алғышарттар орнатылғанына көз жеткізіңіз.

        * Операциялық жүйелер: Microsoft Windows, Linux, MacOS
        * Әзірлеу орталары: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ең соңғы GroupDocs.Signature for .NET нұсқасын [Nuget](https://www.nuget.org/packages/groupdocs.signature) алыңыз.
         
    code: |
        ```csharp    
                
        // Set up input Odt file
        string filePath = "input.odt";
        // Set up output file
        string outputFilePath = "output.odt";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Odt document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Odt құжаттарға Digital тікелей көрсетілімі арқылы қол қою"
    content: |
       Дәл қазір [GroupDocs.Signature қолданбасы](https://products.groupdocs.app/signature/family) веб-сайтына кіру арқылы әртүрлі қолтаңбалармен Odt файлына қол қойыңыз. Тегін онлайн демонстрация сізді күтуде.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# үшін басқа қолдау көрсетілетін Digital қолтаңбалары"
    content: |
        "Odt қолтаңбасының басқа түрлерімен де қол қоюға болады. Төмендегі тізімді қараңыз."
    format: 
       
       
back_to_top:
    enable: true
---