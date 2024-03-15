---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: da
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
head_title: "Node.js Digital Signature API - GroupDocs.Signature"
head_description: "Integrer sikre e-signaturer i Node.js-apps med GroupDocs.Signature. Strømlin dokumentsigneringsarbejdsgange nemt og effektivt."

############################# Header ############################
title: "Underskriv dokumenter<br>med Node.js API"
description: "Signer digitale dokumenter og billeder på enhver platform ved hjælp af vores fleksible API'er og app-baserede løsninger til programmører og slutbrugere."
words:
  for: "til"

actions:
  main: "Download fra NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licensering"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Klar til at komme i gang?"
  description: "Prøv GroupDocs.Signature-funktioner gratis, eller anmod om en licens"

release:
  title: "Version {0} frigivet"
  notes: "Se, hvad der er nyt"
  downloads: "Downloads"

code:
  title: "Signering af PDF'er af Node.js"
  more: "Flere eksempler"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Vælg PDF-dokument
    let signature = new Signature("sample.pdf");
    
    // Giv tekst
    let options = new TextSignOptions("John Smith");
    
    // Indstil farve
    options.ForeColor = Color.Red;
    
    // Underskriv dokument og gem til fil
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signatur Oversigt"
  description: "Dokumenter, der signerer bibliotek, der er klar til at blive brugt i Node.js-applikationer"
  features:
    # feature loop
    - title: "Digitale signaturløsninger til forretningsdokumenter med Node.js"
      content: "GroupDocs.Signature for Node.js via Java tilbyder et omfattende sæt af digitale signaturmuligheder til PDF, Office-dokumenter og billeder. Tekst, stregkoder, billeder, digitale certifikater og metadata er tilgængelige. Strømlinet dokumentbehandling sikrer effektivitet."

    # feature loop
    - title: "Avanceret manipulation af underskrevne dokumenter"
      content: "GroupDocs.Signature giver dig mulighed for at behandle underskrevne dokumenter. Søg og valider signaturer ved hjælp af forskellige kriterier. Udtræk desuden detaljerede dokumentoplysninger eller generer forhåndsvisningsbilleder af sider."

    # feature loop
    - title: "Forskellige outputformater"
      content: "Vores løsning giver omfattende kontrol over outputformatet af signerede dokumenter. Placer signaturer præcist på enhver side, og tilpas deres udseende. Gem signerede dokumenter i adskillige understøttede formater og beskyt dem eventuelt med adgangskoder."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformens uafhængighed"
  description: "GroupDocs.Signature for Node.js via Java udfører dokumentbehandling med forskellige operativsystemer"
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
  title: "Understøttede filformater"
  description: |
    GroupDocs.Signature for Node.js via Java letter operationer for de [populære filformater](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
        ### Billeder og andre formater
        * **Transportabel:** PDF
        * **Billeder:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Andre kontorformater:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Andre formater
        * **Web:** HTML, MHTML
        * **Arkiv:** ZIP, TAR, 7Z
        * **Certifikater:** PFX

############################# Features ############################
features:
  enable: true
  title: "Funktioner af GroupDocs.Signature"
  description: "Signer PDF'er, Office-dokumenter og billeder med digitale signaturer"

  items:
    # feature loop
    - icon: "sign"
      title: "Forretningssignaturer"
      content: "Brug forskellige signaturtyper til at underskrive dokumenter. Placer digitale signaturer præcist på enhver sideplacering."

    # feature loop
    - icon: "custom"
      title: "Tilpasning af signaturudseende"
      content: "Skræddersy de visuelle aspekter af signaturer ved at justere farve, skrifttype, kanter, rotation og mere for at opnå dit ønskede resultat."

    # feature loop
    - icon: "password"
      title: "Adgangskodebeskyttede dokumenter"
      content: "For mange understøttede dokumentformater skal du beskytte signerede dokumenter med en adgangskode for øget sikkerhed."

    # feature loop
    - icon: "protect"
      title: "Forebyggelse af uautoriserede ændringer"
      content: "Beskyt vigtige forretningsdokumenter, der er signeret med digitale certifikater, mod uautoriserede ændringer."

    # feature loop
    - icon: "convert"
      title: "Ønskede outputformater"
      content: "Få ubesværet signerede dokumenter i ethvert understøttet format. Konverter MS Word-dokumenter til PDF-format med lethed."

    # feature loop
    - icon: "preview"
      title: "Forhåndsvisning af dokumenter"
      content: "Gem individuelle dokumentsider som billeder til fremtidige behov."

    # feature loop
    - icon: "search"
      title: "Signatursøgning"
      content: "Hent oplysninger om tidligere tilføjede signaturer i dine dokumenter."

    # feature loop
    - icon: "validate"
      title: "Dokumentvalidering"
      content: "Bekræft ægtheden af ​​underskrifter præsenteret i ethvert dokument."

    # feature loop
    - icon: "update"
      title: "Signaturhåndtering"
      content: "Slet, flyt eller rediger alle signaturer, der er placeret på en dokumentside."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kodeprøver"
  description: "Illustrative eksempler, der viser typiske GroupDocs.Signature for Node.js via Java-operationer"
  items:
    # code sample loop
    - title: "Marker PDF med QR-koder"
      content: |
        Inkorporering af [stregkoder](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) i specifikke PDF-dokumentsider kan strømline forretningsprocesser. Dette afsnit giver et eksempel på tilføjelse af en QR-kode ved hjælp af GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Sådan sætter du QR-kode til PDF.">}}
        ```javascript {style=abap}
        // Indlæs dokumentet for at underskrive
        let signature = new Signature("file_to_sign.pdf");
        
        // Opret QR-kodeindstillinger med foruddefineret tekst
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurer QR-kodekodningstype og position på siden
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Underskriv dokumentet og gem det som resultatfil
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Beskyttelse af en DOCX med en digital signatur"
      content: |
        [Beskyt dine dokumenter](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) med signaturer baseret på digitale certifikater. Digital signatur beskytter dine forretningsdokumenter mod indholdsændringer.
        {{< landing/code title="Sådan sikrer du dokumentets integritet.">}}
        ```javascript {style=abap}   
        // Indlæs dokumentet, der skal signeres digitalt
        let signature = new Signature("file_to_sign.docx");
        
        // Angiv muligheder for digital signering, og angiv stien til certifikatfilen
        let options = new DigitalSignOptions("certificate.pfx");

        // Indstil certifikatets adgangskode
        options.Password = "1234567890";

        // Underskriv dokumentet og gem det på den ønskede sti
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
