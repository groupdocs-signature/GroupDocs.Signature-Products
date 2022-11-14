---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: ISBN
fileformat: Xlsb
productName: .NET
lang: no
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Xlsb for C#

############################# Head ############################
head_title: "eSign {{Filformat}}-dokument med ISBN strekkode i C#"
head_description: "Opprett ISBN strekkodesignatur og legg den på Xlsb-dokumentet med .NET ved å bruke et par linjer med kode. Bruk GroupDocs Document Signature API for å signere ulike filformater."

############################# Header ############################
title: "Generer ISBN strekkodesignatur for {{Filformat}} dokument i C#"
description: "eSignér Xlsb-bedriftsdokumentene dine med ISBN strekkode. Generer strekkodesignatur raskt og enkelt med noen få linjer med kode for å sette opp signeringsalternativer."
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
    title: "Om GroupDocs.Signature for .NET API for strekkodesignaturer."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) er et raskt og enkelt API for å administrere digitale dokumenter e-signering ved hjelp av strekkodetyper som UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 og mange andre. Kunder kan enkelt lage strekkoder som gir nødvendig tekst og legge dem på PDF, Microsoft Office Words-dokumenter, Microsoft Office Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og ulike bildeformater. Strekkoder plassert i dokumenter kan oppdateres, søkes, bekreftes, slettes eller forhåndsvises enten. Dessuten støttes strekkodertilpasning.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trinn for å signere {{Filformat}} med Barcode i C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gir mulighet til å signere Xlsb-dokumenter med Barcode-signaturer raskt og enkelt.
        
        * Opprett en forekomst av signaturklassen som gir Xlsb-fil som skal signere som bane eller minnestrøm
        * Instantiate SignOptions-klassen og angi alle etterspurte data.
        * Påkall Signature.Sign()-metoden ved å sende utdatafilen Xlsb eller minnestrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Få den siste GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Xlsb file
        string filePath = "input.xlsb";
        // Set up output file
        string outputFilePath = "output.xlsb";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.ISBN,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Xlsb document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering av {{Filformat}} dokumenter med Barcode Live Demo"
    content: |
       Signer Xlsb-filen med forskjellige signaturer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family). Gratis online demo venter på deg.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About ISBN Barcode"
          content: |
            International Standard Book Number (ISBN) er en numerisk kommersiell bokidentifikator som er ment å være unik.[a][b] Utgivere kjøper ISBN-numre fra en tilknyttet organisasjon til International ISBN Agency.
          characterset: |
             Numeriske sifre (0-9).
          textcapacity: |
             Nøyaktig 9 siffer + 1 kontrollsiffer.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre støttede Barcode-signaturer for C#"
    content: |
        "Du kan også signere {{Filformat}} med andre signaturtyper. Vennligst se listen nedenfor."
    format: 
        
       
back_to_top:
    enable: true
---