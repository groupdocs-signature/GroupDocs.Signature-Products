---
############################# Static ############################
layout: "landing"
date: 2024-09-25T12:45:24
draft: false

lang: de
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java" 
    # supported_platforms loop
    - title: "Python"
      tag: "python-net" 

############################# Head ############################
head_title: "Node.js-API für digitale Signaturen – GroupDocs.Signature"
head_description: "Integrieren Sie sichere elektronische Signaturen in Node.js-Apps mit GroupDocs.Signature. Optimieren Sie Arbeitsabläufe beim Signieren von Dokumenten einfach und effizient."

############################# Header ############################
title: "Dokumente unterschreiben mit Node.js-API"
description: "Signieren Sie digitale Dokumente und Bilder auf jeder Plattform mit unseren flexiblen APIs und App-basierten Lösungen für Programmierer und Endbenutzer."
words:
  for: "für"

actions:
  main: "Von NPM herunterladen"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
  title: "Bereit anzufangen?"
  description: "Testen Sie die Funktionen von GroupDocs.Signature kostenlos oder fordern Sie eine Lizenz an"

release:
  title: "Version {0} veröffentlicht"
  notes: "Schau was neu ist"
  downloads: "Downloads"

code:
  title: "Signieren von PDFs mit Node.js"
  more: "Mehr Beispiele"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // PDF-Dokument auswählen
    let signature = new Signature("sample.pdf");
    
    // Text bereitstellen
    let options = new TextSignOptions("John Smith");
    
    // Farbe einstellen
    options.ForeColor = Color.Red;
    
    // Dokument unterschreiben und in Datei speichern
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature-Übersicht"
  description: "Bibliothek zum Signieren von Dokumenten, die in Node.js-Anwendungen verwendet werden kann"
  features:
    # feature loop
    - title: "Digitale Signaturlösung für Geschäftsdokumente mit Node.js"
      content: "GroupDocs.Signature for Node.js via Java bietet einen umfassenden Satz digitaler Signaturoptionen für PDF-, Office-Dokumente und Bilder. Es stehen Text, Barcodes, Bilder, digitale Zertifikate und Metadaten zur Verfügung. Eine optimierte Dokumentenverarbeitung sorgt für Effizienz."

    # feature loop
    - title: "Erweiterte Manipulation signierter Dokumente"
      content: "GroupDocs.Signature ermöglicht Ihnen die Verarbeitung signierter Dokumente. Suchen und validieren Sie Signaturen anhand verschiedener Kriterien. Extrahieren Sie außerdem detaillierte Dokumentinformationen oder generieren Sie Vorschaubilder von Seiten."

    # feature loop
    - title: "Verschiedene Ausgabeformate"
      content: "Unsere Lösung bietet umfassende Kontrolle über das Ausgabeformat signierter Dokumente. Positionieren Sie Signaturen präzise auf jeder Seite und passen Sie deren Erscheinungsbild an. Speichern Sie signierte Dokumente in zahlreichen unterstützten Formaten und sichern Sie diese optional mit Passwörtern."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Signature for Node.js via Java führt die Dokumentenverarbeitung mit verschiedenen Betriebssystemen durch"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Unterstützte Dateiformate"
  description: |
    GroupDocs.Signature for Node.js via Java erleichtert Vorgänge für die [beliebten Dateiformate](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office-Formate
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Bilder und andere Formate
        * **tragbar:** PDF
        * **Bilder:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Andere Büroformate:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Andere Formate
        * **Netz:** HTML, MHTML
        * **Archiv:** ZIP, TAR, 7Z
        * **Zertifikate:** PFX

############################# Features ############################
features:
  enable: true
  title: "Funktionen von GroupDocs.Signature"
  description: "Signieren Sie PDFs, Office-Dokumente und Bilder mit digitalen Signaturen"

  items:
    # feature loop
    - icon: "sign"
      title: "Geschäftssignaturen"
      content: "Verwenden Sie verschiedene Signaturtypen zum Signieren von Dokumenten. Platzieren Sie digitale Signaturen präzise an jeder beliebigen Stelle auf der Seite."

    # feature loop
    - icon: "custom"
      title: "Anpassen der Signaturdarstellung"
      content: "Passen Sie die visuellen Aspekte von Signaturen an, indem Sie Farbe, Schriftart, Ränder, Drehung und mehr anpassen, um das gewünschte Ergebnis zu erzielen."

    # feature loop
    - icon: "password"
      title: "Passwortgeschützte Dokumente"
      content: "Schützen Sie signierte Dokumente für viele unterstützte Dokumentformate mit einem Passwort, um die Sicherheit zu erhöhen."

    # feature loop
    - icon: "protect"
      title: "Verhindern unbefugter Änderungen"
      content: "Schützen Sie wichtige, mit digitalen Zertifikaten signierte Geschäftsdokumente vor unbefugten Änderungen."

    # feature loop
    - icon: "convert"
      title: "Gewünschte Ausgabeformate"
      content: "Erhalten Sie mühelos signierte Dokumente in jedem unterstützten Format. Konvertieren Sie MS Word-Dokumente ganz einfach in das PDF-Format."

    # feature loop
    - icon: "preview"
      title: "Vorschau von Dokumenten"
      content: "Speichern Sie einzelne Dokumentseiten als Bilder für den zukünftigen Bedarf."

    # feature loop
    - icon: "search"
      title: "Signatursuche"
      content: "Rufen Sie Informationen zu zuvor hinzugefügten Signaturen in Ihren Dokumenten ab."

    # feature loop
    - icon: "validate"
      title: "Dokumentenvalidierung"
      content: "Überprüfen Sie die Echtheit der in jedem Dokument enthaltenen Unterschriften."

    # feature loop
    - icon: "update"
      title: "Signaturverwaltung"
      content: "Löschen, verschieben oder ändern Sie alle auf einer Dokumentseite platzierten Signaturen."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Anschauliche Beispiele, die typische GroupDocs.Signature for Node.js via Java-Vorgänge veranschaulichen"
  items:
    # code sample loop
    - title: "PDF mit QR-Codes markieren"
      content: |
        Durch die Einbindung von [Barcodes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) in bestimmte PDF-Dokumentseiten können Geschäftsprozesse optimiert werden. Dieser Abschnitt enthält ein Beispiel für das Hinzufügen eines QR-Codes mit GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="So fügen Sie einen QR-Code in ein PDF ein.">}}
        ```javascript {style=abap}
        // Laden Sie das zu signierende Dokument
        let signature = new Signature("file_to_sign.pdf");
        
        // Erstellen Sie QR-Code-Optionen mit vordefiniertem Text
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurieren Sie den Kodierungstyp und die Position des QR-Codes auf der Seite
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Signieren Sie das Dokument und speichern Sie es als Ergebnisdatei
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Schützen eines DOCX mit einer digitalen Signatur"
      content: |
        [Schützen Sie Ihre Dokumente](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) durch Signaturen basierend auf digitalen Zertifikaten. Digitale Signaturen schützen Ihre Geschäftsdokumente vor Inhaltsänderungen.
        {{< landing/code title="So stellen Sie die Dokumentenintegrität sicher.">}}
        ```javascript {style=abap}   
        // Laden Sie das Dokument, das digital signiert werden soll
        let signature = new Signature("file_to_sign.docx");
        
        // Geben Sie Optionen für die digitale Signatur an und geben Sie den Pfad zur Zertifikatsdatei an
        let options = new DigitalSignOptions("certificate.pfx");

        // Legen Sie das Zertifikatspasswort fest
        options.Password = "1234567890";

        // Signieren Sie das Dokument und speichern Sie es im gewünschten Pfad
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
