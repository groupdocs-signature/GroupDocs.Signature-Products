---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:01
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
platform: "Net"
platform_tag: "net"

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
title: "Teken dokumente<br>via .NET API"
description: "Teken digitale dokumente en beelde op enige platform deur ons buigsame API's en toepassingsgebaseerde oplossings vir programmeerders en eindgebruikers te gebruik."
words:
  for: "vir"

actions:
  main: "Gratis NuGet-aflaai"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Lisensiëring"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Gereed om te begin?"
  description: "Probeer GroupDocs.Signature-kenmerke gratis of versoek 'n lisensie"

release:
  title: "Weergawe {0} vrygestel"
  notes: "Kyk wat nuut is"
  downloads: "Aflaaie"

code:
  title: "Teken PDF-lêers in C#"
  more: "Meer voorbeelde"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Kies PDF-dokument
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Verskaf teks
        var options = new TextSignOptions("John Smith")
        {
            // Stel kleur in
            ForeColor = Color.Red
        };
        // Teken dokument en stoor in lêer
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature Oorsig"
  description: "API vir die uitvoer van dokumentondertekening en verwante bewerkings in .NET-toepassings"
  features:
    # feature loop
    - title: "Voeg handtekeninge by besigheidsdokumente in C#"
      content: "Ondertekening van dokumente: Met GroupDocs.Signature vir .NET kan jy verskeie soorte handtekeninge, soos teks, beelde, strepieskodes en digitale sertifikate, by PDF- en Office-dokumente voeg. Hierdie API laat jou toe om jou dokumente met byna enige datatipe te onderteken, insluitend verborge metadata."

    # feature loop
    - title: "Verwerking van ondertekende dokumente"
      content: "Bykomende verwerking: Jy kan kragtige bewerkings op getekende dokumente uitvoer deur GroupDocs.Signature te gebruik. Dit sluit in om na bestaande handtekeninge binne besigheidsdokumente te soek en dit te verifieer met behulp van spesifieke kriteria. Boonop kan u dokumentinligting ophaal en bladsye voorskou deur hierdie .NET API."

    # feature loop
    - title: "Pasmaak van resultate"
      content: "GroupDocs.Signature vir .NET bied uitgebreide aanpassingsopsies. Jy kan handtekeninge op enige plek op 'n dokumentbladsy presies plaas en hul voorkoms aanpas deur 'n verskeidenheid instellings te gebruik. Verder ondersteun hierdie API die stoor van verwerkte dokumente in 'n wye reeks ondersteunde formate."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform onafhanklikheid"
  description: "GroupDocs.Signature vir .NET ondersteun die volgende bedryfstelsels, raamwerke en pakketbestuurders"
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
    GroupDocs.Signature vir .NET ondersteun bedrywighede met die volgende [lêerformate](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Teken PDF's, kantoordokumente en prente vinnig en akkuraat"

  items:
    # feature loop
    - icon: "sign"
      title: "Dokument ondertekening"
      content: "Voeg een of meer ondersteunde tipes handtekeninge akkuraat by enige gespesifiseerde posisie op besigheidsdokumente."

    # feature loop
    - icon: "custom"
      title: "Pas handtekeninge aan"
      content: "Gebruik kenmerke soos kleur, lettertipe, rand, rotasie, ens., om die voorkoms van handtekeninge op te stel."

    # feature loop
    - icon: "password"
      title: "Dokument wagwoordbeskerming"
      content: "Beveilig sekere dokumenttipes deur 'n wagwoord in te stel na ondertekening."

    # feature loop
    - icon: "protect"
      title: "Beskerming teen veranderinge"
      content: "Voorkom veranderinge aan belangrike sakedokumente nadat 'n handtekening met 'n digitale sertifikaat bygevoeg is."

    # feature loop
    - icon: "convert"
      title: "Skakel ondertekende lêers om na ander formate"
      content: "Skakel ondertekende lêers om na gewenste formate, soos om 'n Word-dokument as 'n PDF te stoor."

    # feature loop
    - icon: "preview"
      title: "Onttrek bladsyvoorskoue"
      content: "Onttrek bladsye uit getekende dokumente as individuele beelde vir toekomstige verwerking."

    # feature loop
    - icon: "search"
      title: "Handtekeningsoektog in dokumente"
      content: "Kry inligting oor voorheen bygevoeg handtekeninge in spesifieke dokumente."

    # feature loop
    - icon: "validate"
      title: "Valideer ondertekende dokumente"
      content: "Verifieer die behoorlike ondertekening van dokumente deur valideringskenmerke te gebruik."

    # feature loop
    - icon: "update"
      title: "Dateer handtekeninge op of vee dit uit"
      content: "Herposisioneer spesifieke handtekeninge maklik op 'n bladsy, wysig hul teks, of vee dit uit sonder enige probleme."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kode monsters"
  description: "Sommige gebruik gevalle van tipiese GroupDocs.Signature vir .NET-bedrywighede"
  items:
    # code sample loop
    - title: "Voeg QR-kode by PDF"
      content: |
        Die byvoeging van [QR-kodes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) by spesifieke bladsye van PDF-dokumente kan besigheidsprosesse verbeter. Hieronder is 'n voorbeeld van hoe om 'n QR-kode by te voeg deur GroupDocs.Signature te gebruik.
        {{< landing/code title="Hoe om QR-kode in PDF te plaas.">}}
        ```csharp {style=abap}
        // Laai die dokument om te onderteken
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Skep QR-kode-opsies met voorafbepaalde teks
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Stel QR-kode enkodering tipe en posisie op die bladsy op
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Teken die dokument en stoor dit as die resultaatlêer
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Beskerm 'n DOCX-dokument met 'n digitale sertifikaat"
      content: |
        Jy kan [Beskerm 'n dokument](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) met persoonlike of korporatiewe handtekeninge wat as digitale sertifikate gestoor is. Sulke beskermde dokumente kan nie gewysig word sonder om die handtekening ongeldig te maak nie.
        {{< landing/code title="Hier is hoe om dokumentintegriteit te verseker.">}}
        ```csharp {style=abap}   
        // Laai die dokument wat digitaal onderteken moet word
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Spesifiseer opsies vir digitale ondertekening en verskaf die pad na die sertifikaatlêer
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Stel die sertifikaatwagwoord in
                Password = "1234567890"
            };
            // Teken die dokument en stoor dit op die verlangde pad
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
