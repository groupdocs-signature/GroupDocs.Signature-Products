---
############################# Static ############################
layout: "family"
date:  2024-07-25T14:25:12
draft: false

product: "Signature"
product_tag: "signature"

lang: de

############################# Head ############################
head_title: "C# .NET, Java, Node.js digitale Signatur-Apps"
head_description: "Integrieren Sie elektronische Signaturen in .NET-, Java- oder Node.js-Anwendungen mit GroupDocs.Signature. Unterzeichnen Sie gängige Geschäftsdokumentformate."

############################# Header ############################
title: "E-Signatur-Lösung für Dokumente"
description:  |
  Signieren Sie digitale Dokumente und Bilder auf jeder Plattform mit unseren flexiblen APIs und App-basierten Lösungen für Programmierer und Endbenutzer.

  Suchen und ändern Sie zuvor hinzugefügte Signaturen mit erweiterten Methoden.

  Schützen Sie Dokumente mit digitalen Zertifikaten vor Änderungen und kontrollieren Sie versteckte Metadaten.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Wählen Sie Ihre Plattform"
  title: "Plattformunabhängigkeit"
  description: "Die Bibliothek GroupDocs.Signature unterstützt die folgenden Betriebssysteme und Frameworks:"
  details_link_title: "Erfahren Sie mehr"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Signature .NET 
      color: "blue"
      tag: "net"
      link: "/signature/net/"
      features_link: "https://docs.groupdocs.com/signature/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.6.2 or higher <br> .NET Core 3.0 or higher <br> .NET 6.0 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS <br> Microsoft Azure
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio <br> JetBrains Rider <br> Microsoft Visual Code
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Signature Java
      color: "red"
      tag: "java"
      link: "/signature/java/"
      features_link: "https://docs.groupdocs.com/signature/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java 8 or higher
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    IntelliJ IDEA <br> Eclipse <br> NetBeans
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

    # items loop
    - title: "Node.js"
      description: GroupDocs.Signature Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/signature/nodejs-java/"
      features_link: "https://docs.groupdocs.com/signature/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Jeder andere Texteditor
      
          # features loop
          - rows: "1"
            content: |
                    60+ file formats

############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Signature Hauptfunktionen"
  description: "Unsere Lösung ist darauf ausgelegt, gängige Dokument- und Dateiformate mit verschiedenen Arten von Signaturen zu versehen. Bereichern Sie Ihre Geschäftsprozesse ganz einfach."

  items:
    # items loop
    - icon: "additional"
      title: "Bereichern Sie Ihre Daten mit Signaturen"
      content: "Fügen Sie Text, Bilder, Wasserzeichen usw. zu Ihren Geschäftsdokumenten hinzu."

    # items loop
    - icon: "protect"
      title: "Schützen Sie den Inhalt von Dokumenten"
      content: "Verhindern Sie Dokumentänderungen, indem Sie es mit einem digitalen Zertifikat versiegeln."

    # items loop
    - icon: "search"
      title: "Fügen Sie versteckte Daten und Barcodes hinzu"
      content: "Verwenden Sie Metadaten, um unsichtbare Informationen zu speichern oder benutzerdefinierte Barcodes auf Seiten anzubringen."

    # items loop
    - icon: "manipulate"
      title: "Signaturen manipulieren"
      content: "Suchen, aktualisieren oder löschen Sie alle zuvor hinzugefügten Signaturen."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Schützen Sie Ihre Dateien mit Signaturen"
  description: "GroupDocs.Signature Codebeispiele"
  items:
    # code sample loop
    - title: "QR-Code generieren und hinzufügen"
      content: |
       Mit GroupDocs.Signature können wir QR-Codes generieren und zu Dokumenten mit unterstützten Formaten hinzufügen. Geben Sie den Pfad zu einem Dokument an, das signiert werden muss, und richten Sie die gewünschten Text- und visuellen Optionen für den QR-Code ein. Sie können das generierte QR-Code-Bild in einem beliebigen Bereich einer beliebigen Dokumentseite platzieren.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Geben Sie das Dokument zum Signieren an
            using (Signature signature = new Signature("source.docx"))
            {
                // Erstellen Sie Optionen für QR-Code-Zeichen
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // Legen Sie QR-Code-Optionen fest
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150,
                };

                // Unterzeichnen und speichern Sie die verarbeitete Datei
                SignResult result = signature.Sign("result.docx", options);
            }
            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Geben Sie das Dokument zum Signieren an
            Signature signature = new Signature("source.docx");

            // Erstellen Sie Optionen für QR-Code-Zeichen
            QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith");

            // Legen Sie QR-Code-Optionen fest
            options.setEncodeType(QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Unterzeichnen und speichern Sie die verarbeitete Datei
            signature.sign("result.docx", options);
            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}  
            const signatureLib = require('@groupdocs/groupdocs.signature')

            // Geben Sie das Dokument zum Signieren an
            const signature = new signatureLib.Signature('source.docx');

            // Erstellen Sie Optionen für QR-Code-Zeichen
            const options = new signatureLib.QrCodeSignOptions('JohnSmith');

            // Legen Sie QR-Code-Optionen fest
            options.setEncodeType(signatureLib.QrCodeTypes.QR);
            options.setLeft(50);
            options.setTop(100);

            // Unterzeichnen und speichern Sie die verarbeitete Datei
            signature.sign('result.docx', options);
            ```

############################# Supported Formats ###############################
formats:
  enable: true
  title: "Über 60 Dateiformate werden unterstützt"
  description: "GroupDocs.Signature unterstützt fast alle gängigen Dateiformate"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Statistische Daten unserer Bibliothek"
  description: "Untersuchen Sie wichtige Produktkennzahlen und geben Sie Einblicke in unsere Erfolge, Auswirkungen und unser Wachstum"

  items:
    # items loop
    - number: "50+"
      title: "Unterstützte Formate"
      content: "Signieren von mehr als 60 der beliebtesten Geschäftsdateiformate."

    # items loop
    - number: "500k"
      title: "NuGet-Downloads"
      content: "GroupDocs.Signature für .NET ist eine beliebte Bibliothek mit über 550.000 Downloads auf NuGet."

    # items loop
    - number: "15k"
      title: "Maven-Downloads"
      content: "Java-Entwickler haben GroupDocs.Signature mehr als 15.000 Mal auf Maven heruntergeladen."

    # items loop
    - number: "140+"
      title: "Zufriedene Kunden"
      content: "Einzelne Entwickler und Top-Unternehmen weltweit nutzen unsere Produkte, um innovative Lösungen zu entwickeln."


############################# Customers ###############################
customers:
  enable: true
  title: "Unsere zufriedenen Kunden"
  description: "GroupDocs-Bibliotheken werden von weltweit bekannten und angesehenen Marken auf der ganzen Welt eingesetzt"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Bereit anzufangen?"
  description: "Testen Sie die Funktionen von GroupDocs.Signature kostenlos auf Ihrer Plattform"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/signature/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/signature/java/"

    # items loop
    - title: "Node.js"
      color: "green"
      link: "/signature/nodejs-java/"      

############################# FAQ ###############################
faq:
  enable: true
  title: "Häufig gestellte Fragen"
  description: "Entdecken Sie unsere häufig gestellten Fragen"

  items:
    # items loop
    - question: "Benötigt GroupDocs.Signature eine externe Bibliothek zum Signieren von Dokumenten?"
      answer: "Nein, GroupDocs.Signature funktioniert unabhängig. Es gibt keine Abhängigkeiten von Drittanbietern wie Adobe Acrobat, Microsoft Office usw."

    # items loop
    - question: "Ist es möglich, die Funktionen von GroupDocs.Signature vor dem Kauf zu testen?"
      answer: "Absolut! GroupDocs.Signature bietet eine kostenlose Testversion an. Installieren Sie es und erkunden Sie seine Funktionen. Beachten Sie, dass Testversionen Ihren Dokumenten „Testabzeichen“ hinzufügen und nur die ersten drei Seiten verarbeiten. Um das volle Erlebnis zu genießen, erwerben Sie eine kostenlose 30-tägige temporäre Lizenz, um auf alle Funktionen zuzugreifen. Einzelheiten finden Sie unter [temporäre Lizenz](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Welche Lizenztypen werden angeboten?"
      answer: "Suchen Sie nach einer GroupDocs.Signature-Lizenz? Wir bieten verschiedene Optionen an, die auf Ihre Bedürfnisse zugeschnitten sind. Wählen Sie basierend auf der Teamgröße, den Einsatzorten (Einzelbüro oder Remote-Arbeitsplätze) und ob die Endkundenverteilung die gemeinsame Nutzung des SDK/der API mit Kunden erfordert. Alternativ können Sie sich für eine monatliche Nutzungslizenz mit getakteten Plänen entscheiden – Sie zahlen nur für das, was Sie nutzen. Entdecken Sie unter [Preise](https://purchase.groupdocs.com/pricing/signature/net/), welche Lösung für Sie am besten geeignet ist."

############################# Cloud Links ###############################
cloud_links:
  enable: true
  title: "GroupDocs.Signature Low-Code-APIs"
  description: "Signieren Sie Dateien mit Ihrer Anwendung über unsere cloudbasierte REST-API."
  
  items:
    # items loop
    - title: "GroupDocs.Signature Cloud for cURL"
      content: "Verwenden Sie die cURL RESTful API, um Signaturen in PDF, Word, Excel, PowerPoint, JPEG und viele andere Dateiformate einzufügen."
      icon: "groupdocs_signature-for-curl"
      link: "https://products.groupdocs.cloud/signature/curl"

    # items loop
    - title: "GroupDocs.Signature Cloud for .NET"
      content: "Bereichern Sie Ihre .NET-Anwendungen mit der Signatur von Dokumenten über das Cloud SDK. Schützen Sie Geschäftsdokumente auf Ihre eigene Art und Weise."
      icon: "groupdocs_signature-for-net"
      link: "https://products.groupdocs.cloud/signature/net"

    # items loop
    - title: "GroupDocs.Signature Cloud for Java"
      content: "Das GroupDocs.Signature SDK gewährt Ihren Java-Anwendungen Zugriff auf verschiedene Möglichkeiten zum Signieren beliebiger Dateien."
      icon: "groupdocs_signature-for-java"
      link: "https://products.groupdocs.cloud/signature/java"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Signature Web-Apps"
  description: "GroupDocs.Signature präsentiert eine kostenlose Webanwendung, mit der Sie Dokumente signieren können. Mehr als 60 gängige Dateiformate können KOSTENLOS über Ihren Lieblingsbrowser signiert werden."

  items:
    # items loop
    - title: "GroupDocs.Signature Total"
      content: "Online-Tool zum Signieren von Dokumenten von jedem Gerät aus."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/signature/total"

    # items loop
    - title: "GroupDocs.Signature DOCX"
      content: "Signieren Sie MS Word DOCX online."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/signature/docx"

    # items loop
    - title: "GroupDocs.Signature PDF"
      content: "Schützen Sie PDF-Dokumente online."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/signature/pdf"


      


---