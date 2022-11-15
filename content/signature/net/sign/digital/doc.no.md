---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Doc
productName: .NET
lang: no
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for C#

############################# Head ############################
head_title: "Legger til digitale elektroniske signaturer i filen Doc med C#"
head_description: "Sett digital signatur på Doc-filen for .NET ved å bruke noen få linjer med kode. Bruk GroupDocs Document Signature API til å signere dusinvis av filformater."

############################# Header ############################
title: "eSign Doc-filer med Digital-signaturer i C#"
description: "Slik legger du til Digital-signatur med noen få linjer med .NET-kode"
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
    title: "Om GroupDocs.Signature for .NET API for digitale signaturer"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) er et populært API for å esignere dokumenter med digitale elektroniske signaturer, med digitale sertifikater. For Digitale signaturer bruker API PFX-sertifikatfiler for å esignere dokumenter med passordbeskyttede private og offentlige nøkler. De digitale signaturene kan brukes til å sertifisere forretningsdokumenter med eSign PDF-spesifikk side, sertifisere hele Microsoft Office-dokumenter som Words, Excel, Powerpoint-filer og Open Office-dokumenter. Kunder kan enkelt manipulere signaturene som å redigere dem, fjerne eller justere. API-en gir en måte å søke og bekrefte signaturer på. Dessuten er det gitt mange muligheter for tilpasning av signaturer.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trinn for å signere Doc med Digital i C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gir mulighet til å signere Doc-dokumenter med Digital-signaturer raskt og enkelt.
        
        * Opprett en forekomst av signaturklassen som gir Doc-fil som skal signere som bane eller minnestrøm
        * Instantiate SignOptions-klassen og angi alle etterspurte data.
        * Påkall Signature.Sign()-metoden ved å sende utdatafilen Doc eller minnestrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Få den siste GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";
        // Set up output file
        string outputFilePath = "output.doc";
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

                // sign Doc document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering av Doc dokumenter med Digital Live Demo"
    content: |
       Signer Doc-filen med forskjellige signaturer akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family). Gratis online demo venter på deg.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre støttede Digital-signaturer for C#"
    content: |
        "Du kan også signere Doc med andre signaturtyper. Vennligst se listen nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---