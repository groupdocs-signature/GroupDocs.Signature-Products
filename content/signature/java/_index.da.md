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
head_title: "Java Digital Signature API, Føj eSignatur til PDF Word Excel-billede"
head_description: "Java digital signatur API. Elektronisk signaturbibliotek til digital signering af PDF, Microsoft Word, Excel-regneark, PowerPoint-præsentationer og billeddokumentformater."

############################# Header ############################
title: "Java API til at administrere digitale signaturer"
description: "Administrer eSignatur af billed-, QR-kode-, stregkode-, metadata-, tekst- og stempeltyper i Java-applikationer til signering af billeder og digitale dokumentfilformater."
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
              text: "Oversigt"

            # button loop
            - link: "#features"
              text: "Funktioner"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Live demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Prissætning"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API hjælper dig med at udvikle Java-applikationer med elektroniske signaturfunktioner til at signere digitale dokumenter i understøttede formater uden at installere ekstern software. Det understøtter manipulation og styring af forskellige typer e-signaturer såsom billede, stregkode, QR-kode, stempel, tekst, optisk og metadata. Alle dine elektroniske forretningsdokumenter som Microsoft Office Word, PowerPoint-præsentationer, Excel-regneark, billeder og PDF-filer kan signeres digitalt ved at tilpasse signaturegenskaber, f.eks. skygge, dimensioner, justering og mere i henhold til dine krav. Det digitale signaturbibliotek er enkelt og let og består af en enkelt DLL-fil, der nemt kan integreres i en ny eller en eksisterende Java-applikation.  

      Gennem GroupDocs.Signature for Java API kan du indlæse alle registrerede certifikater fra systemet, eller lokalisere eksisterende signaturer ved hjælp af enkel og avanceret søgning. Mulighederne for at arbejde med adgangskodebeskyttede dokumenter, specificering af almindelige signaturegenskaber (tekststørrelse, opacitet, rotation, verifikation, skrifttypeegenskaber, farveindstillinger, sidenummer, bredde, top, venstre osv.) og understøttelse af implementering af forskellige eSignaturtyper gør det til en pålidelig e-Signaturer administrationsløsning til digitale dokumenter.  

      GroupDocs.Signature for Java er kompatibel med alle Java-versioner og understøtter populære operativsystemer (Windows, Linux, MacOS), der er i stand til at køre Java runtime
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Det er en oversigt over GroupDocs.Signature-funktioner til Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Signaturtyper"
          content: |
            * Tekst signatur
            * Billedsignatur
            * Digitale signaturer
            * QR-kode signatur
            * Stregkode signatur
            * Stempel signatur
            * Form-felt Signatur
      
      ## TAB TWO ##
      tab_two:
        description: |
          Java elektronisk signering API understøtter forskellige dokumentfilformater som angivet nedenfor. [Understøttede dokumentformater.](https://docs.groupdocs.com/signature/java/supported-document-formats/)

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
                * **Billeder**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metafiler**: EMF, WMF, CMX
                * **Transportabel**: PDF
                * **Skalerbar vektorgrafik**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Andre**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature til Java understøtter følgende operativsystemer, rammer og pakkeadministratorer:
        
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
              title: "Understøttede rammer"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Udviklingsmiljøer"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Byg automatiseringsværktøj"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature til Java-funktioner"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Opret, læs, rediger, skjul og slet e-signaturer fra understøttede dokumentformater"

      # feature loop
      - icon: "fas fa-eye"
        content: "Adgang til at blive underskrevet dokument fra stream, relativ sti eller absolut sti"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Anvend tekstsignatur på dokumenter, regneark, præsentationer, billeder og PDF-filer"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Tilføj tekstsignatur som annotering, klistermærke, billede til PDF-filer Konfigurer også stil og farve"

      # feature loop
      - icon: "fas fa-code"
        content: "Signer PDF-dokument, billedfil og få output i andet filformat"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Signer billeder digitalt med tekstsignatur som vandmærke og tilføj gennemsigtighed, rotation til eSignatur"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Søg i certifikater og underskriv Microsoft Word-, Excel- og PDF-dokumenter med digitale certifikater"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Signer tekstbehandlingsdokumentformater med indbyggede tekstvandmærker"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Brug QR-kode, stregkode til at signere Word-, Slide-, Celle-, PDF- og billedfiler"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Konfigurer og anvend stempelsignaturer til sikre understøttede filformater"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Konfigurer og tildel billedsignaturer til dokumenter, regneark, præsentationer, billeder og PDF-filer"

      # feature loop
      - icon: "fas fa-columns"
        content: "Konfigurer signaturegenskaber, f.eks. udseende og fornemmelse, marginer, justering osv."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Anvend digital signatur på adgangskodebeskyttet dokument"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Udfør tekstbekræftelse af PDF-dokumenter ved hjælp af signaturhandleren"

      # feature loop
      - icon: "fas fa-print"
        content: "Digital verifikation af Word-, celle-, PDF-dokumenter med .CER- og .PFX-certifikatbeholdere"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Angiv forskellige måleenhedstyper (f.eks. millimeter, pixel osv.) for PDF-tekstsignaturer"

      # feature loop
      - icon: "fas fa-lock"
        content: "Få dokumentoplysninger via fil eller URL - Tilføj formularfeltsignaturer til PDF-dokumenter"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Tilføj Custom Data Object, Embedded VCard, Email, EPC, MeCard eller Event Object til QR-koden"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Anvend forskellige penselstile på signaturer, f.eks. Gradient, Radial, Solid og Texture Brush"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Signer dokument placeret på FTP eller Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Indstil tekstjustering inde i figurer for dokumenter, dias, billeder og PDF-filer"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Søg, bekræft og underskriv PowerPoint-præsentationsdokumenter digitalt"

      # feature loop
      - icon: "fas fa-cube"
        content: "Placer signatur ved hjælp af pixel i celledokumenter og tekstpositionering til stempelsignaturer"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementer rektangel stempelsignatur med afrundede hjørner"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Udvid stregkode- og QR-kodesignaturer med billeddataindhold"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Tilføj krypterede metadatasignaturer, mens du arbejder med signerings- og søgemuligheder"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Integrer tilpassede objekter til metadatasignaturer i Word, Excel og Præsentationer"

    more_feature:
      # more_feature_loop
      - title: "Konfigurer og anvend nemt eSignaturer"
        content: |
          GroupDocs.Signature for Java API gør det muligt at konfigurere og tilføje eSignaturer til understøttede dokumentformater. Følgende er et kodeeksempel, der viser, hvor nemt det er at anvende en tekstsignatur på en PDF-fil:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // indstille signaturposition
          options.setLeft(100);
          options.setTop(100);
          
          // sæt signaturrektangel
          options.setWidth(100);
          options.setHeight(30);

          // indstille tekstfarve og skrifttype
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // underskrive dokument til fil
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Understøttede stregkodekodningstyper til eSignature"
        content: |
          Ved at bruge GroupDocs.Signature til Java API kan du anvende stregkode- og QR-kodesignaturer på understøttede filformater. GroupDocs.Signature til Java understøtter et stort udvalg af stregkodekodningstyper for at imødekomme de fleste krav. De understøttede stregkodekodningstyper omfatter kode 11, kode 128, kode 16K/32, datastregkoder, GS1 kodeblok, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard og Kode39 Udvidet.

          Tilsvarende giver GroupDocs.Signature for Java API dig mulighed for at bruge QR-kodetyper, såsom QR, Aztec og Data Matrix. Understøttede QR-kode-kodningstyper omfatter Aztec, DataMatrix, GS1 DataMatrix og GS1 QR.

      # more_feature_loop
      - title: "Søg efter signaturer og certifikater"
        content: |
          Gennem GroupDocs.Signature for Java API kan du søge efter QR-kode og stregkodesignaturer i ethvert dokument, præsentation, regneark, billede samt PDF-fil og hente søgeresultatet. Du kan også søge efter brugerdefinerede dataobjekter fra dokumenter, der er signeret med QR-kodesignatur samt Søg efter standard VCard og e-mailobjekt fra dokumenter, der er signeret med QR-kode. Bekræftelse af krypteret tekst af QR-kodesignaturer samt søgning efter metadatasignatur i PDF-dokumenter understøttes også. Anvend yderligere søgekriterier for digitale signaturer af Words & Cells-dokumenter.  

          Søgemulighed er også tilgængelig for metadatasignatur til word-dokumenter, dias og regneark, mens formularfeltsøgning er tilgængelig for PDF-dokumenter.

      # more_feature_loop
      - title: "Konfigurer eSignature-egenskaber"
        content: |
          For at forbedre brugernes brugervenlighed giver GroupDocs.Signature for Java API en masse egenskaber, der kan konfigureres ret nemt. Du kan indstille skrifttype- og farveindstillinger (baggrundsfarve, forgrundsfarve, fed, kursiv, understregning, skrifttypefamilie, skriftstørrelse osv.), Baggrunds- og kantindstillinger (baggrundsfarve, baggrundsgennemsigtighed, kantfarve, kantstregstil, kantlinje, kantvægt, Kantgennemsigtighed osv.), Signaturmargener (Venstre, Top, Bredde, Højde, Polstring osv.) og Opsætning af billedsignaturområde og signaturjustering (Horisontal justering, Lodret justering osv.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature tilbyder dokumentsignerings-API'er til andre populære udviklingsmiljøer"

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