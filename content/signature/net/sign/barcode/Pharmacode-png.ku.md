---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Png
productName: .NET
lang: ku
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Png for C#

############################# Head ############################
head_title: "eSign Png belgeya bi Pharmacode Barcode di C#"
head_description: "Îmzeya barkodê ya Pharmacode biafirîne û bi çend rêzikên kodê bi .NET li ser belgeya Png biafirîne. Ji bo îmzekirina cûrbecûr formatên pelan API-ya Îmzekirina Belgeya GroupDocs bikar bînin."

############################# Header ############################
title: "Di C# de ji bo belgeya Pharmacode îmzeya barkodê çêbike"
description: "Belgeyên karsaziya xwe yên {{Pelformat}} bi Pharmacode Barkodê îmze bikin. Bi çend rêzikên kodê re zû û bi hêsanî îmzeya Barkodê biafirînin da ku vebijarkên îmzekirinê saz bikin."
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
    title: "Derbarê GroupDocs.Signature for .NET API-ya îmzeyên barkodê."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) APIyek bilez û hêsan e ku ji bo birêvebirina e-îmzakirina belgeyên dîjîtal bi karanîna cûreyên barkodê yên wekî UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN. , ITF14 û gelekên din. Xerîdar dikarin bi hêsanî Barkodên ku nivîsa pêwîst peyda dikin biafirînin û wan bixin ser PDF, Belgeyên Microsoft Office Words, pirtûkên xebatê yên Microsoft Office Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û formên cûda yên wêneyê. Barkodên ku di belgeyan de têne danîn dikarin bêne nûve kirin, lêgerîn, verastkirin, jêbirin an pêşdîtin. Digel vê yekê, xwerûkirina barkodê tê piştgirî kirin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Gavên îmzekirina Png bi Barcode di C# de"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) îmzakirina belgeyên Png bi îmzeyên Barcode zû û bi hêsanî peyda dike.
        
        * Nimûneyek ji çîna îmzayê biafirîne ku pelê {{Pelformat}} pêşkêş dike ku divê wekî rêyek an herikîna bîranînê were îmzekirin
        * Dersa SignOptions destnîşan bikin û hemî daneyên daxwazkirî bicîh bikin.
        * Rêbaza Signature.Sign() vexwend ku derana pelê {{Pelformat}} an jî herikîna bîrê derbas dike

    title_right: " Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Signature for .NET li ser hemî platform û pergalên xebitandinê yên sereke têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.

        * Pergalên xebitandinê: Microsoft Windows, Linux, MacOS
        * Jîngehên pêşkeftinê: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Nûtirîn GroupDocs.Signature for .NET ji [Nuget](https://www.nuget.org/packages/groupdocs.signature) bistînin
         
    code: |
        ```csharp    
        
        // Set up input Png file
        string filePath = "input.png";
        // Set up output file
        string outputFilePath = "output.png";

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
                
                // sign Png document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina belgeyên {{Pelformat}} bi Barcode Demoya Zindî"
    content: |
       Naha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) pelê Png bi îmzeyên cihêreng îmze bikin. Demoya serhêl a belaş li benda we ye.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode, ku wekî koda Binary a Derman jî tê zanîn, standardek barkodê ye, ku di pîşesaziya dermanan de wekî pergala kontrolkirina pakkirinê tê bikar anîn.
          characterset: |
             Reqemên hejmarî (0-9).
          textcapacity: |
             Ji 3 heta 131070 tenê yekjimarek yekjimar temsîl dike.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Îmzeyên din ên piştgirî yên Barcode ji bo C#"
    content: |
        "Her weha hûn dikarin {{Pelformat}} bi celebên din ên îmzayê re îmze bikin. Ji kerema xwe lîsteya jêrîn bibînin."
    format: 
        
       
back_to_top:
    enable: true
---