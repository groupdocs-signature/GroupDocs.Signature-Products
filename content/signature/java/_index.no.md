---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:49
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: no
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

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

############################# Head ############################
head_title: "Java Digital Signature Library - GroupDocs.Signature"
head_description: "Styr Java-apper med e-signaturer med GroupDocs.Signature. Signer forretningsdokumenter raskt og enkelt."

############################# Header ############################
title: "Signer dokumenter<br>via Java API"
description: "Signer digitale dokumenter og bilder på hvilken som helst plattform ved å bruke våre fleksible APIer og appbaserte løsninger for programmerere og sluttbrukere."
words:
  for: "til"

actions:
  main: "Gratis nedlasting av Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Lisensering"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Klar til å komme i gang?"
  description: "Prøv GroupDocs.Signature-funksjonene gratis eller be om en lisens"

release:
  title: "Versjon {0} utgitt"
  notes: "Se hva som er nytt"
  downloads: "Nedlastinger"

code:
  title: "Signer PDF-filer i Java"
  more: "Flere eksempler"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Velg PDF-dokument
    Signature signature = new Signature("sample.pdf");
    
    // Gi tekst
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Signer dokument og lagre til fil
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Oversikt"
  description: "API for å utføre dokumentsignering og relaterte operasjoner i Java-applikasjoner"
  features:
    # feature loop
    - title: "Forbedrede forretningsdokumenter med digitale signaturer i Java"
      content: "Rask og tilpassbar signering: GroupDocs.Signature for Java tilbyr et bredt spekter av digitale signaturalternativer for PDF-er, bilder og Office-dokumenter. Du kan bruke tekst, strekkoder, QR-koder, digitale sertifikater, bilder eller skjulte metadata. Dokumentbehandlingen er rask og effektiv."

    # feature loop
    - title: "Manipulere signerte dokumenter"
      content: "Avansert dokumentbehandling involverer kraftige operasjoner på signerte dokumenter ved hjelp av GroupDocs.Signature for Java. Du kan søke etter og validere signaturer som er lagt til forretningsdokumenter ved å bruke ulike nyttige kriterier. I tillegg kan du få tilgang til detaljert informasjon om dokumentet eller få forhåndsvisningsbilder av sidene."

    # feature loop
    - title: "En rekke utgangsvalg"
      content: "Robuste signeringsalternativer lar deg tilpasse utskriften for dokumenter signert med GroupDocs.Signature for Java. Du kan plassere enhver signatur nøyaktig på en dokumentside og konfigurere utseendet på forskjellige måter. Java API støtter lagring av signerte forretningsdokumenter i en rekke støttede formater og gir muligheter for å sikre dem med passord."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformuavhengighet"
  description: "GroupDocs.Signature for Java støtter følgende operativsystemer, rammeverk og pakkeadministratorer"
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
  title: "Støttede filformater"
  description: |
    GroupDocs.Signature for Java støtter operasjoner med følgende [filformater](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office-formater
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Bilder og andre formater
        * **Bærbar:** PDF
        * **Bilder:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Andre kontorformater:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Andre formater
        * **Web:** HTML, MHTML
        * **Arkiv:** ZIP, TAR, 7Z
        * **Sertifikater:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature-funksjoner"
  description: "Signering av PDF-er, Office-dokumenter og bilder med digitale signaturer"

  items:
    # feature loop
    - icon: "sign"
      title: "Legge til signaturer"
      content: "Signer et dokument ved å bruke ulike støttede signaturtyper ved å plassere en digital signatur nøyaktig hvor som helst på hvilken som helst side."

    # feature loop
    - icon: "custom"
      title: "Tilpasse resultater"
      content: "Tilpass signaturutseendet ved å justere farge, skrift, kantlinje, rotasjon og andre funksjoner for å oppnå ønsket resultat."

    # feature loop
    - icon: "password"
      title: "Sikring av dokumenter med passord"
      content: "For mange støttede dokumenttyper kan du beskytte det signerte dokumentet med et passord."

    # feature loop
    - icon: "protect"
      title: "Forhindre uautoriserte endringer"
      content: "Beskytt viktige forretningsdokumenter signert med et digitalt sertifikat mot uautoriserte endringer."

    # feature loop
    - icon: "convert"
      title: "Oppnå resultater i ønskede formater"
      content: "Få enkelt signerte resultatfiler i alle støttede formater. Du kan også konvertere MS Word-dokumenter til PDF uten problemer."

    # feature loop
    - icon: "preview"
      title: "Forhåndsvisning av dokument"
      content: "Lagre hvilken som helst side i et dokument som et bilde for fremtidig behandling."

    # feature loop
    - icon: "search"
      title: "Søker etter signaturer"
      content: "Det er mulig å få informasjon om tidligere tilførte signaturer i spesifikke dokumenter."

    # feature loop
    - icon: "validate"
      title: "Validering av dokumenter"
      content: "Validere riktigheten av signaturer på ethvert signert dokument."

    # feature loop
    - icon: "update"
      title: "Håndtering av signaturer"
      content: "Når en signatur er plassert på en dokumentside, kan den slettes, flyttes eller oppdateres etter behov."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodeprøver"
  description: "Noen bruker tilfeller av typiske GroupDocs.Signature for Java-operasjoner"
  items:
    # code sample loop
    - title: "Forbedre PDF-dokumentet med QR-kode"
      content: |
        Det kan være verdifullt å forbedre forretningsprosessene ved å legge til [QR-koder](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) til bestemte sider med PDF-dokumenter. Det er et eksempel på hvordan du legger til en QR-kode ved hjelp av GroupDocs.Signature for Java.
        {{< landing/code title="Forbedre PDF-dokumentet med QR-kode">}}
        ```java {style=abap}
        // Last inn dokumentet for å signere
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Lag QR-kodealternativer med forhåndsdefinert tekst
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurer QR-kodekodingstype og plassering på siden
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Signer dokumentet og lagre det som resultatfil
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Bruk digital signatur for å beskytte en DOCX"
      content: |
        Du kan [Beskytte et dokument](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) ved å bruke personlige eller bedriftssignaturer lagret som digitale sertifikater. Dokumenter sikret med sertifikat kan ikke endres uten å ugyldiggjøre signaturen.
        {{< landing/code title="Bruk digital signatur for å beskytte en DOCX">}}
        ```java {style=abap}   
        // Last inn dokumentet som skal signeres digitalt
        Signature signature = new Signature("file_to_sign.docx");
        
        // Angi alternativer for digital signering og oppgi banen til sertifikatfilen
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Angi sertifikatpassordet
        options.setPassword("1234567890");

        // Signer dokumentet og lagre det på ønsket bane
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
