---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: nl
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
head_title: ".NET, Java, Cloud API's en online apps voor documenthandtekening"
head_description: "Ontvang een alles-in-één oplossing voor e-handtekening van documenten voor .NET, Java en cloudgebaseerde applicaties. Onderteken veelgebruikte documentformaten online met behulp van een eenvoudige functie voor slepen en neerzetten"

############################# Header ############################
title: "Onderteken documenten<br>met Node.js-API"
description: "Onderteken digitale documenten en afbeeldingen op elk platform met behulp van onze flexibele API's en app-gebaseerde oplossingen voor programmeurs en eindgebruikers."
words:
  for: "voor"

actions:
  main: "Downloaden van NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licentie"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "klaar om te beginnen?"
  description: "Probeer de functies van GroupDocs.Signature gratis of vraag een licentie aan"

release:
  title: "Versie {0} vrijgegeven"
  notes: "Zie wat nieuw is"
  downloads: "Downloads"

code:
  title: "PDF's ondertekenen door Node.js"
  more: "Meer voorbeelden"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Selecteer PDF-document
    let signature = new Signature("sample.pdf");
    
    // Geef tekst op
    let options = new TextSignOptions("John Smith");
    
    // Kleur instellen
    options.ForeColor = Color.Red;
    
    // Onderteken het document en sla het op in een bestand
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature-overzicht"
  description: "Bibliotheek voor het ondertekenen van documenten die klaar is om te worden gebruikt in Node.js-toepassingen"
  features:
    # feature loop
    - title: "Oplossing voor digitale handtekeningen voor zakelijke documenten met Node.js"
      content: "GroupDocs.Signature for Node.js via Java biedt een uitgebreide reeks digitale handtekeningopties voor PDF-, Office-documenten en afbeeldingen. Tekst, barcodes, afbeeldingen, digitale certificaten en metadata zijn beschikbaar. Gestroomlijnde documentverwerking zorgt voor efficiëntie."

    # feature loop
    - title: "Geavanceerde manipulatie van ondertekende documenten"
      content: "Met GroupDocs.Signature kunt u ondertekende documenten verwerken. Zoek en valideer handtekeningen met behulp van verschillende criteria. Extraheer bovendien gedetailleerde documentinformatie of genereer voorbeeldafbeeldingen van pagina's."

    # feature loop
    - title: "Diverse uitvoerformaten"
      content: "Onze oplossing biedt uitgebreide controle over het uitvoerformaat van ondertekende documenten. Plaats handtekeningen nauwkeurig op elke pagina en pas hun uiterlijk aan. Bewaar ondertekende documenten in talloze ondersteunde formaten en beveilig ze optioneel met wachtwoorden."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformonafhankelijkheid"
  description: "GroupDocs.Signature for Node.js via Java voert documentverwerking uit met verschillende besturingssystemen"
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
    GroupDocs.Signature for Node.js via Java vergemakkelijkt bewerkingen voor de [populaire bestandsindelingen](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Kenmerken van GroupDocs.Signature"
  description: "Onderteken PDF's, Office-documenten en afbeeldingen met digitale handtekeningen"

  items:
    # feature loop
    - icon: "sign"
      title: "Zakelijke handtekeningen"
      content: "Gebruik verschillende handtekeningtypen om documenten te ondertekenen. Plaats digitale handtekeningen precies op elke paginalocatie."

    # feature loop
    - icon: "custom"
      title: "Het kenmerkende uiterlijk aanpassen"
      content: "Pas de visuele aspecten van handtekeningen aan door de kleur, het lettertype, de randen, de rotatie en meer aan te passen om het gewenste resultaat te bereiken."

    # feature loop
    - icon: "password"
      title: "Met wachtwoord beveiligde documenten"
      content: "Voor veel ondersteunde documentformaten kunt u ondertekende documenten beveiligen met een wachtwoord voor extra beveiliging."

    # feature loop
    - icon: "protect"
      title: "Ongeautoriseerde wijzigingen voorkomen"
      content: "Bescherm cruciale zakelijke documenten ondertekend met digitale certificaten tegen ongeoorloofde wijzigingen."

    # feature loop
    - icon: "convert"
      title: "Gewenste uitvoerformaten"
      content: "Ontvang moeiteloos ondertekende documenten in elk ondersteund formaat. Converteer MS Word-documenten eenvoudig naar PDF-formaat."

    # feature loop
    - icon: "preview"
      title: "Documenten bekijken"
      content: "Bewaar individuele documentpagina's als afbeeldingen voor toekomstige behoeften."

    # feature loop
    - icon: "search"
      title: "Handtekening zoeken"
      content: "Haal informatie op over eerder toegevoegde handtekeningen in uw documenten."

    # feature loop
    - icon: "validate"
      title: "Documentvalidatie"
      content: "Controleer de authenticiteit van handtekeningen in elk document."

    # feature loop
    - icon: "update"
      title: "Handtekeningenbeheer"
      content: "Verwijder, verplaats of wijzig handtekeningen die op een documentpagina zijn geplaatst."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codevoorbeelden"
  description: "Illustratieve voorbeelden die typische GroupDocs.Signature for Node.js via Java-bewerkingen laten zien"
  items:
    # code sample loop
    - title: "Markeer PDF met QR-codes"
      content: |
        Door [barcodes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) op te nemen in specifieke PDF-documentpagina's kunnen bedrijfsprocessen worden gestroomlijnd. In dit gedeelte wordt een voorbeeld gegeven van het toevoegen van een QR-code met behulp van GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Hoe QR-code naar PDF te zetten.">}}
        ```javascript {style=abap}
        // Laad het document dat u wilt ondertekenen
        let signature = new Signature("file_to_sign.pdf");
        
        // Maak QR-code-opties met vooraf gedefinieerde tekst
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configureer het coderingstype en de positie van de QR-code op de pagina
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Onderteken het document en sla het op als resultaatbestand
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Een DOCX beschermen met een digitale handtekening"
      content: |
        [Bescherm uw documenten](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) door handtekeningen op basis van digitale certificaten. Digitale handtekening beschermt uw zakelijke documenten tegen wijziging van de inhoud.
        {{< landing/code title="Hier leest u hoe u de documentintegriteit kunt garanderen.">}}
        ```javascript {style=abap}   
        // Laad het document dat digitaal moet worden ondertekend
        let signature = new Signature("file_to_sign.docx");
        
        // Geef opties voor digitale ondertekening op en geef het pad naar het certificaatbestand op
        let options = new DigitalSignOptions("certificate.pfx");

        // Stel het certificaatwachtwoord in
        options.Password = "1234567890";

        // Onderteken het document en sla het op in het gewenste pad
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
