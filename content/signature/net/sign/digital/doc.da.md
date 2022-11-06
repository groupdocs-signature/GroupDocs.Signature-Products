---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Doc
productName: .NET
lang: da
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Doc for C#

############################# Head ############################
head_title: "Tilføjelse af digitale elektroniske signaturer til filen Doc med C#"
head_description: "Sæt digital signatur på filen Doc for .NET ved hjælp af et par linjer kode. Brug GroupDocs Document Signature API til at signere snesevis af filformater."

############################# Header ############################
title: "eSign Doc filer med Digital signaturer i C#"
description: "Sådan tilføjer du Digital-signatur med et par linjer med .NET-kode"
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
    title: "Om GroupDocs.Signature for .NET Digitale signaturer API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) er en populær API til at esignere dokumenter med de digitale elektroniske signaturer med digitale certifikater. Til Digitale signaturer bruger API PFX-certifikatfiler til at designe dokument med adgangskodebeskyttede private og offentlige nøgler. De digitale signaturer kan bruges til at certificere forretningsdokumenter med en bestemt eSign PDF-side, certificere hele Microsoft Office-dokumenter som Words, Excel, Powerpoint-filer og Open Office-dokumenter. Kunder kan nemt manipulere signaturerne som at redigere dem, fjerne eller justere. API'en giver mulighed for at søge og verificere signaturer. Desuden er der en masse muligheder for signaturtilpasning.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Trin til at signere {{Filformat}} med Digital i C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) giver mulighed for at signere Doc dokumenter med Digital signaturer hurtigt og nemt.
        
        * Opret en forekomst af signaturklassen, der leverer Doc-fil, der skal signere som sti eller hukommelsesstrøm
        * Instantiér SignOptions-klassen og indstil alle krævede data.
        * Kald Signature.Sign()-metoden ved at sende output Doc-fil eller hukommelsesstrøm

    title_right: " Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.

        * Operativsystemer: Microsoft Windows, Linux, MacOS
        * Udviklingsmiljøer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Få den seneste GroupDocs.Signature for .NET fra [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
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
    title: "Signering af {{Filformat}} dokumenter med Digital Live Demo"
    content: |
       Signer Doc-filen med forskellige signaturer lige nu ved at besøge webstedet [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Gratis online demo venter på dig.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andre understøttede Digital-signaturer for C#"
    content: |
        "Du kan også signere {{Filformat}} med andre signaturtyper. Se venligst listen nedenfor."
    format: 
       
       
back_to_top:
    enable: true
---