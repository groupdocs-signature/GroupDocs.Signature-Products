---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:21
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: de
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, Cloud-APIs und Online-Dokumentensignatur-Apps"
head_description: "Holen Sie sich eine All-in-One-Dokumenten-E-Signatur-Lösung für .NET-, Java- und Cloud-basierte Anwendungen. Signieren Sie gängige Dokumentenformate online mit der einfachen Drag-and-Drop-Funktion"

############################# Header ############################
title: "Dokumente unterschreiben<br>über Java API"
description: "Signieren Sie digitale Dokumente und Bilder auf jeder Plattform mit unseren flexiblen APIs und App-basierten Lösungen für Programmierer und Endbenutzer."
words:
  for: "für"

actions:
  main: "Kostenloser Maven-Download"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Bereit anzufangen?"
  description: "Testen Sie die Funktionen von GroupDocs.Signature kostenlos oder fordern Sie eine Lizenz an"

release:
  title: "Version {0} veröffentlicht"
  notes: "Schau was neu ist"
  downloads: "Downloads"

code:
  title: "Signieren Sie PDF-Dateien in Java"
  more: "Mehr Beispiele"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // PDF-Dokument auswählen
    Signature signature = new Signature("sample.pdf");
    
    // Text bereitstellen
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Dokument unterschreiben und in Datei speichern
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature-Übersicht"
  description: "API zum Durchführen der Dokumentensignierung und verwandter Vorgänge in Java-Anwendungen"
  features:
    # feature loop
    - title: "Verbesserte Geschäftsdokumente mit digitalen Signaturen in Java"
      content: "Schnelles und anpassbares Signieren: GroupDocs.Signature für Java bietet eine breite Palette digitaler Signaturoptionen für PDFs, Bilder und Office-Dokumente. Sie können Text, Barcodes, QR-Codes, digitale Zertifikate, Bilder oder versteckte Metadaten verwenden. Die Dokumentenverarbeitung ist schnell und effizient."

    # feature loop
    - title: "Manipulation signierter Dokumente"
      content: "Die erweiterte Dokumentenverarbeitung umfasst leistungsstarke Vorgänge an signierten Dokumenten mithilfe von GroupDocs.Signature für Java. Sie können anhand verschiedener nützlicher Kriterien nach Signaturen suchen und diese validieren, die Geschäftsdokumenten hinzugefügt wurden. Darüber hinaus können Sie detaillierte Informationen zum Dokument abrufen oder Vorschaubilder seiner Seiten abrufen."

    # feature loop
    - title: "Vielzahl von Ausgabeoptionen"
      content: "Mithilfe robuster Signaturoptionen können Sie die Ausgabe für mit GroupDocs.Signature für Java signierte Dokumente anpassen. Sie können jede Signatur auf jeder Dokumentseite präzise positionieren und ihr Erscheinungsbild auf verschiedene Weise konfigurieren. Die Java-API unterstützt das Speichern signierter Geschäftsdokumente in zahlreichen unterstützten Formaten und bietet Möglichkeiten, diese mit Passwörtern zu sichern."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Signature für Java unterstützt die folgenden Betriebssysteme, Frameworks und Paketmanager"
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Unterstützte Dateiformate"
  description: |
    GroupDocs.Signature für Java unterstützt Vorgänge mit den folgenden [Dateiformaten](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  description: "Signieren von PDFs, Office-Dokumenten und Bildern mit digitalen Signaturen"

  items:
    # feature loop
    - icon: "sign"
      title: "Signaturen hinzufügen"
      content: "Signieren Sie ein Dokument mit verschiedenen unterstützten Signaturtypen, indem Sie eine digitale Signatur genau an jeder Position auf jeder Seite platzieren."

    # feature loop
    - icon: "custom"
      title: "Anpassen der Ergebnisse"
      content: "Passen Sie das Erscheinungsbild der Signatur an, indem Sie Farbe, Schriftart, Rahmen, Drehung und andere Funktionen anpassen, um das gewünschte Ergebnis zu erzielen."

    # feature loop
    - icon: "password"
      title: "Dokumente mit Passwort sichern"
      content: "Bei vielen unterstützten Dokumenttypen können Sie das signierte Dokument mit einem Passwort schützen."

    # feature loop
    - icon: "protect"
      title: "Verhindern Sie unbefugte Änderungen"
      content: "Schützen Sie wichtige, mit einem digitalen Zertifikat signierte Geschäftsdokumente vor unbefugten Änderungen."

    # feature loop
    - icon: "convert"
      title: "Erzielen von Ergebnissen in gewünschten Formaten"
      content: "Erhalten Sie ganz einfach signierte Ergebnisdateien in jedem unterstützten Format. Sie können MS Word-Dokumente auch mühelos in PDF konvertieren."

    # feature loop
    - icon: "preview"
      title: "Dokumentvorschau"
      content: "Speichern Sie jede Seite eines Dokuments als Bild für die zukünftige Verarbeitung."

    # feature loop
    - icon: "search"
      title: "Suche nach Unterschriften"
      content: "Es ist möglich, Informationen über zuvor hinzugefügte Signaturen in bestimmten Dokumenten abzurufen."

    # feature loop
    - icon: "validate"
      title: "Dokumente validieren"
      content: "Überprüfen Sie die Richtigkeit der Unterschriften auf jedem unterzeichneten Dokument."

    # feature loop
    - icon: "update"
      title: "Signaturen verwalten"
      content: "Sobald eine Signatur auf einer Dokumentseite platziert ist, kann sie nach Bedarf gelöscht, verschoben oder aktualisiert werden."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Einige Anwendungsfälle typischer GroupDocs.Signature für Java-Operationen"
  items:
    # code sample loop
    - title: "PDF-Dokument mit QR-Code erweitern"
      content: |
        Die Verbesserung von Geschäftsprozessen durch das Hinzufügen von [QR-Codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) zu bestimmten Seiten von PDF-Dokumenten kann wertvoll sein. Es gibt ein Beispiel für das Hinzufügen eines QR-Codes mit GroupDocs.Signature für Java.
        {{< landing/code title="PDF-Dokument mit QR-Code erweitern">}}
        ```java {style=abap}
        // Laden Sie das zu signierende Dokument
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Erstellen Sie QR-Code-Optionen mit vordefiniertem Text
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurieren Sie den Kodierungstyp und die Position des QR-Codes auf der Seite
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Signieren Sie das Dokument und speichern Sie es als Ergebnisdatei
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Verwenden Sie eine digitale Signatur, um ein DOCX zu schützen"
      content: |
        Sie können [ein Dokument schützen](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/), indem Sie persönliche oder Unternehmenssignaturen verwenden, die als digitale Zertifikate gespeichert sind. Mit einem Zertifikat gesicherte Dokumente können nicht verändert werden, ohne dass die Signatur ungültig wird.
        {{< landing/code title="Verwenden Sie eine digitale Signatur, um ein DOCX zu schützen">}}
        ```java {style=abap}   
        // Laden Sie das Dokument, das digital signiert werden soll
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Geben Sie Optionen für die digitale Signatur an und geben Sie den Pfad zur Zertifikatsdatei an
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Legen Sie das Zertifikatspasswort fest
        options.setPassword("1234567890");

        // Signieren Sie das Dokument und speichern Sie es im gewünschten Pfad
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
