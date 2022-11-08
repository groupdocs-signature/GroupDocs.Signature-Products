---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Docm
productName: .NET
lang: sv
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Docm for C#

############################# Head ############################
head_title: "Ta bort Qrcode-signaturer från Docm-filer via C#"
head_description: "Radering av specifika Qrcode-signaturer från signerade Docm-dokument kan enkelt utföras med kort .NET-kod."

############################# Header ############################
title: "Ta bort Qrcode-signaturer som är placerade i Docm-filer"
description: "Ta bort olika Qrcode-signaturer från Docm-dokument. Att ta bort Qrcode-signaturer kräver enkel C#-kod."
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
    title: "Få information om GroupDocs.Signature for .NET API-funktioner"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API ger många sätt att behandla dina dokument med elektroniska signaturer. Digitala signaturer som texter, bilder, digitala certifikat, streckkoder, QR-koder, stämplar eller metadata finns tillgängliga. Kunder har möjlighet att lägga till, ta bort, uppdatera, verifiera eller söka digitala signaturer i PDF-filer, MS Word-dokument, MS Excel-arbetsböcker, MS PowerPoint-presentationer, Adobe Photoshop-filer och olika bildformat. Ett stort antal användbara funktioner och inställningar tillhandahålls.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Hur man tar bort Qrcode-signaturer från ditt Docm-dokument"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) tillhandahåller användbar funktion för att rensa Docm dokument från Qrcode signaturer med några rader kod.
        
        * Först, instansiera signaturobjekt som skickar sökvägen till ditt dokument som en konstruktorparameter.
        * Skapa sedan ett lämpligt signaturobjekt och ställ in dess unika identifierare.
        * Efter det, åberopa Delete-metoden som skickar signaturobjekt som måste tas bort.
        * Slutligen resultat av processdrift.

    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Signature for .NET stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.

        * Operativsystem: Microsoft Windows, Linux, MacOS
        * Utvecklingsmiljöer: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Ladda ner den senaste versionen av GroupDocs.Signature for .NET från [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Docm file
        string filePath = "input.docm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to delete
                // set up particular signature id
                QrCodeSignature signatureToDelete = new QrCodeSignature(id);

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
    title: "Signering med Qrcode signaturer Live Demo"
    content: |
       Lägg till olika elektroniska signaturer i filen Docm just nu genom att besöka webbplatsen [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ta bort dina Qrcode-signaturer med C#"
    content: |
        "Radering av e-signaturer som lagts till i olika dokumentformat. Ta bort signaturer snabbt utan extra kod."
    format: 
       
       
back_to_top:
    enable: true
---