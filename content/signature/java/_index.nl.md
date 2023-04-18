---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Digital Signature API, voeg eSignature toe aan PDF Word Excel Image"
head_description: "Java-API voor digitale handtekeningen. Bibliotheek met elektronische handtekeningen voor het digitaal ondertekenen van PDF-, Microsoft Word-, Excel-spreadsheets, PowerPoint-presentaties en afbeeldingsdocumentindelingen."

############################# Header ############################
title: "Java API om digitale handtekeningen te beheren"
description: "Beheer e-handtekeningen van afbeeldingen, QR-codes, streepjescodes, metagegevens, tekst- en stempeltypen in Java-toepassingen voor het ondertekenen van afbeeldingen en bestandsindelingen voor digitale documenten."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overzicht"

            # button loop
            - link: "#features"
              text: "Functies"

            # button loop
            - link: "#support"
              text: "Steun"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Live demonstratie"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "prijzen"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API helpt u bij het ontwikkelen van Java-toepassingen met functionaliteit voor elektronische handtekeningen om digitale documenten van ondersteunde indelingen te ondertekenen zonder externe software te installeren. Het ondersteunt manipulatie en beheer van verschillende soorten e-handtekeningen, zoals afbeelding, streepjescode, QR-code, stempel, tekst, optisch en metadata. Al uw elektronische zakelijke documenten zoals Microsoft Office Word, PowerPoint-presentaties, Excel-spreadsheets, afbeeldingen en PDF-bestanden kunnen digitaal worden ondertekend door handtekeningeigenschappen aan te passen, b.v. schaduw, afmetingen, uitlijning en meer volgens uw vereisten. De bibliotheek met digitale handtekeningen is eenvoudig en lichtgewicht en bestaat uit een enkel DLL-bestand dat gemakkelijk kan worden geïntegreerd in een nieuwe of bestaande Java-toepassing.  

      Via GroupDocs.Signature for Java API kunt u alle geregistreerde certificaten van het systeem laden of bestaande handtekeningen lokaliseren met behulp van eenvoudig en geavanceerd zoeken. De opties om te werken met documenten die met een wachtwoord zijn beveiligd, waarbij gemeenschappelijke handtekeningeigenschappen worden gespecificeerd (tekstgrootte, dekking, rotatie, verificatie, lettertype-eigenschappen, kleuropties, paginanummer, breedte, boven, links enz.) en ondersteuning voor het implementeren van verschillende eSignature-typen maken het een betrouwbare Oplossing voor het beheer van e-handtekeningen voor digitale documenten.  

      GroupDocs.Signature voor Java is compatibel met alle Java-versies en ondersteunt populaire besturingssystemen (Windows, Linux, MacOS) die Java runtime kunnen uitvoeren
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Dat is een overzicht van GroupDocs.Signature-functies voor Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "handtekening typen"
          content: |
            * Tekst handtekening
            * Afbeelding Handtekening
            * Digitale handtekeningen
            * QR-code handtekening
            * Barcode handtekening
            * Stempel Handtekening
            * Formulier-veld Handtekening
      
      ## TAB TWO ##
      tab_two:
        description: |
          Java-API voor elektronische ondertekening ondersteunt [documentbestandsindelingen](https://docs.groupdocs.com/signature/java/supported-document-formats/) zoals hieronder vermeld.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **Afbeeldingen**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metabestanden**: EMF, WMF, CMX
                * **Draagbaar**: PDF
                * **Schaalbare vectorafbeeldingen**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Anderen**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature voor Java ondersteunt de volgende besturingssystemen, frameworks en pakketbeheerders:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Besturingssystemen"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Ondersteunde kaders"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Ontwikkelomgevingen"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Bouw automatiseringstool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature voor Java-functies"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Maak, lees, wijzig, verberg en verwijder e-handtekeningen van ondersteunde documentindelingen"

      # feature loop
      - icon: "fas fa-eye"
        content: "Toegang tot ondertekend document van stroom, relatief pad of absoluut pad"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Pas teksthandtekeningen toe op documenten, spreadsheets, presentaties, afbeeldingen en pdf-bestanden"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Voeg teksthandtekening toe als annotatie, sticker, afbeelding aan PDF-bestanden en configureer ook stijl en kleur"

      # feature loop
      - icon: "fas fa-code"
        content: "Onderteken PDF-document, afbeeldingsbestand en ontvang uitvoer in verschillende bestandsindelingen"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Onderteken afbeeldingen digitaal met teksthandtekening als watermerk en voeg transparantie, rotatie toe aan eSignature"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Doorzoek certificaten en onderteken Microsoft Word-, Excel- en PDF-documenten met digitale certificaten"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Onderteken tekstverwerkingsdocumentindelingen met native tekstwatermerken"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Gebruik QR-code, barcode om Word-, Slide-, Cell-, PDF- en afbeeldingsbestanden te ondertekenen"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Stempelhandtekeningen configureren en toepassen op beveiligde ondersteunde bestandsindelingen"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Afbeeldingshandtekeningen instellen en toewijzen aan documenten, spreadsheets, presentaties, afbeeldingen en PDF-bestanden"

      # feature loop
      - icon: "fas fa-columns"
        content: "Configureer Handtekeningeigenschappen, bijv. Look and Feel, Marges, Uitlijning etc."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Digitale handtekening toepassen op met wachtwoord beveiligd document"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Voer tekstverificatie van PDF-documenten uit met behulp van de Signature Handler"

      # feature loop
      - icon: "fas fa-print"
        content: "Digitale verificatie van Word-, Cell- en PDF-documenten met .CER- en .PFX-certificaatcontainers"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Geef verschillende maateenheden op (bijv. millimeters, pixels enz.) voor PDF-teksthandtekeningen"

      # feature loop
      - icon: "fas fa-lock"
        content: "Verkrijg documentinformatie via bestand of URL - Voeg formulierveldhandtekeningen toe aan PDF-documenten"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Voeg aangepast gegevensobject, ingesloten VCard, e-mail, EPC, MeCard of gebeurtenisobject toe aan QR-code"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Pas verschillende penseelstijlen toe op handtekeningen, bijv. Verlooppenseel, radiaal penseel, effen penseel en textuurpenseel"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Document ondertekenen Bevindt zich op FTP of Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Stel tekstuitlijning in vormen in voor documenten, dia's, afbeeldingen en pdf-bestanden"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Zoek, verifieer en onderteken PowerPoint-presentatiedocumenten digitaal"

      # feature loop
      - icon: "fas fa-cube"
        content: "Plaats handtekening met behulp van pixels in celdocumenten en tekstpositionering voor stempelhandtekeningen"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementeer rechthoekige stempelhandtekening met afgeronde hoeken"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Breid barcode- en QR-codehandtekeningen uit met beeldgegevensinhoud"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Voeg versleutelde metagegevenshandtekeningen toe terwijl u werkt met ondertekenings- en zoekopties"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Voeg aangepaste objecten toe aan metagegevenshandtekeningen in Word, Excel en presentaties"

    more_feature:
      # more_feature_loop
      - title: "Eenvoudig eSignatures configureren en toepassen"
        content: |
          GroupDocs.Signature for Java API maakt het mogelijk om eSignatures te configureren en toe te voegen aan ondersteunde documentindelingen. Hieronder volgt een codevoorbeeld dat laat zien hoe eenvoudig het is om een ​​teksthandtekening toe te passen op een PDF-bestand:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // handtekeningpositie instellen
          options.setLeft(100);
          options.setTop(100);
          
          // handtekening rechthoek instellen
          options.setWidth(100);
          options.setHeight(30);

          // stel tekstkleur en lettertype in
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // document ondertekenen om in te dienen
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Ondersteunde typen barcodecodering voor eSignature"
        content: |
          Met GroupDocs.Signature for Java API kunt u barcode- en QR-codehandtekeningen toepassen op ondersteunde bestandsindelingen. GroupDocs.Signature voor Java ondersteunt een groot aantal typen barcodecodering om aan de meeste eisen te voldoen. De ondersteunde soorten streepjescodecodering zijn: Code 11, Code 128, Code 16K/32, Databar-codes, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard en Code39 verlengd.

          Op dezelfde manier kunt u met GroupDocs.Signature for Java API QR-codetypen gebruiken, zoals QR, Aztec en Data Matrix. Ondersteunde QR-Code-coderingstypen zijn onder meer Aztec, DataMatrix, GS1 DataMatrix en GS1 QR.

      # more_feature_loop
      - title: "Zoek Handtekeningen & Certificaten"
        content: |
          Via GroupDocs.Signature for Java API kunt u zoeken naar handtekeningen van QR-codes en streepjescodes in elk document, presentatie, spreadsheet, afbeelding en PDF-bestand, en het zoekresultaat ophalen. U kunt ook aangepaste gegevensobjecten zoeken in documenten die zijn ondertekend met QR-Code-handtekening, evenals in standaard VCard- en e-mailobjecten zoeken in documenten die zijn ondertekend met QR-code. Het verifiëren van gecodeerde tekst van QR-codehandtekeningen en het zoeken naar metadatahandtekeningen in PDF-documenten wordt ook ondersteund. Pas aanvullende zoekcriteria toe voor digitale handtekeningen van Words & Cells-documenten.  

          De zoekoptie is ook beschikbaar voor metadatahandtekeningen voor Word-documenten, dia's en spreadsheets, terwijl zoeken in formuliervelden beschikbaar is voor PDF-documenten.

      # more_feature_loop
      - title: "Configureer eSignature-eigenschappen"
        content: |
          Om de UX van eindgebruikers te verbeteren, biedt GroupDocs.Signature for Java API veel eigenschappen die vrij eenvoudig kunnen worden geconfigureerd. U kunt lettertype- en kleuropties instellen (Achtergrondkleur, Voorgrondkleur, Vet, Cursief, Onderstrepen, Lettertypefamilie, Lettergrootte enz.), Achtergrond- en randopties (Achtergrondkleur, Achtergrondtransparantie, Randkleur, Randstreepstijl, Randdikte, Randtransparantie enz.), Handtekeningmarges (links, boven, breedte, hoogte, opvulling enz.) en Instelling beeldhandtekeninggebied en handtekeninguitlijning (horizontale uitlijning, verticale uitlijning enz.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature biedt API's voor het bekijken van documenten voor andere populaire ontwikkelomgevingen"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---