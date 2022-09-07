---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Otp
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Otp for C#

############################# Head ############################
head_title: "Aktualisieren Sie Image-Signaturen, die in Otp-Dateien platziert wurden, mit C#"
head_description: "Verwenden Sie den einfachen und leicht verständlichen .NET-Code für die Aktualisierung von Image-Signaturen in signierten Otp-Dokumenten."

############################# Header ############################
title: "Bearbeiten und aktualisieren Sie Image-Signaturen, die in Otp-Dateien platziert sind"
description: "Die API für .NET bietet Funktionen für die Aktualisierung von Image-Signaturen in Otp-Dokumenten. Aktualisieren Sie schnell und einfach elektronische Signaturen in Ihren Otp-Dokumenten mit ein paar Zeilen C#-Code."
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
    title: "Erfahren Sie mehr über GroupDocs.Signature for .NET-API-Funktionen"
    content: |
        Die API-Funktionalität von [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) enthält eine große Auswahl an Mitteln zur Verarbeitung nachgefragter Dokumentenformate mithilfe elektronischer Signaturen. Ein breites Spektrum an elektronischen Signaturen wie Texte, Bilder, digitale Zertifikate, Barcodes, QR-Codes, Stempel oder Metadaten werden unterstützt. Kunden können digitale Signaturen in PDFs, MS Word-Dokumenten, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedenen Bildformaten hinzufügen, entfernen, bearbeiten, validieren oder suchen. Zahlreiche nützliche Funktionen und Einstellungen stehen zur Verfügung.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "So ändern Sie Image-Signaturen in Ihrem Otp-Dokument"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) enthält nützliche Funktionen wie die Aktualisierung von Image-Signaturen, die in Otp-Dokumenten platziert sind. Es ermöglicht das Ändern von Signaturfunktionen ohne zusätzlichen Code.
        
        * Erstellen Sie zunächst ein Signature-Objekt, das als Konstruktorparameterpfad zu einem Dokument übergeben wird, das aktualisiert werden soll.
        * Instanziieren Sie dann ein geeignetes bestimmtes Signaturobjekt und richten Sie seine Kennung und Eigenschaften ein, die geändert werden müssen.
        * Rufen Sie zuletzt die Update-Methode von Signature auf, indem Sie ein bestimmtes Signaturobjekt übergeben.
        * Verarbeiten Sie die Aktualisierungsergebnisse zu Ihrer Benachrichtigung.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Laden Sie die neueste Version von GroupDocs.Signature for .NET von [Nuget](https://www.nuget.org/packages/groupdocs.signature) herunter
         
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
    title: "Signieren mit Image-Signaturen Live-Demo"
    content: |
       Fügen Sie jetzt verschiedene elektronische Signaturen zur Datei Otp hinzu, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aktualisieren Sie verschiedene Image-Signaturen über C#"
    content: |
        "Bearbeiten von digitalen Signaturen, die in verschiedenen Dokumentformaten platziert sind. Aktualisieren Sie Signaturdaten ohne zusätzlichen Code."
    format: 
       
       
back_to_top:
    enable: true
---