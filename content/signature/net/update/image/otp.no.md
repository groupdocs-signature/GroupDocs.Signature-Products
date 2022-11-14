---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Otp
productName: .NET
lang: no
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Otp for C#

############################# Head ############################
head_title: "Oppdater Image-signaturer plassert på Otp-filer med C#"
head_description: "Bruk enkel og enkel for å forstå .NET-koden for Image-signaturoppdatering i signerte {{Filformat}}-dokumenter."

############################# Header ############################
title: "Rediger og oppdater Image-signaturer plassert i {{Filformat}}-filer"
description: "API for .NET gir funksjonalitet for Image-signaturer som oppdateres i {{Filformat}}-dokumenter. Oppdater e-signaturer i {{Filformat}}-dokumentene dine med et par linjer med C#-kode raskt og enkelt."
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
    title: "Lær om GroupDocs.Signature for .NET API-funksjoner"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API-funksjonalitet inneholder et stort utvalg måter å behandle etterspurte dokumentformater ved å bruke elektroniske signaturer. Et bredt spekter av e-signaturer som tekster, bilder, digitale sertifikater, strekkoder, QR-koder, stempler eller metadata støttes. Kunder kan legge til, fjerne, redigere, validere eller søke i digitale signaturer i PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og ulike bildeformater. Mange nyttige funksjoner og innstillinger er tilgjengelige.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hvordan endre Image-signaturer i {{Filformat}}-dokumentet ditt"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inkluderer nyttige funksjoner som oppdatering av Image-signaturer plassert i {{Filformat}}-dokumenter. Det gjør det mulig å endre signaturfunksjoner uten ekstra kode.
        
        * Til å begynne med, lag signaturobjekt som passerer som en konstruktørparameterbane til et dokument som skal oppdateres.
        * Deretter instansierer du et passende bestemt signaturobjekt og setter opp identifikatoren og egenskapene som må endres.
        * Til slutt kaller du Signatures oppdateringsmetode som sender et bestemt signaturobjekt.
        * Behandle oppdatering av resultater til din varsel.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Last ned den nyeste versjonen av GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Otp file
        string filePath = "input.otp";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                ImageSignature signatureToUpdate = new ImageSignature(id)
                {
                    // specify signature width
                    Width = 170,
                    // specify signature height
                    Height = 250,
                    // set left position
                    Left = 10,
                    // set top position
                    Top = 10
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Oppdatering av Image-signaturene på dokumentsidene - Live Demo"
    content: |
       Rediger ulike elektroniske signaturer til Otp-dokumentet akkurat nå ved å gå til nettstedet [GroupDocs.Signature-appen](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Oppdater forskjellige Image-signaturer via C#"
    content: |
        "Redigering av digitale signaturer som er plassert i ulike dokumentformater. Oppdater signaturdata uten ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---