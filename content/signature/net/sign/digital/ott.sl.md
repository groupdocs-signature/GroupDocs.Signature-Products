---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Ott
productName: .NET
lang: sl
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ott for C#

############################# Head ############################
head_title: "Dodajanje digitalnih elektronskih podpisov datoteki Ott z C#"
head_description: "Z nekaj vrsticami kode postavite digitalni podpis na datoteko Ott za .NET. Uporabite API za podpis dokumentov GroupDocs za podpis na desetine formatov datotek."

############################# Header ############################
title: "Datoteke eSign Ott s podpisi Digital v C#"
description: "Kako dodati podpis Digital z nekaj vrsticami kode .NET"
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
    title: "O API-ju za digitalne podpise GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) je priljubljen API za oblikovanje dokumentov z digitalnimi elektronskimi podpisi z digitalnimi potrdili. API za digitalne podpise uporablja datoteke s potrdili PFX za podpis dokumenta z zasebnimi in javnimi ključi, zaščitenimi z geslom. Digitalni podpisi se lahko uporabljajo za potrjevanje poslovnih dokumentov z določeno stranjo eSign PDF, potrjevanje celotnih dokumentov Microsoft Office, kot so Words, Excel, datoteke Powerpoint in dokumenti Open Office. Stranke lahko preprosto manipulirajo s podpisi, kot jih urejajo, odstranjujejo ali prilagajajo. API omogoča iskanje in preverjanje podpisov. Poleg tega je na voljo veliko možnosti za prilagajanje podpisov.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Koraki za podpis Ott z Digital v C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) omogoča hitro in enostavno podpisovanje dokumentov Ott s podpisi Digital.
        
        * Ustvarite primerek razreda podpisa, ki zagotavlja datoteko Ott, ki naj bi se podpisala kot pot ali pomnilniški tok
        * Instanciirajte razred SignOptions in nastavite vse zahtevane podatke.
        * Prikličite metodo Signature.Sign(), ki posreduje izhodno datoteko Ott ali pomnilniški tok

    title_right: " Sistemske zahteve"
    content_right: |
        GroupDocs.Signature for .NET so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.

        * Operacijski sistemi: Microsoft Windows, Linux, MacOS
        * Razvojna okolja: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Pridobite najnovejši GroupDocs.Signature for .NET iz [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ott file
        string filePath = "input.ott";
        // Set up output file
        string outputFilePath = "output.ott";
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

                // sign Ott document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Podpisovanje dokumentov Ott z Digital Live Demo"
    content: |
       Takoj zdaj podpišite datoteko Ott z različnimi podpisi, tako da obiščete spletno mesto [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Brezplačna spletna predstavitev čaka na vas.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Drugi podprti podpisi Digital za C#"
    content: |
        "Ott lahko podpišete tudi z drugimi vrstami podpisov. Oglejte si spodnji seznam."
    format: 
       
       
back_to_top:
    enable: true
---