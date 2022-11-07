---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Postnet
fileformat: Bmp
productName: .NET
lang: ku
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Bmp for C#

############################# Head ############################
head_title: "eSign Bmp belgeya bi Postnet Barcode di C#"
head_description: "Îmzeya barkodê ya Postnet biafirîne û bi çend rêzikên kodê bi .NET li ser belgeya Bmp biafirîne. Ji bo îmzekirina cûrbecûr formatên pelan API-ya Îmzekirina Belgeya GroupDocs bikar bînin."

############################# Header ############################
title: "Di C# de ji bo belgeya Postnet îmzeya barkodê çêbike"
description: "Belgeyên karsaziya xwe yên {{Pelformat}} bi Postnet Barkodê îmze bikin. Bi çend rêzikên kodê re zû û bi hêsanî îmzeya Barkodê biafirînin da ku vebijarkên îmzekirinê saz bikin."
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
    title_left: "Gavên îmzekirina Bmp bi Barcode di C# de"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) îmzakirina belgeyên Bmp bi îmzeyên Barcode zû û bi hêsanî peyda dike.
        
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
        
        // Set up input Bmp file
        string filePath = "input.bmp";
        // Set up output file
        string outputFilePath = "output.bmp";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Postnet,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Bmp document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina belgeyên {{Pelformat}} bi Barcode Demoya Zindî"
    content: |
       Naha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) pelê Bmp bi îmzeyên cihêreng îmze bikin. Demoya serhêl a belaş li benda we ye.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Postnet Barcode"
          content: |
            POSTNET (Teknîka kodkirina hejmarî ya posteyê) sembolek barkodê ye ku ji hêla Karûbarê Posta Dewletên Yekbûyî ve tê bikar anîn da ku di rêvekirina nameyê de arîkar bike.
          characterset: |
             Reqemên hejmarî (0-9).
          textcapacity: |
             Heta 11 tîpan.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAACcAAAAjCAYAAAAXMhMjAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAACeSURBVFhH7c7BCkMxEELR/P9Pp1LoRrCXpi4Cbw5kIRKZtS82x52a407Ncae+HrfWer8Pyr+i/3NcQv/nuIT+z3EJ/X/Ocf9mlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2uREaa2eXG6Gxdna5ERprZ5cbobF2drkRGmtnlxuhsXZ2ubnAHHdqjjt18XF7vwDevzbHqsQWPwAAAABJRU5ErkJggg==

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