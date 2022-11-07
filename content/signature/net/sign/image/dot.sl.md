---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Dot
productName: .NET
lang: sl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Dot for C#

############################# Head ############################
head_title: "Dodajanje podpisov Image v datoteko Dot z C#"
head_description: "Z nekaj vrsticami kode postavite podpis Image na datoteko Dot za .NET. Uporabite API za podpis dokumentov GroupDocs za podpis na desetine formatov datotek."

############################# Header ############################
title: "Podpišite Dot datoteke s podpisi Image v C#"
description: "Kako dodati podpis Image z nekaj vrsticami kode .NET"
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
    title: "O API-ju za slikovne podpise GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je priljubljen API za e-podpisovanje digitalnih dokumentov. Na voljo so podpisi, kot so besedila, slike, digitalna potrdila, črtne kode, QR-kode, žigi ali metapodatki. Podpise lahko postavite na datoteke PDF, dokumente MS Word, delovne zvezke MS Excel, predstavitve MS PowerPoint, datoteke Adobe Photoshop in različne formate slik. Stranke lahko podpišejo svoj dokument in posodabljajo, iščejo, preverjajo, brišejo ali si predogledajo e-podpise, ki so bili na teh dokumentih. Poleg tega je na voljo veliko možnosti za prilagajanje podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraki za podpis Dot z Image v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) omogoča hitro in enostavno podpisovanje dokumentov Dot s podpisi Image.
        
        * Ustvarite primerek razreda podpisa, ki zagotavlja datoteko Dot, ki naj bi se podpisala kot pot ali pomnilniški tok
        * Instanciirajte razred SignOptions in nastavite vse zahtevane podatke.
        * Prikličite metodo Signature.Sign(), ki posreduje izhodno datoteko Dot ali pomnilniški tok

    title_right: " Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for .NET so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Pridobite najnovejši GroupDocs.Signature for .NET iz [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dot file
        string filePath = "input.dot";
        // Set up output file
        string outputFilePath = "output.dot";
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

            // sign Dot document
            SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanje dokumentov Dot z Image Live Demo"
    content: |
       Takoj zdaj podpišite datoteko Dot z različnimi podpisi, tako da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Brezplačna spletna predstavitev čaka na vas.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podprti podpisi Image za C#"
    content: |
        "Dot lahko podpišete tudi z drugimi vrstami podpisov. Oglejte si spodnji seznam."
    format: 
       
       
back_to_top:
    enable: true
---