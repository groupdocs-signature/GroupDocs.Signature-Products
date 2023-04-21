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
head_title: "Java Digital Signature API, Legg til eSignatur til PDF Word Excel Image"
head_description: "Java digital signatur API. Elektronisk signaturbibliotek for digital signering av PDF, Microsoft Word, Excel-regneark, PowerPoint-presentasjoner og bildedokumentformater."

############################# Header ############################
title: "Java API for å administrere digitale signaturer"
description: "Administrer e-signatur av bilde-, QR-kode-, strekkode-, metadata-, tekst- og stempeltyper i Java-applikasjoner for signering av bilder og digitale dokumentfilformater."
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
              text: "Oversikt"

            # button loop
            - link: "#features"
              text: "Egenskaper"

            # button loop
            - link: "#support"
              text: "Brukerstøtte"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Prissetting"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API hjelper deg med å utvikle Java-applikasjoner med funksjonalitet for elektroniske signaturer for å signere digitale dokumenter i støttede formater uten å installere ekstern programvare. Den støtter manipulering og administrasjon av ulike typer e-signaturer som bilde, strekkode, QR-kode, stempel, tekst, optisk og metadata. Alle dine elektroniske forretningsdokumenter som Microsoft Office Word, PowerPoint-presentasjoner, Excel-regneark, bilder og PDF-filer kan signeres digitalt ved å tilpasse signaturegenskaper, f.eks. skygge, dimensjoner, justering og mer i henhold til dine krav. Det digitale signaturbiblioteket er enkelt og lett, og består av en enkelt DLL-fil som enkelt kan integreres i nye eller eksisterende Java-applikasjoner.  

      Gjennom GroupDocs.Signature for Java API kan du laste inn alle registrerte sertifikater fra systemet, eller finne eksisterende signaturer ved hjelp av enkelt og avansert søk. Alternativene for å jobbe med passordbeskyttede dokumenter, spesifisering av vanlige signaturegenskaper (tekststørrelse, opasitet, rotasjon, verifisering, skriftegenskaper, fargealternativer, sidetall, bredde, topp, venstre osv.) og støtte for implementering av forskjellige eSignaturtyper gjør det til en pålitelig e-Signaturer administrasjonsløsning for digitale dokumenter.  

      GroupDocs.Signature for Java er kompatibel med alle Java-versjoner og støtter populære operativsystemer (Windows, Linux, MacOS) som er i stand til å kjøre Java runtime
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Det er en oversikt over GroupDocs.Signature-funksjoner for Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Signaturtyper"
          content: |
            * Tekstsignatur
            * Bildesignatur
            * Digitale signaturer
            * QR-kode signatur
            * Strekkodesignatur
            * Stempel signatur
            * Skjemafeltsignatur
      
      ## TAB TWO ##
      tab_two:
        description: |
          Java elektronisk signering API støtter ulike dokumentfilformater som er oppført nedenfor. [Støttede dokumentformater.](https://docs.groupdocs.com/signature/java/supported-document-formats/)

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
                * **Bilder**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metafiler**: EMF, WMF, CMX
                * **Bærbar**: PDF
                * **Skalerbar vektorgrafikk**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Andre**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java støtter følgende operativsystemer, rammer og pakkeadministratorer:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operativsystemer"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Støttede rammer"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Utviklingsmiljøer"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Bygg automatiseringsverktøy"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature for Java-funksjoner"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Opprett, les, endre, skjul og slett e-signaturer fra støttede dokumentformater"

      # feature loop
      - icon: "fas fa-eye"
        content: "Tilgang til å være signert dokument fra strøm, relativ vei eller absolutt vei"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Bruk tekstsignatur på dokumenter, regneark, presentasjoner, bilder og PDF-filer"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Legg til tekstsignatur som merknad, klistremerke, bilde til PDF-filer. Konfigurer også stil og farge"

      # feature loop
      - icon: "fas fa-code"
        content: "Signer PDF-dokument, bildefil og få utdata i forskjellig filformat"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Signer bilder digitalt med tekstsignatur som vannmerke og legg til gjennomsiktighet, rotasjon til e-signatur"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Søk i sertifikater og signer Microsoft Word-, Excel- og PDF-dokumenter med digitale sertifikater"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Signer tekstbehandlingsdokumentformater med innfødte tekstvannmerker"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Bruk QR-kode, strekkode for å signere Word-, lysbilde-, celle-, PDF- og bildefiler"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Konfigurer og bruk stempelsignaturer for å sikre støttede filformater"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Konfigurer og tilordne bildesignaturer til dokumenter, regneark, presentasjoner, bilder og PDF-filer"

      # feature loop
      - icon: "fas fa-columns"
        content: "Konfigurer signaturegenskaper, for eksempel utseende og følelse, marginer, justering osv."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Bruk digital signatur på passordbeskyttet dokument"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Utfør tekstverifisering av PDF-dokumenter ved hjelp av signaturbehandleren"

      # feature loop
      - icon: "fas fa-print"
        content: "Digital verifisering av Word-, celle-, PDF-dokumenter med .CER- og .PFX-sertifikatbeholdere"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Spesifiser forskjellige måleenhetstyper (f.eks. millimeter, piksler osv.) for PDF-tekstsignaturer"

      # feature loop
      - icon: "fas fa-lock"
        content: "Skaff dokumentinformasjon via fil eller URL - Legg til skjemafeltsignaturer til PDF-dokumenter"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Legg til tilpasset dataobjekt, innebygd VCard, e-post, EPC, MeCard eller hendelsesobjekt i QR-koden"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Bruk forskjellige børstestiler på signaturer, for eksempel gradient, radial, solid og teksturbørste"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Signer dokument som ligger på FTP eller Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Angi tekstjustering i figurer for dokumenter, lysbilder, bilder og PDF-filer"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Søk, verifiser og signer PowerPoint-presentasjonsdokumenter digitalt"

      # feature loop
      - icon: "fas fa-cube"
        content: "Plasser signatur ved hjelp av piksler i celledokumenter og tekstplassering for stempelsignaturer"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementer rektangelstempelsignatur med avrundede hjørner"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Utvid strekkode- og QR-kodesignaturer med bildedatainnhold"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Legg til krypterte metadatasignaturer mens du arbeider med signerings- og søkealternativer"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Bygg inn tilpassede objekter til metadatasignaturer i Word, Excel og presentasjoner"

    more_feature:
      # more_feature_loop
      - title: "Enkelt konfigurere og bruke eSignaturer"
        content: |
          GroupDocs.Signature for Java API gjør det mulig å konfigurere og legge til eSignaturer til støttede dokumentformater. Følgende er et kodeeksempel som viser hvor enkelt det er å bruke en tekstsignatur på en PDF-fil:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // angi signaturposisjon
          options.setLeft(100);
          options.setTop(100);
          
          // sett signaturrektangel
          options.setWidth(100);
          options.setHeight(30);

          // angi tekstfarge og skrifttype
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // signere dokument til fil
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Støttede strekkodekodingstyper for eSignature"
        content: |
          Ved å bruke GroupDocs.Signature for Java API kan du bruke strekkode og QR-kodesignaturer på støttede filformater. GroupDocs.Signature for Java støtter et stort utvalg av strekkodekodingstyper for å imøtekomme de fleste krav. De støttede strekkodekodingstypene inkluderer kode 11, kode 128, kode 16K/32, databarkoder, GS1-kodeblokk, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard og Kode39 Utvidet.

          Tilsvarende lar GroupDocs.Signature for Java API deg bruke QR-kodetyper, som QR, Aztec og Data Matrix. Støttede QR-kode-kodingstyper inkluderer Aztec, DataMatrix, GS1 DataMatrix og GS1 QR.

      # more_feature_loop
      - title: "Søk i signaturer og sertifikater"
        content: |
          Gjennom GroupDocs.Signature for Java API kan du søke etter QR-kode- og strekkodesignaturer i ethvert dokument, presentasjon, regneark, bilde, samt PDF-fil, og hente søkeresultatet. Du kan også søke etter egendefinerte dataobjekter fra dokumenter signert med QR-kodesignatur samt Søk etter standard VCard og e-postobjekt fra dokumenter signert med QR-kode. Verifisering av kryptert tekst av QR-kodesignaturer samt søk etter metadatasignatur i PDF-dokumenter støttes også. Bruk ytterligere søkekriterier for digitale signaturer for Words & Cells-dokumenter.  

          Søkealternativ er også tilgjengelig for metadatasignatur for word-dokumenter, lysbilder og regneark, mens skjemafeltsøk er tilgjengelig for PDF-dokumenter.

      # more_feature_loop
      - title: "Konfigurer eSignature-egenskaper"
        content: |
          For å forbedre brukeropplevelsen til sluttbrukere tilbyr GroupDocs.Signature for Java API mange egenskaper som kan konfigureres ganske enkelt. Du kan angi font- og fargealternativer (bakgrunnsfarge, forgrunnsfarge, fet, kursiv, understreking, skriftfamilie, skriftstørrelse osv.), Bakgrunns- og kantalternativer (bakgrunnsfarge, bakgrunnsgjennomsiktighet, kantfarge, kantstrekstil, kantlinje, kantvekt, Border Transparency etc.), Signaturmarger (Venstre, Topp, Bredde, Høyde, Polstring etc.), og Oppsett bildesignaturområde og signaturjustering (Horisontal justering, Vertikal justering etc.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature tilbyr API-er for dokumentsignering for andre populære utviklingsmiljøer"

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