---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Ods
productName: .NET
lang: ku
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ods for C#

############################# Head ############################
head_title: "Zêdekirina îmzeyên elektronîkî yên dîjîtal li pelê Ods bi C#"
head_description: "Ji bo .NET bi çend rêzikên kodê Îmzeya Dîjîtal bixin ser pelê {{Pelformat}}. API-ya Îmzekirina Belgeya GroupDocs bikar bînin da ku bi dehan formatên pelan îmze bikin."

############################# Header ############################
title: "eSign Ods pelên bi Digital di C# de"
description: "Meriv çawa bi çend rêzikên koda .NET nîşana Digital zêde bike"
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
    title: "Derbarê GroupDocs.Signature for .NET API-ya îmzeyên dîjîtal"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API-ya populer e ku bi îmzeyên elektronîkî yên dîjîtal, bi sertîfîkayên dîjîtal ve, belgeyan çêdike. Ji bo îmzeyên dîjîtal API pelên sertîfîkayên PFX bikar tîne da ku belgeyê bi bişkojkên taybet û giştî yên parastî bi şîfreyê veqetîne. Dibe ku îmzeyên dîjîtal ji bo pejirandina belgeyên karsaziyê bi rûpela taybetî ya eSign PDF-ê re, pejirandina tevahî belgeyên Microsoft Office yên mîna Words, Excel, pelên Powerpoint, û belgeyên Open Office-ê werin bikar anîn. Xerîdar dikarin bi hêsanî îmzeyan wekî sererastkirina wan, rakirin an sererastkirina wan manîpule bikin. API ji bo lêgerîn û verastkirina îmzeyan rêyek peyda dike. Digel vê yekê, ji bo xwerûkirina îmzeyan gelek jêhatî têne peyda kirin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Gavên îmzekirina Ods bi Digital di C# de"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) îmzakirina belgeyên Ods bi îmzeyên Digital zû û bi hêsanî peyda dike.
        
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
                
        // Set up input Ods file
        string filePath = "input.ods";
        // Set up output file
        string outputFilePath = "output.ods";
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

                // sign Ods document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina belgeyên {{Pelformat}} bi Digital Demoya Zindî"
    content: |
       Naha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) pelê Ods bi îmzeyên cihêreng îmze bikin. Demoya serhêl a belaş li benda we ye.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Îmzeyên din ên piştgirî yên Digital ji bo C#"
    content: |
        "Her weha hûn dikarin {{Pelformat}} bi celebên din ên îmzayê re îmze bikin. Ji kerema xwe lîsteya jêrîn bibînin."
    format: 
       
       
back_to_top:
    enable: true
---