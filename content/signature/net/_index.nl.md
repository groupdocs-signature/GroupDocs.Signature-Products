---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:50
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: nl
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
head_title: "C# .NET Digitale handtekeningen API - GroupDocs.Handtekening"
head_description: "Integreer de verwerking van digitale handtekeningen in uw .NET-apps met behulp van GroupDocs.Signature. Beveilig uw bestanden snel en efficiënt met handtekeningen."

############################# Header ############################
title: "Onderteken documenten<br>via .NET-API"
description: "Onderteken digitale documenten en afbeeldingen op elk platform met behulp van onze flexibele API's en app-gebaseerde oplossingen voor programmeurs en eindgebruikers."
words:
  for: "voor"

actions:
  main: "Gratis NuGet-download"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licentie"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "klaar om te beginnen?"
  description: "Probeer de functies van GroupDocs.Signature gratis of vraag een licentie aan"

release:
  title: "Versie {0} vrijgegeven"
  notes: "Zie wat nieuw is"
  downloads: "Downloads"

code:
  title: "Onderteken PDF-bestanden in C#"
  more: "Meer voorbeelden"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Selecteer PDF-document
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Geef tekst op
        var options = new TextSignOptions("John Smith")
        {
            // Kleur instellen
            ForeColor = Color.Red
        };
        // Onderteken het document en sla het op in een bestand
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature-overzicht"
  description: "API voor het uitvoeren van documentondertekening en gerelateerde bewerkingen in .NET-applicaties"
  features:
    # feature loop
    - title: "Handtekeningen toevoegen aan zakelijke documenten in C#"
      content: "Ondertekening van documenten: Met GroupDocs.Signature voor .NET kunt u verschillende soorten handtekeningen, zoals tekst, afbeeldingen, streepjescodes en digitale certificaten, toevoegen aan PDF- en Office-documenten. Met deze API kunt u uw documenten ondertekenen met vrijwel elk gegevenstype, inclusief verborgen metadata."

    # feature loop
    - title: "Verwerken van ondertekende documenten"
      content: "Extra verwerking: U kunt krachtige bewerkingen uitvoeren op ondertekende documenten met behulp van GroupDocs.Signature. Dit omvat het zoeken naar bestaande handtekeningen in bedrijfsdocumenten en het verifiëren ervan aan de hand van specifieke criteria. Bovendien kunt u via deze .NET API documentinformatie ophalen en voorbeeldpagina's bekijken."

    # feature loop
    - title: "Resultaten aanpassen"
      content: "GroupDocs.Signature voor .NET biedt uitgebreide aanpassingsmogelijkheden. U kunt handtekeningen overal op een documentpagina nauwkeurig plaatsen en hun uiterlijk aanpassen met behulp van diverse instellingen. Bovendien ondersteunt deze API het opslaan van verwerkte documenten in een groot aantal ondersteunde formaten."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformonafhankelijkheid"
  description: "GroupDocs.Signature voor .NET ondersteunt de volgende besturingssystemen, frameworks en pakketbeheerders"
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
  title: "Ondersteunde bestandsformaten"
  description: |
    GroupDocs.Signature voor .NET ondersteunt bewerkingen met de volgende [bestandsindelingen](https://docs.groupdocs.com/signature/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office-formaten
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Afbeeldingen en andere formaten
        * **Draagbaar:** PDF
        * **Afbeeldingen:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Andere kantoorformaten:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Andere formaten
        * **Web:** HTML, MHTML
        * **Archief:** ZIP, TAR, 7Z
        * **Certificaten:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature-functies"
  description: "Onderteken PDF's, Office-documenten en afbeeldingen snel en nauwkeurig"

  items:
    # feature loop
    - icon: "sign"
      title: "Ondertekening van documenten"
      content: "Voeg nauwkeurig een of meerdere ondersteunde typen handtekeningen toe op elke opgegeven positie in zakelijke documenten."

    # feature loop
    - icon: "custom"
      title: "Pas handtekeningen aan"
      content: "Gebruik functies zoals kleur, lettertype, rand, rotatie, enz. om de weergave van handtekeningen te configureren."

    # feature loop
    - icon: "password"
      title: "Wachtwoordbeveiliging voor documenten"
      content: "Beveilig bepaalde documenttypen door na ondertekening een wachtwoord in te stellen."

    # feature loop
    - icon: "protect"
      title: "Bescherming tegen veranderingen"
      content: "Voorkom wijzigingen in belangrijke zakelijke documenten na het plaatsen van een handtekening met een digitaal certificaat."

    # feature loop
    - icon: "convert"
      title: "Converteer ondertekende bestanden naar andere formaten"
      content: "Converteer ondertekende bestanden naar gewenste formaten, zoals het opslaan van een Word-document als PDF."

    # feature loop
    - icon: "preview"
      title: "Paginavoorbeelden extraheren"
      content: "Extraheer pagina's uit ondertekende documenten als individuele afbeeldingen voor toekomstige verwerking."

    # feature loop
    - icon: "search"
      title: "Handtekeningen zoeken in documenten"
      content: "Haal informatie op over eerder toegevoegde handtekeningen in specifieke documenten."

    # feature loop
    - icon: "validate"
      title: "Valideer ondertekende documenten"
      content: "Controleer de juiste ondertekening van documenten met behulp van validatiefuncties."

    # feature loop
    - icon: "update"
      title: "Handtekeningen bijwerken of verwijderen"
      content: "Verplaats specifieke handtekeningen eenvoudig op een pagina, wijzig de tekst ervan of verwijder ze zonder problemen."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codevoorbeelden"
  description: "Enkele gebruiksscenario's van typische GroupDocs.Signature voor .NET-bewerkingen"
  items:
    # code sample loop
    - title: "Voeg QR-code toe aan PDF"
      content: |
        Het toevoegen van [QR-codes](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) aan specifieke pagina's van PDF-documenten kan bedrijfsprocessen verbeteren. Hieronder ziet u een voorbeeld van hoe u een QR-code kunt toevoegen met GroupDocs.Signature.
        {{< landing/code title="Hoe QR-code naar PDF te zetten.">}}
        ```csharp {style=abap}
        // Laad het document dat u wilt ondertekenen
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Maak QR-code-opties met vooraf gedefinieerde tekst
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Configureer het coderingstype en de positie van de QR-code op de pagina
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Onderteken het document en sla het op als resultaatbestand
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Een DOCX-document beveiligen met een digitaal certificaat"
      content: |
        U kunt [een document beveiligen](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) met behulp van persoonlijke of zakelijke handtekeningen die zijn opgeslagen als digitale certificaten. Dergelijke beschermde documenten kunnen niet worden gewijzigd zonder de handtekening ongeldig te maken.
        {{< landing/code title="Hier leest u hoe u de documentintegriteit kunt garanderen.">}}
        ```csharp {style=abap}   
        // Laad het document dat digitaal moet worden ondertekend
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Geef opties voor digitale ondertekening op en geef het pad naar het certificaatbestand op
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Stel het certificaatwachtwoord in
                Password = "1234567890"
            };
            // Onderteken het document en sla het op in het gewenste pad
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
