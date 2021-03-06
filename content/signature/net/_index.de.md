---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET-API für digitale Signaturen – Elektronisches Signieren von PDF-Word-Excel-Bildern"
head_description: "C# .NET-API für digitale Signaturen, Bibliothek für elektronische Signaturen zum elektronischen Signieren von PDF-, Word-, Excel-Tabellen, PowerPoint-, Bild- und Grafikdokumentformaten."

############################# Header ############################
title: "Einheimisch .NET-API für elektronische Signaturen"
description: "Fügen Sie Dokumentenformaten digitale Signaturen hinzu und implementieren Sie beliebte eSignaturtypen (Text, Bild, QR-Code, Barcode, Stempel und Metadaten) in .NET-Anwendungen."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "/border/groupdocs-signature-net.svg"
        product: "GroupDocs.Signature"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Überblick"

            # button loop
            - link: "#features"
              text: "Merkmale"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/net"
              text: "Preisgestaltung"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Überblick ############################
overview:
    enable: true
    content: |
      Verwenden Sie GroupDocs.Signature for .NET API, um Anwendungen in C#, ASP.NET und anderen .NET-basierten Technologien zu erstellen, mit denen Sie digitale Geschäftsdokumente wie PDF, Microsoft Word, Excel-Tabellen, PowerPoint-Präsentationen, Bilder, OpenDocument und mehr signieren können andere branchenübliche Dateiformate, ohne dass zusätzliche Software installiert werden muss. Diese Bibliothek für elektronische Signaturen ist einfach zu handhaben, und .NET-Entwickler können ihren Anwendungen problemlos erweiterte Funktionen für digitale Signaturen hinzufügen, die es Benutzern ermöglichen, elektronische Signaturen aus gängigen Dokumentformaten sicher zu signieren, zu suchen und zu überprüfen. Es unterstützt die Implementierung einer Vielzahl von Signaturtypen wie Text, Bild, Barcode, QR-Code, Formularfeld, Stempel und Metadaten.

      Die Dokumentensignatur-API bietet Ihnen einfache und erweiterte Suchoptionen, um Ihre erforderlichen Signaturen auf einem Dokument im Handumdrehen zu finden. Die Optionen zum Anwenden von Signaturstilen, Erscheinungsbildmanagement und Anpassen von Signatureigenschaften wie Abmessungen, Schatten, Ausrichtung und mehr sind ebenfalls mit dieser funktionsreichen API zum Signieren von Dokumenten möglich.

      GroupDocs.Signature für .NET kann in jeder Entwicklungsumgebung verwendet werden, die die .NET-Plattform unterstützt. Es ist mit allen .NET-basierten Sprachen kompatibel und unterstützt gängige Betriebssysteme (Windows, Linux, MacOS), auf denen Mono- oder .NET-Frameworks (einschließlich .NET Core) installiert werden können.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Nachfolgend finden Sie eine Übersicht über GroupDocs.Signature für .NET:
      
        left:
          enable: true
          icon: "fab fa-html5"
          title: "Signaturtypen"
          content: |
            * Textsignatur
            * Bildsignatur
            * Digitale Signaturen
            * QR-Code-Signatur
            * Barcode-Signatur
            * Stempel Unterschrift
            * Metadaten-Signatur
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Signature für .NET unterstützt die Anzeige aller gängigen [Dokumentdateiformate](https://docs.groupdocs.com/signature/net/supported-document-formats/). Mit nur wenigen Codezeilen können Sie Ihren .NET-Anwendungen PDF-Signaturen, Microsoft Office Word, Excel-Tabellen, Bilder, HTML, Outlook-E-Mails, OneNote, Project und Grafikanzeigefunktionen hinzufügen.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Andere Formate"
              content: |
                * **Bilder**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **JPEG2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metadateien**: EMF, WMF, CMX
                * **Tragbar**: PDF
                * **Skalierbare Vektorgrafiken**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Andere**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for .NET unterstützt das Folgen Betriebssysteme, Frameworks & Paket-Managers:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Betriebssysteme"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Unterstützte Frameworks"
              content: |
                * .NET Framework 2.0 oder höher
                * Mono Framework 1.2 oder höher
                * .NET-Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Paket-Manager"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Entwicklungsumgebungen"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Merkmale ############################
features:
    enable: true
    title: "GroupDocs.Signature for .NET Merkmale"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Erstellen, suchen, aktualisieren, verbergen, überprüfen und löschen Sie elektronische Signaturen aus unterstützten Dokumentformaten"

      # feature loop
      - icon: "fas fa-eye"
        content: "Geben Sie XML Advanced Electronic Signatures (XAdES) für Excel-Tabellen an"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Retrieve Image Content from Documents Signed with QR-Code, BarCode & Bildsignaturs"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Höhe, Breite, Ränder & Ausrichtung für Text oder Bildsignatur festlegen & auf bestimmter Seite platzieren"

      # feature loop
      - icon: "fas fa-code"
        content: "PowerPoint-Präsentationsdokumente suchen, überprüfen und digital signieren"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Signieren Sie Textverarbeitungsdokumentformate mit nativen Textwasserzeichen"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Wenden Sie Text- oder Bildsignatur auf einem bestimmten Excel-Blatt an oder legen Sie die elektronische Signatur für alle Blätter fest"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Geben Sie eine bestimmte Zeilen- und Spaltennummer an, um Text oder Bildsignatur in der Excel-Tabelle zu platzieren"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Wenden Sie Schatten auf die Textsignatur in Microsoft PowerPoint an und richten Sie Farbe, Winkel und Transparenz ein"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Konfigurieren Sie Textsignatur-Rahmenstile und Schriftartoptionen für Excel-Tabellen"

      # feature loop
      - icon: "fas fa-columns"
        content: "Bildsignaturtyp einstellen, z.B. Rund oder Quadratisch & Ränder, Schriftfarbe, Rotation konfigurieren"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Wenden Sie digitale Zertifikate auf Dokumente, Tabellenkalkulationen und PDF-Dateien mit Signaturzeile an"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Führen Sie Farbeinstellungen durch, wenden Sie Transparenz und Drehung auf die Textsignatur an"

      # feature loop
      - icon: "fas fa-print"
        content: "Richten Sie Helligkeits- und Graustufenoptionen ein und legen Sie den Einzug der Bildsignatur in einem Bild fest"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Benutzerdefinierte Objekte einbetten, serialisieren sowie Metadaten-Signaturwerte von PDF-Dokumenten verschlüsseln und entschlüsseln"

      # feature loop
      - icon: "fas fa-lock"
        content: "Ausblenden, Entfernen oder Anpassen des Erscheinungsbilds digitaler Signaturen aus PDF-Dokumenten"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Signieren Sie PDF-Dokumente mit digitalem Formularfeld und Textsignatur als Bild, Anmerkung, Aufkleber oder Wasserzeichen"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Fügen Sie Textsignatur in Formularfelder von MS Word- und PDF-Dokumenten ein"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Geben Sie beliebige Seiten von Dokumenten für die Verarbeitung der Signatur oder die erweiterte Überprüfung der elektronischen Signatur für Word-Dateien an"

      # feature loop
      - icon: "fas fa-heading"
        content: "Speichern Sie eine signierte Bilddatei in einem anderen Format und exportieren Sie eine signierte Tabelle als Bild oder mehrseitiges TIFF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Weisen Sie signierten Dateien Passwörter zu, ändern und entfernen Sie sie und wenden Sie eSignatur auf passwortgeschützte Dateien an"

      # feature loop
      - icon: "fas fa-cube"
        content: "eSign-Arbeitsblätter, PowerPoint-Folien, Word-Dokumente und Bilder mit benutzerdefinierten Objekten in Metadaten"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Richten Sie Signatur-Pinselstile als Vollton, Textur, linearen Verlauf und radialen Verlauf ein"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Signieren Sie Dokumente mit benutzerdefiniertem verschlüsseltem QR-Code-Text oder Daten"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Dateien im DjVu-Format als Bilddokument suchen und signieren"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Extrahieren Sie Dokumentinformationen, z. B. Seitenzahl, über die Datei-URL"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Suchen, signieren und überprüfen Sie CorelDraw-Dateien als Bilddokumente"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Bewahren Sie den Verlauf der verarbeiteten oder gelöschten Signaturinformationen auf, die in den Metadaten gespeichert sind"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Benutzerdefiniertes Datenobjekt, VCard oder E-Mail-Objekt zum QR-Code hinzufügen und verschlüsselten QR-Code in PDF-Dateien überprüfen"

    more_feature:
      # more_feature_loop
      - title: "Easily Add Digitale Signaturen"
        content: |
          Mit GroupDocs.Signature for .NET API können Sie verschiedene Arten von Signaturen zu unterstützten Dateiformaten hinzufügen. Die Signaturtypen wie Text, Bild, Digital, Stempel, QR-Code, Barcode und Metadaten können mit GroupDocs.Signature für .NET angewendet werden. Das folgende Codebeispiel zeigt, wie eine Textsignatur auf ein PDF-Dokument angewendet wird:

          ```cs
          using (Signature signature = new Signature("D:\\sample.pdf"))
          {
            TextSignOptions options = new TextSignOptions("John Smith")
            {
              ForeColor = Color.Red
            };
            signature.Sign("D:\\signed.pdf", options);
          }
          ```
      # more_feature_loop
      - title: "Supported Barcode Signaturtypen"
        content: "Unsere Signaturmanipulations-API bietet Ihnen Funktionen zum Anwenden von Barcode-Signaturen auf unterstützte Dokumentformate. GroupDocs.Signature für .NET unterstützt verschiedene Barcode-Typen wie Code128, Code39Extended, Code39Standard, EAN14, EAN8, ITF14, UPCA und UPCE. Ein statisches Objekt namens „AllTypes“ wird ebenfalls bereitgestellt, um alle registrierten Barcode-Typen zu unterstützen.."

      # more_feature_loop
      - title: "Suchen Sie nach Signaturen und Zertifikaten"
        content: |
          GroupDocs.Signature for .NET API ermöglicht Ihnen die Suche nach digitalen Zertifikaten in Word-Dokumenten, Excel-Tabellen und PDF-Dateien. Sie können auch alle im System registrierten digitalen Zertifikate abrufen. Metadaten-Signaturen können auch in Word-Dokumenten, Excel-Tabellen, Bildern und PDF-Dateien mit GroupDocs.Signature for .NET API gesucht werden.

          Über GroupDocs.Signature for .NET API können Sie QR-Code- und Barcode-Signaturen in allen Dokumenten, Präsentationen, Tabellenkalkulationen, Bildern sowie PDF-Dateien suchen und den Suchfortschritt abrufen. Sie können auch benutzerdefinierte Datenobjekte aus mit QR-Code-Signatur signierten Dokumenten suchen.

      # more_feature_loop
      - title: "Erweiterte Suchoptionen für Barcode"
        content: "Sie können Ihren erforderlichen Barcode über GroupDocs.Signature for.NET API sehr einfach suchen und finden, da unsere Signatur-API erweiterte Suchoptionen bietet. Diese ermöglichen es Ihnen, Barcodes auf einer bestimmten Seite zu suchen, ein Dokument zu durchsuchen, verschiedene zu durchsuchende Seiten anzugeben (erste, letzte, gerade, ungerade), nach Barcodes mit einem bestimmten Codierungstyp zu suchen, Barcodes basierend auf einer bestimmten Textzeichenfolge zu suchen oder Barcodes zu suchen basierend auf einer Zeichenfolge mit der Option enthält"

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature bietet APIs zum Anzeigen von Dokumenten für andere beliebte Entwicklungsumgebungen"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for Java"
          image: "/border/groupdocs-signature-java.svg"
          product: "GroupDocs.Signature"
          platform: "Java"
          link: "/signature/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---