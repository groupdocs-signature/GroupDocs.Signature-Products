---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Text
fileformat: Potm
productName: .NET
lang: no
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Potm for C#

############################# Head ############################
head_title: "Bekreftelse av Text signaturer for Potm filer via C#"
head_description: "Bruk bare noen få linjer med .NET-kode for å bekrefte Potm-dokumenter og deres Text-signaturer."

############################# Header ############################
title: "Text signaturbekreftelse for {{Filformat}}-filer"
description: "API for .NET gir mulighet til å bekrefte Text-signaturer i Potm-dokumenter. Verifisering av e-signaturer i Potm-dokumentene dine kan utføres raskt og enkelt."
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
    title: "Oppdag nye GroupDocs.Signature for .NET API-funksjoner"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API gir et bredt spekter av måter å behandle en rekke dokumentformater ved å bruke elektroniske signaturer. Mange typer digitale signaturer som tekster, bilder, digitale sertifikater, strekkoder, QR-koder, stempler eller metadata støttes. Kunder kan legge til, fjerne, redigere, validere eller søke i digitale signaturer i PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og ulike bildeformater. Utrolig mange tilleggsfunksjoner og innstillinger er tilgjengelige.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Slik validerer du Text-signaturer i {{Filformat}}-dokumentet ditt"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inkluderer nyttige funksjoner som bekreftelse av Text-signaturer plassert på Potm-dokumenter. Bruk denne muligheten uten å implementere ekstra kode.
        
        * For det første instansierer Signature-klassen som gir en konstruktørparameterbane til et dokument som skal verifiseres.
        * For det andre, opprett et nytt VerifyOptions-objekt og sett opp alle nødvendige egenskaper.
        * Til slutt påkaller du Signatures objektbekreftelsesmetode ved å sende VerifyOptions-forekomsten.
        * Behandle deretter bekreftelsesresultater.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Last ned den nyeste versjonen av GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Potm file
        string filePath = "input.potm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                TextVerifyOptions options = new TextVerifyOptions()
                {
                    // Process all pages 
                    AllPages = true,
                    // set up text match type
                    MatchType = TextMatchType.Exact,
                    // specify text pattern to search
                    Text = "Very important signature",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering med Text signaturer Live Demo"
    content: |
       Legg til ulike elektroniske signaturer i Potm-filen akkurat nå ved å gå til nettstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bekreft andre Text-signaturer med C#"
    content: |
        "Verifikasjon av elektroniske signaturer plassert i ulike dokumenter. Sjekk kvaliteten på signaturene i de populære filformatene som vist nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---