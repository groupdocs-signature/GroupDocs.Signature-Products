---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: af
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
head_title: ".NET, Java, Wolk API's en Aanlyn Dokument Handtekening Apps"
head_description: "Kry alles-in-een dokument e-handtekening oplossing vir .NET, Java en wolk-gebaseerde toepassings. Teken algemene dokumentformate aanlyn met 'n eenvoudige sleep-en-losfunksie"

############################# Header ############################
title: "Teken dokumente<br>met Node.js API"
description: "Teken digitale dokumente en beelde op enige platform deur ons buigsame API's en toepassingsgebaseerde oplossings vir programmeerders en eindgebruikers te gebruik."
words:
  for: "vir"

actions:
  main: "Laai af van NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Lisensiëring"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Gereed om te begin?"
  description: "Probeer GroupDocs.Signature-kenmerke gratis of versoek 'n lisensie"

release:
  title: "Weergawe {0} vrygestel"
  notes: "Kyk wat nuut is"
  downloads: "Aflaaie"

code:
  title: "Teken van PDF's deur Node.js"
  more: "Meer voorbeelde"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Kies PDF-dokument
    let signature = new Signature("sample.pdf");
    
    // Verskaf teks
    let options = new TextSignOptions("John Smith");
    
    // Stel kleur in
    options.ForeColor = Color.Red;
    
    // Teken dokument en stoor in lêer
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Oorsig"
  description: "Dokumente wat biblioteek onderteken wat gereed is om in Node.js-toepassings gebruik te word"
  features:
    # feature loop
    - title: "Oplossing vir digitale handtekeninge vir besigheidsdokumente met Node.js"
      content: "GroupDocs.Signature for Node.js via Java bied 'n omvattende stel digitale handtekeningopsies vir PDF, Office-dokumente en prente. Teks, strepieskodes, beelde, digitale sertifikate en metadata is beskikbaar. Gestroomlynde dokumentverwerking verseker doeltreffendheid."

    # feature loop
    - title: "Gevorderde manipulasie van getekende dokumente"
      content: "GroupDocs.Signature bemagtig jou om ondertekende dokumente te verwerk. Soek en valideer handtekeninge deur verskeie kriteria te gebruik. Onttrek ook gedetailleerde dokumentinligting of genereer voorskoubeelde van bladsye."

    # feature loop
    - title: "Diverse uitvoerformate"
      content: "Ons oplossing bied uitgebreide beheer oor die uitvoerformaat van ondertekende dokumente. Plaas handtekeninge presies op enige bladsy en pas hul voorkoms aan. Stoor ondertekende dokumente in talle ondersteunde formate en beveilig dit opsioneel met wagwoorde."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform onafhanklikheid"
  description: "GroupDocs.Signature for Node.js via Java voer dokumentverwerking met verskeie bedryfstelsels uit"
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
  title: "Ondersteunde lêerformate"
  description: |
    GroupDocs.Signature for Node.js via Java fasiliteer bewerkings vir die [gewilde lêerformate](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office-formate
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Prente en ander formate
        * **Draagbaar:** PDF
        * **Beelde:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Ander kantoorformate:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Ander formate
        * **Web:** HTML, MHTML
        * **Argiewe:** ZIP, TAR, 7Z
        * **Sertifikate:** PFX

############################# Features ############################
features:
  enable: true
  title: "Kenmerke van GroupDocs.Signature"
  description: "Teken PDF's, Office-dokumente en beelde met digitale handtekeninge"

  items:
    # feature loop
    - icon: "sign"
      title: "Besigheidshandtekeninge"
      content: "Gebruik verskeie handtekeningtipes om dokumente te onderteken. Plaas digitale handtekeninge presies op enige bladsy-ligging."

    # feature loop
    - icon: "custom"
      title: "Pas handtekeningvoorkoms aan"
      content: "Pas die visuele aspekte van handtekeninge aan deur kleur, lettertipe, grense, rotasie en meer aan te pas om die gewenste uitkoms te bereik."

    # feature loop
    - icon: "password"
      title: "Wagwoord-beskermde dokumente"
      content: "Vir baie ondersteunde dokumentformate, beskerm ondertekende dokumente met 'n wagwoord vir ekstra sekuriteit."

    # feature loop
    - icon: "protect"
      title: "Voorkoming van ongemagtigde wysigings"
      content: "Beskerm belangrike sakedokumente wat met digitale sertifikate onderteken is teen ongemagtigde veranderings."

    # feature loop
    - icon: "convert"
      title: "Gewenste uitvoerformate"
      content: "Kry moeiteloos ondertekende dokumente in enige ondersteunde formaat. Skakel MS Word-dokumente met gemak na PDF-formaat om."

    # feature loop
    - icon: "preview"
      title: "Dokumentevoorskou"
      content: "Stoor individuele dokumentbladsye as beelde vir toekomstige behoeftes."

    # feature loop
    - icon: "search"
      title: "Soek na handtekening"
      content: "Kry inligting oor voorheen bygevoeg handtekeninge binne jou dokumente."

    # feature loop
    - icon: "validate"
      title: "Dokument validering"
      content: "Verifieer die egtheid van handtekeninge wat in enige dokument aangebied word."

    # feature loop
    - icon: "update"
      title: "Handtekeningbestuur"
      content: "Vee uit, hervestig of wysig enige handtekeninge wat op enige dokumentbladsy geplaas is."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kode monsters"
  description: "Illustratiewe voorbeelde wat tipiese GroupDocs.Signature for Node.js via Java-bewerkings uitstal"
  items:
    # code sample loop
    - title: "Merk PDF met QR-kodes"
      content: |
        Die inkorporering van [strepieskodes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) in spesifieke PDF-dokumentbladsye kan besigheidsprosesse stroomlyn. Hierdie afdeling verskaf 'n voorbeeld van die byvoeging van 'n QR-kode deur GroupDocs.Signature for Node.js via Java te gebruik.
        {{< landing/code title="Hoe om QR-kode in PDF te plaas.">}}
        ```javascript {style=abap}
        // Laai die dokument om te onderteken
        let signature = new Signature("file_to_sign.pdf");
        
        // Skep QR-kode-opsies met voorafbepaalde teks
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Stel QR-kode enkodering tipe en posisie op die bladsy op
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Teken die dokument en stoor dit as die resultaatlêer
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Beskerm 'n DOCX met 'n digitale handtekening"
      content: |
        [Beskerm jou dokumente](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) deur handtekeninge gebaseer op digitale sertifikate. Digitale handtekening beskerm u besigheidsdokumente teen inhoudsverandering.
        {{< landing/code title="Hier is hoe om dokumentintegriteit te verseker.">}}
        ```javascript {style=abap}   
        // Laai die dokument wat digitaal onderteken moet word
        let signature = new Signature("file_to_sign.docx");
        
        // Spesifiseer opsies vir digitale ondertekening en verskaf die pad na die sertifikaatlêer
        let options = new DigitalSignOptions("certificate.pfx");

        // Stel die sertifikaatwagwoord in
        options.Password = "1234567890";

        // Teken die dokument en stoor dit op die verlangde pad
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
