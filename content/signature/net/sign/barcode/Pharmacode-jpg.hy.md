---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Jpg
productName: .NET
lang: hy
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Jpg for C#

############################# Head ############################
head_title: "eSign Jpg փաստաթուղթը Pharmacode շտրիխ կոդով C#-ում"
head_description: "Ստեղծեք Pharmacode շտրիխ կոդի ստորագրություն և դրեք այն Jpg փաստաթղթում .NET-ով` օգտագործելով մի քանի տող կոդ: Օգտագործեք GroupDocs Document Signature API-ը՝ տարբեր ֆայլերի ձևաչափեր ստորագրելու համար:"

############################# Header ############################
title: "Ստեղծեք Pharmacode շտրիխ կոդ ստորագրություն Jpg փաստաթղթի համար C#-ում"
description: "Ստորագրեք ձեր Jpg բիզնես փաստաթղթերը Pharmacode շտրիխ կոդով: Ստեղծեք շտրիխ կոդ ստորագրություն արագ և հեշտությամբ մի քանի տող կոդի միջոցով՝ ստորագրման տարբերակները կարգավորելու համար:"
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
    title: "GroupDocs.Signature for .NET շտրիխ ստորագրությունների API-ի մասին:"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) արագ և հեշտ API է՝ թվային փաստաթղթերի էլեկտրոնային ստորագրումը կառավարելու համար՝ օգտագործելով շտրիխ կոդերի տեսակները, ինչպիսիք են UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN: , ITF14 և շատ ուրիշներ: Հաճախորդները կարող են հեշտությամբ ստեղծել շտրիխ կոդեր, որոնք տրամադրում են պահանջվող տեքստը և տեղադրել դրանք PDF-ի, Microsoft Office Words փաստաթղթերի, Microsoft Office Excel աշխատանքային գրքույկների, MS PowerPoint ներկայացումների, Adobe Photoshop ֆայլերի և պատկերի տարբեր ձևաչափերի վրա: Փաստաթղթերում տեղադրված շտրիխ կոդերը կարող են թարմացվել, որոնվել, ստուգվել, ջնջվել կամ նախադիտվել: Ավելին, շտրիխ կոդերի հարմարեցումն ապահովված է:
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Jpg-ը Barcode-ով C#-ով ստորագրելու քայլեր"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) հնարավորություն է տալիս արագ և հեշտությամբ ստորագրել Jpg փաստաթղթերը Barcode ստորագրություններով:
        
        * Ստեղծեք Signature դասի օրինակ, որը տրամադրում է Jpg ֆայլ, որը պետք է ստորագրվի որպես ճանապարհ կամ հիշողության հոսք
        * Տեղադրեք SignOptions դասը և սահմանեք բոլոր պահանջվող տվյալները:
        * Հրավիրեք Signature.Sign() մեթոդը՝ փոխանցելով ելքային Jpg ֆայլը կամ հիշողության հոսքը

    title_right: " Համակարգի պահանջները"
    content_right: |
        GroupDocs.Signature for .NET-ն աջակցվում է բոլոր հիմնական հարթակներում և օպերացիոն համակարգերում: Նախքան ստորև նշված կոդը գործարկելը, խնդրում ենք համոզվել, որ ձեր համակարգում տեղադրված են հետևյալ նախադրյալները.

        * Օպերացիոն համակարգեր՝ Microsoft Windows, Linux, MacOS
        * Մշակման միջավայրեր՝ Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ստացեք վերջին GroupDocs.Signature for .NET-ը [Nuget]-ից (https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Jpg file
        string filePath = "input.jpg";
        // Set up output file
        string outputFilePath = "output.jpg";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Pharmacode,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Jpg document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Jpg փաստաթղթերի ստորագրում Barcode Live Demo-ով"
    content: |
       Ստորագրեք Jpg ֆայլը տարբեր ստորագրություններով հենց հիմա՝ այցելելով [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) կայքը: Անվճար առցանց ցուցադրություն սպասում է ձեզ:

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode-ը, որը նաև հայտնի է որպես Pharmaceutical Binary Code, շտրիխ կոդերի ստանդարտ է, որն օգտագործվում է դեղագործական արդյունաբերության մեջ որպես փաթեթավորման վերահսկման համակարգ:
          characterset: |
             Թվային թվեր (0-9):
          textcapacity: |
             Ներկայացնում է միայն մեկ ամբողջ թիվ 3-ից մինչև 131070:
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Այլ աջակցվող Barcode ստորագրություններ C#-ի համար"
    content: |
        "Դուք կարող եք նաև ստորագրել Jpg ստորագրության այլ տեսակներով: Խնդրում ենք տեսնել ստորև ներկայացված ցուցակը:"
    format: 
        
       
back_to_top:
    enable: true
---