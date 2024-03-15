---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: sl
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
head_title: "API za digitalni podpis Node.js – GroupDocs.Signature"
head_description: "Integrirajte varne e-podpise v aplikacije Node.js s GroupDocs.Signature. Preprosto in učinkovito poenostavite delovne tokove podpisovanja dokumentov."

############################# Header ############################
title: "Podpišite dokumente<br>z API-jem Node.js"
description: "Podpisujte digitalne dokumente in slike na kateri koli platformi z uporabo naših prilagodljivih API-jev in rešitev, ki temeljijo na aplikacijah, za programerje in končne uporabnike."
words:
  for: "za"

actions:
  main: "Prenesite iz NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licenciranje"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Ste pripravljeni začeti?"
  description: "Preizkusite funkcije GroupDocs.Signature brezplačno ali zahtevajte licenco"

release:
  title: "Izdana različica {0}"
  notes: "Oglejte si, kaj je novega"
  downloads: "Prenosi"

code:
  title: "Podpisovanje PDF-jev z Node.js"
  more: "Več primerov"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Izberite dokument PDF
    let signature = new Signature("sample.pdf");
    
    // Navedite besedilo
    let options = new TextSignOptions("John Smith");
    
    // Nastavite barvo
    options.ForeColor = Color.Red;
    
    // Podpišite dokument in ga shranite v datoteko
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Pregled"
  description: "Knjižnica za podpisovanje dokumentov, pripravljena za uporabo v aplikacijah Node.js"
  features:
    # feature loop
    - title: "Rešitev za digitalne podpise za poslovne dokumente z Node.js"
      content: "GroupDocs.Signature for Node.js via Java ponuja obsežen nabor možnosti digitalnega podpisa za dokumente PDF, Office in slike. Na voljo so besedilo, črtne kode, slike, digitalna potrdila in metapodatki. Poenostavljena obdelava dokumentov zagotavlja učinkovitost."

    # feature loop
    - title: "Napredno manipuliranje s podpisanimi dokumenti"
      content: "GroupDocs.Signature vam omogoča obdelavo podpisanih dokumentov. Iskanje in preverjanje podpisov z različnimi kriteriji. Poleg tega izvlecite podrobne informacije o dokumentu ali ustvarite slike za predogled strani."

    # feature loop
    - title: "Različni izhodni formati"
      content: "Naša rešitev zagotavlja obsežen nadzor nad izhodno obliko podpisanih dokumentov. Natančno postavite podpise na katero koli stran in prilagodite njihov videz. Podpisane dokumente shranite v številnih podprtih formatih in jih po želji zaščitite z gesli."

############################# Platforms ############################
platforms:
  enable: true
  title: "Neodvisnost platforme"
  description: "GroupDocs.Signature for Node.js via Java izvaja obdelavo dokumentov z različnimi operacijskimi sistemi"
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
  title: "Podprti formati datotek"
  description: |
    GroupDocs.Signature for Node.js via Java olajša operacije za [priljubljene formate datotek](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formati
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Slike in drugi formati
        * **Prenosni:** PDF
        * **Slike:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Drugi pisarniški formati:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Drugi formati
        * **Splet:** HTML, MHTML
        * **Arhivi:** ZIP, TAR, 7Z
        * **Certifikati:** PFX

############################# Features ############################
features:
  enable: true
  title: "Značilnosti GroupDocs.Signature"
  description: "Z digitalnimi podpisi podpišite dokumente PDF, Officeove dokumente in slike"

  items:
    # feature loop
    - icon: "sign"
      title: "Poslovni podpisi"
      content: "Za podpisovanje dokumentov uporabite različne vrste podpisov. Natančno postavite digitalne podpise na katero koli stran."

    # feature loop
    - icon: "custom"
      title: "Prilagajanje videza podpisa"
      content: "Prilagodite vizualne vidike podpisov tako, da prilagodite barvo, pisavo, obrobe, vrtenje in drugo, da dosežete želeni rezultat."

    # feature loop
    - icon: "password"
      title: "Dokumenti, zaščiteni z geslom"
      content: "Za več podprtih formatov dokumentov zaščitite podpisane dokumente z geslom za dodatno varnost."

    # feature loop
    - icon: "protect"
      title: "Preprečevanje nepooblaščenih sprememb"
      content: "Zaščitite ključne poslovne dokumente, podpisane z digitalnimi potrdili, pred nepooblaščenimi spremembami."

    # feature loop
    - icon: "convert"
      title: "Želeni izhodni formati"
      content: "Z lahkoto pridobite podpisane dokumente v katerem koli podprtem formatu. Pretvorite dokumente MS Word v format PDF z lahkoto."

    # feature loop
    - icon: "preview"
      title: "Predogled dokumentov"
      content: "Shranite posamezne strani dokumenta kot slike za prihodnje potrebe."

    # feature loop
    - icon: "search"
      title: "Iskanje podpisa"
      content: "Pridobite informacije o predhodno dodanih podpisih v vaših dokumentih."

    # feature loop
    - icon: "validate"
      title: "Validacija dokumenta"
      content: "Preverite pristnost podpisov v katerem koli dokumentu."

    # feature loop
    - icon: "update"
      title: "Upravljanje podpisov"
      content: "Izbrišite, premaknite ali spremenite vse podpise na kateri koli strani dokumenta."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Vzorci kod"
  description: "Ilustrativni primeri, ki prikazujejo tipične operacije GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Označite PDF s kodami QR"
      content: |
        Vključitev [črtnih kod](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) v določene strani dokumenta PDF lahko poenostavi poslovne procese. V tem razdelku je primer dodajanja kode QR z uporabo GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Kako vstaviti QR kodo v PDF.">}}
        ```javascript {style=abap}
        // Naložite dokument za podpis
        let signature = new Signature("file_to_sign.pdf");
        
        // Ustvarite možnosti kode QR z vnaprej določenim besedilom
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Konfigurirajte vrsto in položaj kodiranja kode QR na strani
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Podpišite dokument in ga shranite kot datoteko z rezultati
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Zaščita DOCX z digitalnim podpisom"
      content: |
        [Zaščitite svoje dokumente](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) s podpisi na podlagi digitalnih potrdil. Digitalni podpis zaščiti vaše poslovne dokumente pred spreminjanjem vsebine.
        {{< landing/code title="Tukaj je opisano, kako zagotoviti celovitost dokumenta.">}}
        ```javascript {style=abap}   
        // Naložite dokument, ki ga želite digitalno podpisati
        let signature = new Signature("file_to_sign.docx");
        
        // Določite možnosti digitalnega podpisovanja in navedite pot do datoteke potrdila
        let options = new DigitalSignOptions("certificate.pfx");

        // Nastavite geslo za potrdilo
        options.Password = "1234567890";

        // Podpišite dokument in ga shranite na želeno pot
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
