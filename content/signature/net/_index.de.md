---
############################# Static ############################
layout: "landing"
date: 2024-09-25T12:45:24
draft: false

lang: de
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

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
head_title: "C# .NET-API für digitale Signaturen – GroupDocs.Signature"
head_description: "Integrieren Sie die Verarbeitung digitaler Signaturen in Ihre .NET-Apps mit GroupDocs.Signature. Sichern Sie Ihre Dateien schnell und effizient mit Signaturen."

############################# Header ############################
title: "Dokumente unterschreiben über die .NET-API"
description: "Signieren Sie digitale Dokumente und Bilder auf jeder Plattform mit unseren flexiblen APIs und App-basierten Lösungen für Programmierer und Endbenutzer."
words:
  for: "für"

actions:
  main: "Kostenloser NuGet-Download"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net/"
  title: "Bereit anzufangen?"
  description: "Testen Sie die Funktionen von GroupDocs.Signature kostenlos oder fordern Sie eine Lizenz an"

release:
  title: "Version {0} veröffentlicht"
  notes: "Schau was neu ist"
  downloads: "Downloads"

code:
  title: "PDF-Dateien in C# signieren"
  more: "Mehr Beispiele"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // PDF-Dokument auswählen
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Text bereitstellen
        var options = new TextSignOptions("John Smith")
        {
            // Farbe einstellen
            ForeColor = Color.Red
        };
        // Dokument unterschreiben und in Datei speichern
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature-Übersicht"
  description: "API zum Durchführen der Dokumentensignierung und verwandter Vorgänge in .NET-Anwendungen"
  features:
    # feature loop
    - title: "Hinzufügen von Signaturen zu Geschäftsdokumenten in C#"
      content: "Signieren von Dokumenten: Mit GroupDocs.Signature für .NET können Sie PDF- und Office-Dokumenten verschiedene Arten von Signaturen hinzufügen, z. B. Text, Bilder, Barcodes und digitale Zertifikate. Mit dieser API können Sie Ihre Dokumente mit nahezu jedem Datentyp signieren, einschließlich versteckter Metadaten."

    # feature loop
    - title: "Bearbeitung signierter Dokumente"
      content: "Zusätzliche Verarbeitung: Mit GroupDocs.Signature können Sie leistungsstarke Vorgänge an signierten Dokumenten durchführen. Dazu gehört die Suche nach vorhandenen Signaturen in Geschäftsdokumenten und deren Überprüfung anhand bestimmter Kriterien. Darüber hinaus können Sie über diese .NET-API Dokumentinformationen und Vorschauseiten abrufen."

    # feature loop
    - title: "Anpassen der Ergebnisse"
      content: "GroupDocs.Signature für .NET bietet umfangreiche Anpassungsmöglichkeiten. Sie können Signaturen überall auf einer Dokumentseite präzise positionieren und ihr Erscheinungsbild mithilfe verschiedener Einstellungen anpassen. Darüber hinaus unterstützt diese API das Speichern verarbeiteter Dokumente in einer Vielzahl unterstützter Formate."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Signature für .NET unterstützt die folgenden Betriebssysteme, Frameworks und Paketmanager"
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
    GroupDocs.Signature für .NET unterstützt Vorgänge mit den folgenden [Dateiformaten](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  title: "GroupDocs.Signature-Funktionen"
  description: "PDFs, Office-Dokumente und Bilder schnell und präzise signieren"

  items:
    # feature loop
    - icon: "sign"
      title: "Unterzeichnung des Dokuments"
      content: "Fügen Sie eine oder mehrere unterstützte Signaturarten präzise an jeder angegebenen Position in Geschäftsdokumenten hinzu."

    # feature loop
    - icon: "custom"
      title: "Passen Sie Signaturen an"
      content: "Nutzen Sie Funktionen wie Farbe, Schriftart, Rahmen, Drehung usw., um das Erscheinungsbild von Signaturen zu konfigurieren."

    # feature loop
    - icon: "password"
      title: "Passwortschutz für Dokumente"
      content: "Sichern Sie bestimmte Dokumenttypen, indem Sie nach dem Signieren ein Passwort festlegen."

    # feature loop
    - icon: "protect"
      title: "Schutz vor Veränderungen"
      content: "Verhindern Sie Änderungen an wichtigen Geschäftsdokumenten, nachdem Sie eine Signatur mit einem digitalen Zertifikat angehängt haben."

    # feature loop
    - icon: "convert"
      title: "Konvertieren Sie signierte Dateien in andere Formate"
      content: "Konvertieren Sie signierte Dateien in gewünschte Formate, z. B. Speichern eines Word-Dokuments als PDF."

    # feature loop
    - icon: "preview"
      title: "Extrahieren Sie Seitenvorschauen"
      content: "Extrahieren Sie Seiten aus signierten Dokumenten als einzelne Bilder für die zukünftige Verarbeitung."

    # feature loop
    - icon: "search"
      title: "Signatursuche in Dokumenten"
      content: "Rufen Sie Informationen zu zuvor hinzugefügten Signaturen in bestimmten Dokumenten ab."

    # feature loop
    - icon: "validate"
      title: "Validieren Sie signierte Dokumente"
      content: "Überprüfen Sie die ordnungsgemäße Signatur von Dokumenten mithilfe von Validierungsfunktionen."

    # feature loop
    - icon: "update"
      title: "Signaturen aktualisieren oder löschen"
      content: "Positionieren Sie bestimmte Signaturen ganz einfach auf einer Seite neu, ändern Sie ihren Text oder löschen Sie sie ohne Probleme."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Einige Anwendungsfälle typischer GroupDocs.Signature für .NET-Vorgänge"
  items:
    # code sample loop
    - title: "QR-Code zum PDF hinzufügen"
      content: |
        Das Hinzufügen von [QR-Codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) zu bestimmten Seiten von PDF-Dokumenten kann Geschäftsprozesse verbessern. Nachfolgend finden Sie ein Beispiel für das Hinzufügen eines QR-Codes mithilfe von GroupDocs.Signature.
        {{< landing/code title="So fügen Sie einen QR-Code in ein PDF ein.">}}
        ```csharp {style=abap}
        // Laden Sie das zu signierende Dokument
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Erstellen Sie QR-Code-Optionen mit vordefiniertem Text
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Konfigurieren Sie den Kodierungstyp und die Position des QR-Codes auf der Seite
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Signieren Sie das Dokument und speichern Sie es als Ergebnisdatei
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Schützen eines DOCX-Dokuments mithilfe eines digitalen Zertifikats"
      content: |
        Sie können [ein Dokument schützen](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/), indem Sie persönliche oder Unternehmenssignaturen verwenden, die als digitale Zertifikate gespeichert sind. Solche geschützten Dokumente können nicht geändert werden, ohne dass die Signatur ungültig wird.
        {{< landing/code title="So stellen Sie die Dokumentenintegrität sicher.">}}
        ```csharp {style=abap}   
        // Laden Sie das Dokument, das digital signiert werden soll
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Geben Sie Optionen für die digitale Signatur an und geben Sie den Pfad zur Zertifikatsdatei an
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Legen Sie das Zertifikatspasswort fest
                Password = "1234567890"
            };
            // Signieren Sie das Dokument und speichern Sie es im gewünschten Pfad
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---