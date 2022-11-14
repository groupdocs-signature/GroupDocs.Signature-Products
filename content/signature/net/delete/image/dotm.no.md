---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Dotm
productName: .NET
lang: no
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Dotm for C#

############################# Head ############################
head_title: "Slett Image-signaturer fra Dotm-filer via C#"
head_description: "Sletting av spesifikke Image-signaturer fra signerte Dotm-dokumenter kan enkelt utføres med kort .NET-kode."

############################# Header ############################
title: "Fjern Image-signaturer som er plassert i {{Filformat}}-filer"
description: "Slett forskjellige Image-signaturer fra {{Filformat}}-dokumenter. Fjerning av Image-signaturer krever enkel C#-kode."
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
    title: "Få informasjon om GroupDocs.Signature for .NET API-funksjoner"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API gir mange måter å behandle dokumentene dine på ved hjelp av elektroniske signaturer. Digitale signaturer som tekster, bilder, digitale sertifikater, strekkoder, QR-koder, frimerker eller metadata er tilgjengelig. Kunder har mulighet til å legge til, slette, oppdatere, verifisere eller søke i digitale signaturer på PDF-er, MS Word-dokumenter, MS Excel-arbeidsbøker, MS PowerPoint-presentasjoner, Adobe Photoshop-filer og ulike bildeformater. Et stort antall nyttige funksjoner og innstillinger er gitt.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Slik fjerner du Image-signaturer fra {{Filformat}}-dokumentet"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) gir nyttig funksjon for å tømme {{Filformat}} dokumenter for Image signaturer med noen få linjer med kode.
        
        * For det første, instansierer Signatur-objektets bane til dokumentet som en konstruktørparameter.
        * Deretter oppretter du et passende signaturobjekt og setter opp dets unike identifikator.
        * Deretter påkaller du Slett-metoden som sender signaturobjekt som må slettes.
        * Til slutt resultat av prosessdrift.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Utviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Last ned den nyeste versjonen av GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotm file
        string filePath = "input.dotm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

                // provide signature features to delete
                // set up particular signature id
                ImageSignature signatureToDelete = new ImageSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signering med Image signaturer Live Demo"
    content: |
       Legg til ulike elektroniske signaturer i Dotm-filen akkurat nå ved å gå til nettstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Slett Image-signaturene dine med C#"
    content: |
        "Sletting av e-signaturer som ble lagt til ulike dokumentformater. Fjern signaturer raskt uten ekstra kode."
    format: 
       
       
back_to_top:
    enable: true
---