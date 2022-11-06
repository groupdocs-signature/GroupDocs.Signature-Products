---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Jpg
productName: .NET
lang: kk
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Jpg for C#

############################# Head ############################
head_title: "Image қолтаңбаларын Jpg файлына C# арқылы қосу"
head_description: "Кодтың бірнеше жолын пайдаланып, .NET үшін Jpg файлына Image Қолтаңбасын қойыңыз. Ондаған файл пішіміне қол қою үшін GroupDocs Document Signature API пайдаланыңыз."

############################# Header ############################
title: "Jpg файлдарға C# жүйесінде Image қолтаңбаларымен қол қойыңыз"
description: "Image .NET кодының бірнеше жолы бар қолтаңбаны қалай қосуға болады"
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
    title: "GroupDocs.Signature for .NET кескін қолтаңбалары API туралы"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) — цифрлық құжаттарға электрондық қол қоюға арналған танымал API. Мәтіндер, суреттер, цифрлық сертификаттар, штрих-кодтар, QR-кодтар, мөрлер немесе метадеректер сияқты қолтаңбалар бар. Қолтаңбалар PDF файлдарына, MS Word құжаттарына, MS Excel жұмыс кітаптарына, MS PowerPoint презентацияларына, Adobe Photoshop файлдарына және әртүрлі кескін пішімдеріне қойылуы мүмкін. Тұтынушылар өз құжатына қол қоя алады және сол құжаттарға қойылған электрондық қолтаңбаларды жаңартуға, іздеуге, тексеруге, жоюға немесе алдын ала қарауға болады. Сонымен қатар, қолтаңбаларды теңшеуге арналған көптеген мүмкіндіктер қарастырылған.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# жүйесінде Image арқылы Jpg файлына қол қою қадамдары"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) Jpg құжаттарға Image қолтаңбаларымен жылдам және оңай қол қою мүмкіндігін береді.
        
        * Жол немесе жад ағыны ретінде қол қойылатын Jpg файлын қамтамасыз ететін Signature класының данасын жасаңыз
        * SignOptions сыныбын жасаңыз және барлық қажетті деректерді орнатыңыз.
        * Jpg шығыс файлын немесе жад ағынын беретін Signature.Sign() әдісін шақырыңыз

    title_right: " Жүйе талаптары"
    content_right: |
        GroupDocs.Signature for .NET барлық негізгі платформалар мен операциялық жүйелерде қолдау көрсетеді. Төмендегі кодты орындамас бұрын, жүйеде келесі алғышарттар орнатылғанына көз жеткізіңіз.

        * Операциялық жүйелер: Microsoft Windows, Linux, MacOS
        * Әзірлеу орталары: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ең соңғы GroupDocs.Signature for .NET нұсқасын [Nuget](https://www.nuget.org/packages/groupdocs.signature) алыңыз.
         
    code: |
        ```csharp    
                
        // Set up input Jpg file
        string filePath = "input.jpg";
        // Set up output file
        string outputFilePath = "output.jpg";
        // Provide image file
        string imageFilePath = "image.png";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
            //Provide sign options
            ImageSignOptions options = new ImageSignOptions(imageFilePath)
            {
                // set signature position
                Left = 50,
                Top = 200
            };

            // sign Jpg document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Jpg құжаттарға Image тікелей көрсетілімі арқылы қол қою"
    content: |
       Дәл қазір [GroupDocs.Signature қолданбасы](https://products.groupdocs.app/signature/family) веб-сайтына кіру арқылы әртүрлі қолтаңбалармен Jpg файлына қол қойыңыз. Тегін онлайн демонстрация сізді күтуде.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# үшін басқа қолдау көрсетілетін Image қолтаңбалары"
    content: |
        "{{Файл пішімі}} қолтаңбасының басқа түрлерімен де қол қоюға болады. Төмендегі тізімді қараңыз."
    format: 
       
       
back_to_top:
    enable: true
---