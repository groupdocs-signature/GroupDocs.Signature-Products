---
############################# Static ############################
layout: "landing"
date: 2023-09-13T10:36:50
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: af
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, Wolk API's en Aanlyn Dokument Handtekening Apps"
head_description: "Kry alles-in-een dokument e-handtekening oplossing vir .NET, Java en wolk-gebaseerde toepassings. Teken algemene dokumentformate aanlyn met 'n eenvoudige sleep-en-losfunksie"

############################# Header ############################
title: "Teken dokumente<br>via Java API"
description: "Teken digitale dokumente en beelde op enige platform deur ons buigsame API's en toepassingsgebaseerde oplossings vir programmeerders en eindgebruikers te gebruik."
words:
  for: "vir"

actions:
  main: "Gratis Maven-aflaai"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Lisensiëring"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Gereed om te begin?"
  description: "Probeer GroupDocs.Signature-kenmerke gratis of versoek 'n lisensie"

release:
  title: "Weergawe {0} vrygestel"
  notes: "Kyk wat nuut is"
  downloads: "Aflaaie"

code:
  title: "Teken PDF-lêers in Java"
  more: "Meer voorbeelde"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Kies PDF-dokument
    Signature signature = new Signature("sample.pdf");
    
    // Verskaf teks
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Teken dokument en stoor in lêer
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Oorsig"
  description: "API vir die uitvoer van dokumentondertekening en verwante bewerkings in Java-toepassings"
  features:
    # feature loop
    - title: "Verbeterde besigheidsdokumente met digitale handtekeninge in Java"
      content: "Vinnige en aanpasbare ondertekening: GroupDocs.Signature vir Java bied 'n wye reeks digitale handtekeningopsies vir PDF's, beelde en Office-dokumente. Jy kan teks, strepieskodes, QR-kodes, digitale sertifikate, prente of versteekte metadata gebruik. Die dokumentverwerking is vinnig en doeltreffend."

    # feature loop
    - title: "Manipuleer ondertekende dokumente"
      content: "Gevorderde dokumentverwerking behels kragtige bewerkings op ondertekende dokumente deur GroupDocs.Signature vir Java te gebruik. U kan handtekeninge wat by besigheidsdokumente gevoeg is soek en bekragtig met behulp van verskeie nuttige kriteria. Daarbenewens kan jy toegang tot gedetailleerde inligting oor die dokument kry of voorskoubeelde van sy bladsye kry."

    # feature loop
    - title: "Verskeidenheid uitsetkeuses"
      content: "Robuuste ondertekenopsies laat jou toe om die uitvoer vir dokumente wat met GroupDocs.Signature vir Java onderteken is, aan te pas. Jy kan enige handtekening presies op enige dokumentbladsy posisioneer en die voorkoms daarvan op verskeie maniere instel. Die Java API ondersteun die stoor van ondertekende besigheidsdokumente in talle ondersteunde formate en bied opsies om dit met wagwoorde te beveilig."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform onafhanklikheid"
  description: "GroupDocs.Signature vir Java ondersteun die volgende bedryfstelsels, raamwerke en pakketbestuurders"
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
  title: "Ondersteunde lêerformate"
  description: |
    GroupDocs.Signature vir Java ondersteun bedrywighede met die volgende [lêerformate](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "GroupDocs.Signature kenmerke"
  description: "Ondertekening van PDF's, Office Documents en beelde met digitale handtekeninge"

  items:
    # feature loop
    - icon: "merge"
      title: "Voeg handtekeninge by"
      content: "Teken 'n dokument deur verskeie ondersteunde handtekeningtipes te gebruik deur 'n digitale handtekening presies op enige posisie op enige bladsy te plaas."

    # feature loop
    - icon: "split"
      title: "Pasmaak van resultate"
      content: "Pas die kenmerkende voorkoms aan deur kleur, lettertipe, rand, rotasie en ander kenmerke aan te pas om die gewenste resultaat te bereik."

    # feature loop
    - icon: "move"
      title: "Beveilig dokumente met wagwoord"
      content: "Vir baie ondersteunde dokumenttipes kan jy die ondertekende dokument met 'n wagwoord beskerm."

    # feature loop
    - icon: "remove"
      title: "Voorkoming van ongemagtigde veranderinge"
      content: "Beskerm belangrike sakedokumente wat met 'n digitale sertifikaat onderteken is teen ongemagtigde wysigings."

    # feature loop
    - icon: "rotate"
      title: "Verkry resultate in gewenste formate"
      content: "Kry maklik getekende resultaatlêers in enige ondersteunde formaat. Jy kan ook moeiteloos MS Word-dokumente na PDF omskakel."

    # feature loop
    - icon: "swap"
      title: "Dokumentvoorskou"
      content: "Stoor enige bladsy van 'n dokument as 'n prent vir toekomstige verwerking."

    # feature loop
    - icon: "extract"
      title: "Soek na handtekeninge"
      content: "Dit is moontlik om inligting oor voorheen bygevoegde handtekeninge in spesifieke dokumente te kry."

    # feature loop
    - icon: "orientation"
      title: "Valideer dokumente"
      content: "Bekragtig die korrektheid van handtekeninge op enige ondertekende dokument."

    # feature loop
    - icon: "preview"
      title: "Die bestuur van handtekeninge"
      content: "Sodra 'n handtekening op 'n dokumentbladsy geplaas is, kan dit uitgevee, geskuif of opgedateer word soos nodig."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kode monsters"
  description: "Sommige gebruik gevalle van tipiese GroupDocs.Signature vir Java-bewerkings"
  items:
    # code sample loop
    - title: "Verbeter PDF-dokument met QR-kode"
      content: |
        Om besigheidsprosesse te verbeter deur [QR-kodes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) by spesifieke bladsye van PDF-dokumente by te voeg, kan waardevol wees. Daar is 'n voorbeeld van hoe om 'n QR-kode by te voeg deur GroupDocs.Signature vir Java te gebruik.
        {{< landing/code title="Verbeter PDF-dokument met QR-kode">}}
        ```java {style=abap}
        // Laai die dokument om te onderteken
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Skep QR-kode-opsies met voorafbepaalde teks
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Stel QR-kode enkodering tipe en posisie op die bladsy op
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Teken die dokument en stoor dit as die resultaatlêer
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Gebruik digitale handtekening om 'n DOCX te beskerm"
      content: |
        Jy kan [Beveilig 'n dokument](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) met persoonlike of korporatiewe handtekeninge wat as digitale sertifikate gestoor is. Dokumente wat met sertifikaat beveilig is, kan nie verander word sonder om die handtekening ongeldig te maak nie.
        {{< landing/code title="Gebruik digitale handtekening om 'n DOCX te beskerm">}}
        ```java {style=abap}   
        // Laai die dokument wat digitaal onderteken moet word
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Spesifiseer opsies vir digitale ondertekening en verskaf die pad na die sertifikaatlêer
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Stel die sertifikaatwagwoord in
        options.setPassword("1234567890");

        // Teken die dokument en stoor dit op die verlangde pad
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

############################# Reviews ############################
# reviews:
# enable: true
# title: "{reviews.title}"
# description: "{reviews.description}"

# items:
#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_1.content}"
#     author: "{reviews.review_1.author}"
#     company: "{reviews.review_1.company}"

#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_2.content}"
#     author: "{reviews.review_2.author}"
#     company: "{reviews.review_2.company}"
---
