---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Dot
productName: .NET
lang: ku
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Dot for C#

############################# Head ############################
head_title: "Bi rêya C# îmzeyên elektronîkî yên Metadata li belgeyên Dot bişînin"
head_description: "Metadata wekî îmzeyên elektronîkî yên veşartî di hundurê belgeyên xwe yên Dot de bi karanîna çend rêzikên koda C# bikar bînin. API-ya Îmzekirina Belgeya GroupDocs bikar bînin da ku belge û pelên karsaziya xwe bi agahdariya Metadata e-îmza bikin."

############################# Header ############################
title: "Îmzeyên elektronîkî yên metadata ji bo belgeya Dot bi rêya .NET ji bo karanîna hêsan û hêsan in!"
description: "Belge û peymanên xwe yên {{Pelformat}} bi navnîşên Metadata veşartî re îmze bikin. Ji bo PDF, belgeyên MS Word, pirtûkên xebatê MS Excel, pêşandanên MS PowerPoint û cûrbecûr formatên wêneyê bêyî pirsgirêk û kodkirina zêde Metadata biafirînin."
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
    title: "Der barê GroupDocs.Signature for .NET API-ya îmzeyên metadata"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API-ya navdar e ji bo e-îmzakirina belgeyên dîjîtal. Îmzeyên wekî nivîs, wêne, sertîfîkayên dîjîtal, barkod, QR-kod, stamp an metadata hene. Dibe ku îmze li ser PDF, belgeyên MS Word, pirtûkên xebatê yên MS Excel, pêşandanên MS PowerPoint, pelên Adobe Photoshop û cûrbecûr formên wêneyan werin danîn. Xerîdar dikarin belgeya xwe îmze bikin û e-îmzayên ku li ser wan belgeyan hatine danîn nûve bikin, bigerin, verast bikin, jêbikin an pêşdîtin bikin. Digel vê yekê, ji bo xwerûkirina îmzeyan gelek jêhatî têne peyda kirin.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Gavên îmzekirina Dot bi Metadata di C# de"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) îmzakirina belgeyên Dot bi îmzeyên Metadata zû û bi hêsanî peyda dike.
        
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
        
        // Set up input Dot file
        string filePath = "input.dot";
        // Set up output file
        string outputFilePath = "output.dot";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Dot document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Îmzekirina belgeyên {{Pelformat}} bi Metadata Demoya Zindî"
    content: |
       Naha bi serdana malpera [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) pelê Dot bi îmzeyên cihêreng îmze bikin. Demoya serhêl a belaş li benda we ye.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Îmzeyên din ên piştgirî yên Metadata ji bo C#"
    content: |
        "Her weha hûn dikarin {{Pelformat}} bi celebên din ên îmzayê re îmze bikin. Ji kerema xwe lîsteya jêrîn bibînin."
    format: 
       
       
back_to_top:
    enable: true
---