---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Image
fileformat: Odt
productName: Java
lang: de
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Odt for Java

############################# Head ############################
head_title: "Aktualisieren Sie Image-Signaturen, die in Odt-Dateien platziert wurden, mit Java"
head_description: "Verwenden Sie den einfachen und leicht verständlichen Java-Code für die Aktualisierung von Image-Signaturen in signierten Odt-Dokumenten."

############################# Header ############################
title: "Bearbeiten und aktualisieren Sie Image-Signaturen, die in Odt-Dateien platziert sind"
description: "Die API für Java bietet Funktionen für die Aktualisierung von Image-Signaturen in Odt-Dokumenten. Aktualisieren Sie schnell und einfach elektronische Signaturen in Ihren Odt-Dokumenten mit ein paar Zeilen Java-Code."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Erfahren Sie mehr über GroupDocs.Signature for Java-API-Funktionen"
    content: |
        Die API-Funktionalität von [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) enthält eine große Auswahl an Mitteln zur Verarbeitung nachgefragter Dokumentenformate mithilfe elektronischer Signaturen. Ein breites Spektrum an elektronischen Signaturen wie Texte, Bilder, digitale Zertifikate, Barcodes, QR-Codes, Stempel oder Metadaten werden unterstützt. Kunden können digitale Signaturen in PDFs, MS Word-Dokumenten, MS Excel-Arbeitsmappen, MS PowerPoint-Präsentationen, Adobe Photoshop-Dateien und verschiedenen Bildformaten hinzufügen, entfernen, bearbeiten, validieren oder suchen. Zahlreiche nützliche Funktionen und Einstellungen stehen zur Verfügung.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "So ändern Sie Image-Signaturen in Ihrem Odt-Dokument"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) enthält nützliche Funktionen wie die Aktualisierung von Image-Signaturen, die in Odt-Dokumenten platziert sind. Es ermöglicht das Ändern von Signaturfunktionen ohne zusätzlichen Code.
        
        * Erstellen Sie zunächst ein Signature-Objekt, das als Konstruktorparameterpfad zu einem Dokument übergeben wird, das aktualisiert werden soll.
        * Instanziieren Sie dann ein geeignetes bestimmtes Signaturobjekt und richten Sie seine Kennung und Eigenschaften ein, die geändert werden müssen.
        * Rufen Sie zuletzt die Update-Methode von Signature auf, indem Sie ein bestimmtes Signaturobjekt übergeben.
        * Verarbeiten Sie die Aktualisierungsergebnisse zu Ihrer Benachrichtigung.

    title_right: "System Anforderungen"
    content_right: |
        GroupDocs.Signature for Java werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.

        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebungen: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Laden Sie die neueste Version von GroupDocs.Signature for Java von [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) herunter
         
    code: |
        ```java    
                
        // Set up input Odt file
        String filePath = "input.odt";
        // Set up output file
        String outputFilePath = "output.odt";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to update
        // set up particular signature id
        ImageSignature signatureToUpdate = new ImageSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(170);
        // specify signature height
        signatureToUpdate.setHeight(250);
        // set left position
        signatureToUpdate.setLeft(10);
        // set top position
        signatureToUpdate.setTop(10);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Aktualisieren der Image-Signaturen auf den Dokumentseiten – Live-Demo"
    content: |
       Bearbeiten Sie jetzt verschiedene elektronische Signaturen des Dokuments Odt, indem Sie die Website [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) besuchen.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Aktualisieren Sie verschiedene Image-Signaturen über Java"
    content: |
        "Bearbeiten von digitalen Signaturen, die in verschiedenen Dokumentformaten platziert sind. Aktualisieren Sie Signaturdaten ohne zusätzlichen Code."
    format: 
       
       
back_to_top:
    enable: true
---