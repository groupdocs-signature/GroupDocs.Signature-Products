---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Digital Signature API, Hinzufügen von eSignatur zu PDF Word Excel Image"
head_description: "Java-API für digitale Signaturen. Elektronische Signaturbibliothek zum digitalen Signieren von PDF-, Microsoft Word-, Excel-Tabellen, PowerPoint-Präsentationen und Bilddokumentformaten."

############################# Header ############################
title: "Java-API zum Verwalten digitaler Signaturen"
description: "Verwalten Sie die elektronische Signatur von Bild-, QR-Code-, Barcode-, Metadaten-, Text- und Stempeltypen in Java-Anwendungen zum Signieren von Bildern und digitalen Dokumentdateiformaten."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

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
              text: "Unterstützung"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Live-Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Preisgestaltung"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API unterstützt Sie bei der Entwicklung von Java-Anwendungen mit Funktionen für elektronische Signaturen, um digitale Dokumente in unterstützten Formaten zu signieren, ohne externe Software installieren zu müssen. Es unterstützt die Manipulation und Verwaltung verschiedener Arten von elektronischen Signaturen wie Bild, Barcode, QR-Code, Stempel, Text, optische und Metadaten. Alle Ihre elektronischen Geschäftsdokumente wie Microsoft Office Word, PowerPoint-Präsentationen, Excel-Tabellen, Bilder und PDF-Dateien können digital signiert werden, indem Sie Signatureigenschaften anpassen, z. Schatten, Abmessungen, Ausrichtung und mehr nach Ihren Wünschen. Die digitale Signaturbibliothek ist einfach und leichtgewichtig und besteht aus einer einzigen DLL-Datei, die problemlos in eine neue oder eine vorhandene Java-Anwendung integriert werden kann.  

      Über GroupDocs.Signature for Java API können Sie alle registrierten Zertifikate aus dem System laden oder vorhandene Signaturen mit einer einfachen und erweiterten Suche finden. Die Optionen zum Arbeiten mit passwortgeschützten Dokumenten, das Festlegen gemeinsamer Signatureigenschaften (Textgröße, Deckkraft, Drehung, Überprüfung, Schriftarteigenschaften, Farboptionen, Seitenzahl, Breite, oben, links usw.) und die Unterstützung der Implementierung verschiedener eSignatur-Typen machen es zu einer zuverlässigen E-Signaturen-Verwaltungslösung für digitale Dokumente.  

      GroupDocs.Signature for Java ist mit allen Java-Versionen kompatibel und unterstützt gängige Betriebssysteme (Windows, Linux, MacOS), die Java-Runtime ausführen können
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Das ist eine Übersicht der GroupDocs.Signature-Funktionen für Java:
      
        right:
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
            * Formularfeld-Signatur
      
      ## TAB TWO ##
      tab_two:
        description: |
          Die Java-API für elektronische Signaturen unterstützt [Dokumentdateiformate](https://docs.groupdocs.com/signature/java/supported-document-formats/) wie unten aufgeführt.

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
            - title: "Images & Other Formats"
              content: |
                * **Bilder**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metadateien**: EMF, WMF, CMX
                * **tragbar**: PDF
                * **Skalierbare Vektorgrafiken**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Andere**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java unterstützt folgende Betriebssysteme, Frameworks & Package Manager:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Betriebssysteme"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Unterstützte Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Entwicklungsumgebungen"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build-Automatisierungstool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature für Java-Funktionen"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Elektronische Signaturen aus unterstützten Dokumentformaten erstellen, lesen, ändern, ausblenden und löschen"

      # feature loop
      - icon: "fas fa-eye"
        content: "Zugriff auf ein signiertes Dokument aus Stream, relativem Pfad oder absolutem Pfad"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Wenden Sie eine Textsignatur auf Dokumente, Tabellenkalkulationen, Präsentationen, Bilder und PDF-Dateien an"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Textsignatur als Anmerkung, Aufkleber, Bild zu PDF-Dateien hinzufügen und Stil und Farbe konfigurieren"

      # feature loop
      - icon: "fas fa-code"
        content: "Signieren Sie PDF-Dokumente, Bilddateien und erhalten Sie die Ausgabe in einem anderen Dateiformat"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Signieren Sie Bilder digital mit einer Textsignatur als Wasserzeichen und fügen Sie der eSignatur Transparenz und Rotation hinzu"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Durchsuchen Sie Zertifikate und signieren Sie Microsoft Word-, Excel- und PDF-Dokumente mit digitalen Zertifikaten"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Signieren Sie Textverarbeitungsdokumentformate mit nativen Textwasserzeichen"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Verwenden Sie QR-Code, Barcode, um Word-, Slide-, Cell-, PDF- und Bilddateien zu signieren"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Konfigurieren und wenden Sie Stempelsignaturen an, um unterstützte Dateiformate zu sichern"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Einrichten und Zuweisen von Bildsignaturen zu Dokumenten, Tabellenkalkulationen, Präsentationen, Bildern und PDF-Dateien"

      # feature loop
      - icon: "fas fa-columns"
        content: "Signatureigenschaften konfigurieren, z. B. Aussehen und Verhalten, Ränder, Ausrichtung usw."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Wenden Sie eine digitale Signatur auf ein passwortgeschütztes Dokument an"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Führen Sie eine Textüberprüfung von PDF-Dokumenten mit dem Signatur-Handler durch"

      # feature loop
      - icon: "fas fa-print"
        content: "Digitale Überprüfung von Word-, Cell- und PDF-Dokumenten mit .CER- und .PFX-Zertifikatscontainern"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Geben Sie verschiedene Maßeinheitstypen (z. B. Millimeter, Pixel usw.) für PDF-Textsignaturen an"

      # feature loop
      - icon: "fas fa-lock"
        content: "Abrufen von Dokumentinformationen über Datei oder URL - Hinzufügen von Formularfeldsignaturen zu PDF-Dokumenten"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Fügen Sie dem QR-Code benutzerdefiniertes Datenobjekt, eingebettete VCard, E-Mail, EPC, MeCard oder Event-Objekt hinzu"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Wenden Sie verschiedene Pinselstile auf Signaturen an, z. B. Verlaufs-, Radial-, Vollton- und Texturpinsel"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Unterschreiben Sie das Dokument, das sich auf FTP oder Azure Cloud Storage befindet"

      # feature loop
      - icon: "fas fa-heading"
        content: "Legen Sie die Textausrichtung in Formen für Dokumente, Folien, Bilder und PDF-Dateien fest"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "PowerPoint-Präsentationsdokumente suchen, überprüfen und digital signieren"

      # feature loop
      - icon: "fas fa-cube"
        content: "Platzieren Sie die Signatur mithilfe von Pixeln in Zelldokumenten und Textpositionierung für Stempelsignaturen"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementieren Sie eine rechteckige Stempelsignatur mit abgerundeten Ecken"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Erweitern Sie Barcode- und QR-Code-Signaturen mit Bilddateninhalten"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Fügen Sie verschlüsselte Metadatensignaturen hinzu, während Sie mit Signier- und Suchoptionen arbeiten"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Betten Sie benutzerdefinierte Objekte in Metadaten-Signaturen in Word, Excel und Präsentationen ein"

    more_feature:
      # more_feature_loop
      - title: "eSignaturen einfach konfigurieren und anwenden"
        content: |
          GroupDocs.Signature for Java API ermöglicht das Konfigurieren und Hinzufügen von eSignaturen zu unterstützten Dokumentformaten. Das folgende Codebeispiel zeigt, wie einfach es ist, eine Textsignatur auf eine PDF-Datei anzuwenden:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // Signaturposition festlegen
          options.setLeft(100);
          options.setTop(100);
          
          // Unterschriftsrechteck setzen
          options.setWidth(100);
          options.setHeight(30);

          // Stellen Sie Textfarbe und Schriftart ein
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // Unterschreiben Sie das Dokument, um es zu archivieren
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Unterstützte Barcode-Codierungstypen für elektronische Signaturen"
        content: |
          Mit GroupDocs.Signature for Java API können Sie Barcode- und QR-Code-Signaturen auf unterstützte Dateiformate anwenden. GroupDocs.Signature für Java unterstützt eine große Auswahl an Barcode-Codierungstypen, um den meisten Anforderungen gerecht zu werden. Zu den unterstützten Barcode-Codierungstypen gehören Code 11, Code 128, Code 16K/32, Databar Codes, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard und Code39 erweitert.

          In ähnlicher Weise können Sie mit GroupDocs.Signature for Java API QR-Code-Typen wie QR, Aztec und Data Matrix verwenden. Zu den unterstützten QR-Code-Codierungstypen gehören Aztec, DataMatrix, GS1 DataMatrix und GS1 QR.

      # more_feature_loop
      - title: "Suchen Sie nach Signaturen und Zertifikaten"
        content: |
          Über GroupDocs.Signature for Java API können Sie QR-Code- und Barcode-Signaturen in allen Dokumenten, Präsentationen, Tabellenkalkulationen, Bildern sowie PDF-Dateien suchen und das Suchergebnis abrufen. Sie können auch benutzerdefinierte Datenobjekte aus mit QR-Code-Signatur signierten Dokumenten sowie Standard-VCard- und E-Mail-Objekte aus mit QR-Code signierten Dokumenten durchsuchen. Die Überprüfung des verschlüsselten Textes von QR-Code-Signaturen sowie die Suche nach Metadaten-Signaturen in PDF-Dokumenten wird ebenfalls unterstützt. Wenden Sie zusätzliche Suchkriterien für digitale Signaturen von Words & Cells-Dokumenten an.  

          Die Suchoption ist auch für Metadaten-Signaturen für Word-Dokumente, Folien und Tabellenkalkulationen verfügbar, während die Formularfeldsuche für PDF-Dokumente verfügbar ist.

      # more_feature_loop
      - title: "Konfigurieren Sie eSignatur-Eigenschaften"
        content: |
          Um die UX von Endbenutzern zu verbessern, bietet GroupDocs.Signature for Java API viele Eigenschaften, die ziemlich einfach konfiguriert werden können. Sie können Schriftart- und Farboptionen (Hintergrundfarbe, Vordergrundfarbe, Fett, Kursiv, Unterstrichen, Schriftfamilie, Schriftgröße usw.), Hintergrund- und Rahmenoptionen (Hintergrundfarbe, Hintergrundtransparenz, Rahmenfarbe, Rahmenstrichstil, Rahmenstärke, Rahmentransparenz usw.), Unterschriftsränder (Links, Oben, Breite, Höhe, Auffüllung usw.) und Einrichtung des Bildunterschriftsbereichs und der Unterschriftsausrichtung (Horizontale Ausrichtung, Vertikale Ausrichtung usw.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature bietet APIs zum Anzeigen von Dokumenten für andere beliebte Entwicklungsumgebungen"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---