---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Ots
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Ots for C#

############################# Head ############################
head_title: "Löschen Sie Text-Signaturen aus Ots-Dateien über C#"
head_description: "Das Löschen bestimmter Text-Signaturen aus signierten Ots-Dokumenten kann einfach mit dem kurzen .NET-Code durchgeführt werden."

############################# Header ############################
title: "Entfernen Sie Text-Signaturen, die in Ots-Dateien platziert sind"
description: "Löschen Sie verschiedene Text-Signaturen aus Ots-Dokumenten. Das Entfernen von Text-Signaturen erfordert einfachen C#-Code."
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
    title_left: "So entfernen Sie Text-Signaturen aus Ihrem Ots-Dokument"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bietet eine nützliche Funktion zum Löschen von Ots-Dokumenten von Text-Signaturen mit ein paar Codezeilen.
        
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
                
        // Set up input Ots file
        string filePath = "input.ots";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to delete
                // set up particular signature id
                TextSignature signatureToDelete = new TextSignature(id);

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
    title: "Signieren mit Text-Signaturen Live-Demo"
    content: |
       Fügen Sie jetzt verschiedene elektronische Signaturen zur Datei Ots hinzu, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Löschen Sie Ihre Text-Signaturen mit C#"
    content: |
        "Löschung von E-Signaturen, die verschiedenen Dokumentenformaten hinzugefügt wurden. Entfernen Sie Signaturen schnell ohne zusätzlichen Code."
    format: 
       
       
back_to_top:
    enable: true
---