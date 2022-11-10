---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Svg
productName: .NET
lang: sl
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Svg for C#

############################# Head ############################
head_title: "Dodajte elektronske podpise metapodatkov dokumentom Svg prek C#"
head_description: "Uporabite metapodatke kot skrite elektronske podpise znotraj svojih dokumentov Svg z nekaj vrsticami kode C#. Uporabite API za podpis dokumentov GroupDocs za e-podpisovanje poslovnih dokumentov in datotek z informacijami o metapodatkih."

############################# Header ############################
title: "Elektronski podpisi metapodatkov za dokument Svg preko .NET so preprosti in enostavni za uporabo!"
description: "e-Podpišite svoje Svg dokumente in pogodbe s skritimi vnosi metapodatkov. Ustvarite metapodatke za PDF-je, dokumente MS Word, delovne zvezke MS Excel, predstavitve MS PowerPoint in različne formate slik brez težav in dodatnega kodiranja."
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
    title: "O API-ju za podpise metapodatkov GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je priljubljen API za e-podpisovanje digitalnih dokumentov. Na voljo so podpisi, kot so besedila, slike, digitalna potrdila, črtne kode, QR-kode, žigi ali metapodatki. Podpise lahko postavite na datoteke PDF, dokumente MS Word, delovne zvezke MS Excel, predstavitve MS PowerPoint, datoteke Adobe Photoshop in različne formate slik. Stranke lahko podpišejo svoj dokument in posodabljajo, iščejo, preverjajo, brišejo ali si predogledajo e-podpise, ki so bili na teh dokumentih. Poleg tega je na voljo veliko možnosti za prilagajanje podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraki za podpis Svg z Metadata v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) omogoča hitro in enostavno podpisovanje dokumentov Svg s podpisi Metadata.
        
        * Ustvarite primerek razreda podpisa, ki zagotavlja datoteko Svg, ki naj bi se podpisala kot pot ali pomnilniški tok
        * Instanciirajte razred SignOptions in nastavite vse zahtevane podatke.
        * Prikličite metodo Signature.Sign(), ki posreduje izhodno datoteko Svg ali pomnilniški tok

    title_right: " Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for .NET so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Pridobite najnovejši GroupDocs.Signature for .NET iz [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Svg file
        string filePath = "input.svg";
        // Set up output file
        string outputFilePath = "output.svg";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                MetadataSignOptions options = new MetadataSignOptions();

                // Specify different Metadata Signatures and add them to options signature collection
                // set start id
                ushort imgsMetadataId = 41996;
                // setup int value
                ImageMetadataSignature mdSign_DocId = new ImageMetadataSignature(imgsMetadataId++, 123456); // int
                options.Signatures.Add(mdSign_DocId);
                // setup Author property
                ImageMetadataSignature mdSign_Author = new ImageMetadataSignature(imgsMetadataId++, "Mr.Scherlock Holmes"); // string
                options.Signatures.Add(mdSign_Author);
                // setup data of sign date
                ImageMetadataSignature mdSign_Date = new ImageMetadataSignature(imgsMetadataId++, DateTime.Now); // DateTime
                options.Signatures.Add(mdSign_Date);
                // setup double
                ImageMetadataSignature mdSign_Amnt = new ImageMetadataSignature(imgsMetadataId++, 123.456M); //decimal value
                options.Signatures.Add(mdSign_Amnt);

                // sign Svg document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanje dokumentov Svg z Metadata Live Demo"
    content: |
       Takoj zdaj podpišite datoteko Svg z različnimi podpisi, tako da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Brezplačna spletna predstavitev čaka na vas.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podprti podpisi Metadata za C#"
    content: |
        "Svg lahko podpišete tudi z drugimi vrstami podpisov. Oglejte si spodnji seznam."
    format: 
       
       
back_to_top:
    enable: true
---