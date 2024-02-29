---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:06
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
head_title: ".NET, Java, Cloud API's en online apps voor documenthandtekening"
head_description: "Ontvang een alles-in-één oplossing voor e-handtekening van documenten voor .NET, Java en cloudgebaseerde applicaties. Onderteken veelgebruikte documentformaten online met behulp van een eenvoudige functie voor slepen en neerzetten"

############################# Header ############################
title: "Onderteken documenten<br>via Java-API"
description: "Onderteken digitale documenten en afbeeldingen op elk platform met behulp van onze flexibele API's en app-gebaseerde oplossingen voor programmeurs en eindgebruikers."
words:
  for: "voor"

actions:
  main: "Gratis Maven-download"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licentie"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "klaar om te beginnen?"
  description: "Probeer de functies van GroupDocs.Signature gratis of vraag een licentie aan"

release:
  title: "Versie {0} vrijgegeven"
  notes: "Zie wat nieuw is"
  downloads: "Downloads"

code:
  title: "Onderteken PDF-bestanden in Java"
  more: "Meer voorbeelden"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Selecteer PDF-document
    Signature signature = new Signature("sample.pdf");
    
    // Geef tekst op
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Onderteken het document en sla het op in een bestand
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature-overzicht"
  description: "API voor het uitvoeren van documentondertekening en gerelateerde bewerkingen in Java-applicaties"
  features:
    # feature loop
    - title: "Verbeterde zakelijke documenten met digitale handtekeningen in Java"
      content: "Snel en aanpasbaar ondertekenen: GroupDocs.Signature voor Java biedt een breed scala aan opties voor digitale handtekeningen voor PDF's, afbeeldingen en Office-documenten. U kunt tekst, barcodes, QR-codes, digitale certificaten, afbeeldingen of verborgen metadata gebruiken. De documentverwerking is snel en efficiënt."

    # feature loop
    - title: "Het manipuleren van ondertekende documenten"
      content: "Geavanceerde documentverwerking omvat krachtige bewerkingen op ondertekende documenten met behulp van GroupDocs.Signature voor Java. U kunt handtekeningen die aan bedrijfsdocumenten zijn toegevoegd, zoeken en valideren met behulp van verschillende handige criteria. Bovendien hebt u toegang tot gedetailleerde informatie over het document of kunt u voorbeeldafbeeldingen van de pagina's verkrijgen."

    # feature loop
    - title: "Verscheidenheid aan uitvoerkeuzes"
      content: "Dankzij de robuuste ondertekeningsopties kunt u de uitvoer aanpassen voor documenten die zijn ondertekend met GroupDocs.Signature voor Java. U kunt elke handtekening nauwkeurig op elke documentpagina plaatsen en de weergave ervan op verschillende manieren configureren. De Java API ondersteunt het opslaan van ondertekende bedrijfsdocumenten in talloze ondersteunde formaten en biedt opties om deze met wachtwoorden te beveiligen."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platformonafhankelijkheid"
  description: "GroupDocs.Signature voor Java ondersteunt de volgende besturingssystemen, frameworks en pakketbeheerders"
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
  title: "Ondersteunde bestandsformaten"
  description: |
    GroupDocs.Signature voor Java ondersteunt bewerkingen met de volgende [bestandsindelingen](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  description: "PDF's, Office-documenten en afbeeldingen ondertekenen met digitale handtekeningen"

  items:
    # feature loop
    - icon: "sign"
      title: "Handtekeningen toevoegen"
      content: "Onderteken een document met verschillende ondersteunde handtekeningtypen door een digitale handtekening precies op elke positie op elke pagina te plaatsen."

    # feature loop
    - icon: "custom"
      title: "Resultaten aanpassen"
      content: "Pas het uiterlijk van de handtekening aan door de kleur, het lettertype, de rand, de rotatie en andere functies aan te passen om het gewenste resultaat te bereiken."

    # feature loop
    - icon: "password"
      title: "Documenten beveiligen met wachtwoord"
      content: "Voor veel ondersteunde documenttypen kunt u het ondertekende document beveiligen met een wachtwoord."

    # feature loop
    - icon: "protect"
      title: "Ongeautoriseerde wijzigingen voorkomen"
      content: "Bescherm belangrijke zakelijke documenten ondertekend met een digitaal certificaat tegen ongeoorloofde wijzigingen."

    # feature loop
    - icon: "convert"
      title: "Resultaten verkrijgen in gewenste formaten"
      content: "Verkrijg eenvoudig ondertekende resultaatbestanden in elk ondersteund formaat. Ook kunt u moeiteloos MS Word-documenten naar PDF converteren."

    # feature loop
    - icon: "preview"
      title: "Documentvoorbeeld"
      content: "Sla elke pagina van een document op als afbeelding voor toekomstige verwerking."

    # feature loop
    - icon: "search"
      title: "Zoeken naar handtekeningen"
      content: "Het is mogelijk om informatie te krijgen over eerder toegevoegde handtekeningen in specifieke documenten."

    # feature loop
    - icon: "validate"
      title: "Valideren van documenten"
      content: "Valideer de juistheid van handtekeningen op elk ondertekend document."

    # feature loop
    - icon: "update"
      title: "Handtekeningen beheren"
      content: "Zodra een handtekening op een documentpagina is geplaatst, kan deze indien nodig worden verwijderd, verplaatst of bijgewerkt."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codevoorbeelden"
  description: "Enkele gebruiksscenario's van typische GroupDocs.Signature voor Java-bewerkingen"
  items:
    # code sample loop
    - title: "Verbeter het PDF-document met QR-code"
      content: |
        Het kan waardevol zijn om bedrijfsprocessen te verbeteren door [QR-codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) toe te voegen aan specifieke pagina's van PDF-documenten. Er is een voorbeeld van hoe u een QR-code kunt toevoegen met GroupDocs.Signature voor Java.
        {{< landing/code title="Verbeter het PDF-document met QR-code">}}
        ```java {style=abap}
        // Laad het document dat u wilt ondertekenen
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Maak QR-code-opties met vooraf gedefinieerde tekst
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configureer het coderingstype en de positie van de QR-code op de pagina
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Onderteken het document en sla het op als resultaatbestand
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Gebruik digitale handtekening om een ​​DOCX te beschermen"
      content: |
        U kunt een document [Beveiligen](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) met behulp van persoonlijke of zakelijke handtekeningen die zijn opgeslagen als digitale certificaten. Met een certificaat beveiligde documenten kunnen niet worden gewijzigd zonder de handtekening ongeldig te maken.
        {{< landing/code title="Gebruik digitale handtekening om een ​​DOCX te beschermen">}}
        ```java {style=abap}   
        // Laad het document dat digitaal moet worden ondertekend
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Geef opties voor digitale ondertekening op en geef het pad naar het certificaatbestand op
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Stel het certificaatwachtwoord in
        options.setPassword("1234567890");

        // Onderteken het document en sla het op in het gewenste pad
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
