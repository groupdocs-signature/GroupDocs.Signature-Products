---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: no
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
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

############################# Head ############################
head_title: ".NET, Java, Cloud APIer og nettbaserte dokumentsignaturapper"
head_description: "Få alt-i-ett dokument-e-signaturløsning for .NET, Java og skybaserte applikasjoner. Signer vanlige dokumentformater på nettet ved hjelp av enkel dra og slipp-funksjon"

############################# Header ############################
title: "Signer dokumenter<br>med Node.js API"
description: "Signer digitale dokumenter og bilder på hvilken som helst plattform ved å bruke våre fleksible APIer og appbaserte løsninger for programmerere og sluttbrukere."
words:
  for: "til"

actions:
  main: "Last ned fra NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Lisensering"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Klar til å komme i gang?"
  description: "Prøv GroupDocs.Signature-funksjonene gratis eller be om en lisens"

release:
  title: "Versjon {0} utgitt"
  notes: "Se hva som er nytt"
  downloads: "Nedlastinger"

code:
  title: "Signering av PDF-er av Node.js"
  more: "Flere eksempler"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // Velg PDF-dokument
    let signature = new Signature("sample.pdf");
    
    // Gi tekst
    let options = new TextSignOptions("John Smith");
    
    // Sett farge
    options.ForeColor = Color.Red;
    
    // Signer dokument og lagre til fil
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Oversikt"
  description: "Dokumenter signeringsbibliotek som er klart til bruk i Node.js-applikasjoner"
  features:
    # feature loop
    - title: "Digital signaturløsning for forretningsdokumenter med Node.js"
      content: "GroupDocs.Signature for Node.js via Java tilbyr et omfattende sett med digitale signaturalternativer for PDF, Office-dokumenter og bilder. Tekst, strekkoder, bilder, digitale sertifikater og metadata er tilgjengelig. Strømlinjeformet dokumentbehandling sikrer effektivitet."

    # feature loop
    - title: "Avansert manipulering av signerte dokumenter"
      content: "GroupDocs.Signature gir deg mulighet til å behandle signerte dokumenter. Søk og valider signaturer ved å bruke ulike kriterier. Trekk i tillegg ut detaljert dokumentinformasjon eller generer forhåndsvisningsbilder av sider."

    # feature loop
    - title: "Ulike utdataformater"
      content: "Vår løsning gir omfattende kontroll over utdataformatet til signerte dokumenter. Plasser signaturer nøyaktig på hvilken som helst side og tilpass utseendet deres. Lagre signerte dokumenter i en rekke støttede formater og eventuelt sikre dem med passord."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformuavhengighet"
  description: "GroupDocs.Signature for Node.js via Java utfører dokumentbehandling med ulike operativsystemer"
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
  title: "Støttede filformater"
  description: |
    GroupDocs.Signature for Node.js via Java forenkler operasjoner for [populære filformater](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Funksjoner til GroupDocs.Signature"
  description: "Signer PDF-er, Office-dokumenter og bilder med digitale signaturer"

  items:
    # feature loop
    - icon: "sign"
      title: "Forretningssignaturer"
      content: "Bruk ulike signaturtyper for å signere dokumenter. Plasser digitale signaturer nøyaktig på hvilken som helst sideplassering."

    # feature loop
    - icon: "custom"
      title: "Tilpasse signaturutseende"
      content: "Skreddersy de visuelle aspektene ved signaturer ved å justere farge, skrift, kantlinjer, rotasjon og mer for å oppnå ønsket resultat."

    # feature loop
    - icon: "password"
      title: "Passordbeskyttede dokumenter"
      content: "For mange støttede dokumentformater, beskytt signerte dokumenter med et passord for ekstra sikkerhet."

    # feature loop
    - icon: "protect"
      title: "Forhindre uautoriserte endringer"
      content: "Beskytt viktige forretningsdokumenter signert med digitale sertifikater mot uautoriserte endringer."

    # feature loop
    - icon: "convert"
      title: "Ønskede utdataformater"
      content: "Få signerte dokumenter i alle støttede formater uten problemer. Konverter MS Word-dokumenter til PDF-format med letthet."

    # feature loop
    - icon: "preview"
      title: "Forhåndsvisning av dokumenter"
      content: "Lagre individuelle dokumentsider som bilder for fremtidige behov."

    # feature loop
    - icon: "search"
      title: "Signatursøk"
      content: "Hent informasjon om tidligere lagt til signaturer i dokumentene dine."

    # feature loop
    - icon: "validate"
      title: "Dokumentvalidering"
      content: "Bekreft ektheten til signaturer som presenteres i ethvert dokument."

    # feature loop
    - icon: "update"
      title: "Signaturbehandling"
      content: "Slett, flytt eller modifiser eventuelle signaturer som er plassert på en dokumentside."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodeprøver"
  description: "Illustrerende eksempler som viser typiske GroupDocs.Signature for Node.js via Java-operasjoner"
  items:
    # code sample loop
    - title: "Merk PDF med QR-koder"
      content: |
        Å inkludere [strekkoder](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) i spesifikke PDF-dokumentsider kan strømlinjeforme forretningsprosesser. Denne delen gir et eksempel på å legge til en QR-kode ved å bruke GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Hvordan sette QR-kode til PDF.">}}
        ```javascript {style=abap}
        // Last inn dokumentet for å signere
        let signature = new Signature("file_to_sign.pdf");
        
        // Lag QR-kodealternativer med forhåndsdefinert tekst
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurer QR-kodekodingstype og plassering på siden
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Signer dokumentet og lagre det som resultatfil
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Beskytte en DOCX med en digital signatur"
      content: |
        [Beskytt dokumentene dine](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) med signaturer basert på digitale sertifikater. Digital signatur beskytter forretningsdokumentene dine mot endring av innhold.
        {{< landing/code title="Slik sikrer du dokumentets integritet.">}}
        ```javascript {style=abap}   
        // Last inn dokumentet som skal signeres digitalt
        let signature = new Signature("file_to_sign.pdf");
        
        // Angi alternativer for digital signering og oppgi banen til sertifikatfilen
        let options = new DigitalSignOptions("certificate.pfx");

        // Angi sertifikatpassordet
        options.Password = "1234567890";

        // Signer dokumentet og lagre det på ønsket bane
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
