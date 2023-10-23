---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Zip
productName: .NET
lang: de
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Zip for C#

############################# Head ############################
head_title: "Hinzufügen digitaler elektronischer Signaturen zur Zip-Datei mit C#"
head_description: "Fügen Sie der Zip-Datei für .NET mit ein paar Codezeilen eine digitale Signatur hinzu. Verwenden Sie die GroupDocs Document Signature API, um Dutzende von Dateiformaten zu signieren."

############################# Header ############################
title: "eSigniere Zip-Dateien mit Digital-Signaturen in C#"
description: "So fügen Sie eine Digital-Signatur mit ein paar Zeilen .NET-Code hinzu"
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
    title: "Über die API für digitale Signaturen von GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ist eine beliebte API zum Signieren von Dokumenten mit digitalen elektronischen Signaturen und digitalen Zertifikaten. Für die API für digitale Signaturen werden PFX-Zertifikatsdateien verwendet, um Dokumente mit passwortgeschützten privaten und öffentlichen Schlüsseln zu signieren. Die digitalen Signaturen können verwendet werden, um Geschäftsdokumente mit eSign-PDF-Einzelseiten zu zertifizieren, ganze Microsoft Office-Dokumente wie Words, Excel, Powerpoint-Dateien und Open Office-Dokumente zu zertifizieren. Kunden können die Signaturen einfach manipulieren, z. B. bearbeiten, entfernen oder anpassen. Die API bietet eine Möglichkeit, Signaturen zu suchen und zu überprüfen. Darüber hinaus werden viele Möglichkeiten zur Anpassung von Signaturen bereitgestellt.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Schritte zum Signieren von Zip mit Digital in C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) bietet die Möglichkeit, Zip-Dokumente mit Digital-Signaturen schnell und einfach zu signieren.
        
        * Erstellen Sie eine Instanz der Signature-Klasse, die die Zip-Datei bereitstellt, die als Pfad oder Speicherstream signiert werden soll
        * Instanziieren Sie die SignOptions-Klasse und legen Sie alle erforderlichen Daten fest.
        * Rufen Sie die Signature.Sign()-Methode auf und übergeben Sie die Zip-Ausgabedatei oder den Speicherstrom

    title_right: " System Anforderungen"
    content_right: |
        GroupDocs.Signature for .NET werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Holen Sie sich das neueste GroupDocs.Signature for .NET von [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Zip file
        string filePath = "input.zip";
        // Set up output file
        string outputFilePath = "output.zip";
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

                // sign Zip document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Signieren von Zip-Dokumenten mit Digital Live-Demo"
    content: |
       Signieren Sie die Datei Zip jetzt mit verschiedenen Signaturen, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen. Kostenlose Online-Demo wartet auf Sie.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Andere unterstützte Digital-Signaturen für C#"
    content: |
        "Sie können Zip auch mit anderen Signaturtypen signieren. Bitte sehen Sie sich die Liste unten an."
    format: 
       
       
back_to_top:
    enable: true
---