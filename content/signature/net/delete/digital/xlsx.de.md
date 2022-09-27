---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Digital
fileformat: Xlsx
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsx for C#

############################# Head ############################
head_title: "Löschen Sie Digital-Signaturen aus Xlsx-Dateien über C#"
head_description: "Das Löschen bestimmter Digital-Signaturen aus signierten Xlsx-Dokumenten kann einfach mit dem kurzen .NET-Code durchgeführt werden."

############################# Header ############################
title: "Entfernen Sie Digital-Signaturen, die in Xlsx-Dateien platziert sind"
description: "Löschen Sie verschiedene Digital-Signaturen aus Xlsx-Dokumenten. Das Entfernen von Digital-Signaturen erfordert einfachen C#-Code."
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
    title: "Informieren Sie sich über GroupDocs.Signature for .NET-API-Funktionen"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API bietet viele Möglichkeiten, Ihre Dokumente mit elektronischen Signaturen zu verarbeiten. Digitale Signaturen wie Texte, Bilder, digitale Zertifikate, Barcodes, QR-Codes, Stempel oder Metadaten sind verfügbar. Kunden haben die Möglichkeit, digitale Signaturen in PDFs, MS Word-Dokumenten, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedenen Bildformaten hinzuzufügen, zu löschen, zu aktualisieren, zu überprüfen oder zu durchsuchen. Eine große Anzahl nützlicher Funktionen und Einstellungen werden bereitgestellt.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "So entfernen Sie Digital-Signaturen aus Ihrem Xlsx-Dokument"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bietet eine nützliche Funktion zum Löschen von Xlsx-Dokumenten von Digital-Signaturen mit ein paar Codezeilen.
        
        * Instanziieren Sie zunächst das Signaturobjekt, das den Pfad zu Ihrem Dokument als Konstruktorparameter übergibt.
        * Erstellen Sie dann ein geeignetes Signaturobjekt und richten Sie seine eindeutige Kennung ein.
        * Rufen Sie danach die Delete-Methode auf und übergeben Sie das Signaturobjekt, das gelöscht werden muss.
        * Schließlich resultieren Prozessoperationen.

    title_right: "System Anforderungen"
    content_right: |
        GroupDocs.Signature for .NET werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Laden Sie die neueste Version von GroupDocs.Signature for .NET von [Nuget](https://www.nuget.org/packages/groupdocs.signature) herunter
         
    code: |
        ```csharp    
                
        // Set up input Xlsx file
        string filePath = "input.xlsx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "a01e1940-997a-444b-89af-9309a2d559a5";

                // provide signature features to delete
                // set up particular signature id
                DigitalSignature signatureToDelete = new DigitalSignature(id);

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
    title: "Signieren mit Digital-Signaturen Live-Demo"
    content: |
       Fügen Sie jetzt verschiedene elektronische Signaturen zur Datei Xlsx hinzu, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Löschen Sie Ihre Digital-Signaturen mit C#"
    content: |
        "Löschung von E-Signaturen, die verschiedenen Dokumentenformaten hinzugefügt wurden. Entfernen Sie Signaturen schnell ohne zusätzlichen Code."
    format: 
       
       
back_to_top:
    enable: true
---