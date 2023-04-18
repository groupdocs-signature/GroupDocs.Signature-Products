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
head_title: "Java Digital Signature API, Lägg till eSignatur till PDF Word Excel Image"
head_description: "Java digital signatur API. Elektroniskt signaturbibliotek för att digitalt signera PDF, Microsoft Word, Excel-kalkylblad, PowerPoint-presentationer och bilddokumentformat."

############################# Header ############################
title: "Java API för att hantera digitala signaturer"
description: "Hantera e-signatur av bild-, QR-kod-, streckkods-, metadata-, text- och stämpeltyper i Java-applikationer för signering av bilder och digitala dokumentfilformat."
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
              text: "Översikt"

            # button loop
            - link: "#features"
              text: "Funktioner"

            # button loop
            - link: "#support"
              text: "Stöd"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Live-demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Prissättning"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API hjälper dig att utveckla Java-applikationer med elektroniska signaturfunktioner för att signera digitala dokument i format som stöds utan att installera någon extern programvara. Den stöder manipulation och hantering av olika typer av e-signaturer som bild, streckkod, QR-kod, stämpel, text, optisk och metadata. Alla dina elektroniska affärsdokument som Microsoft Office Word, PowerPoint-presentationer, Excel-kalkylblad, bilder och PDF-filer kan signeras digitalt genom att anpassa signaturegenskaper t.ex. skugga, dimensioner, justering och mer enligt dina krav. Det digitala signaturbiblioteket är enkelt och lätt och består av en enda DLL-fil som enkelt kan integreras i nya eller befintliga Java-applikationer.  

      Genom GroupDocs.Signature för Java API kan du ladda alla registrerade certifikat från systemet, eller hitta befintliga signaturer med enkel och avancerad sökning. Alternativen att arbeta med lösenordsskyddade dokument, ange vanliga signaturegenskaper (textstorlek, opacitet, rotation, verifiering, teckensnittsegenskaper, färgalternativ, sidnummer, bredd, topp, vänster etc) och stöd för att implementera olika e-signaturtyper gör det till en pålitlig Hanteringslösning för e-signaturer för digitala dokument.  

      GroupDocs.Signature för Java är kompatibel med alla Java-versioner och stöder populära operativsystem (Windows, Linux, MacOS) som kan köra Java runtime
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Det är en översikt över GroupDocs.Signature-funktioner för Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Signaturtyper"
          content: |
            * Text Signatur
            * Bildsignatur
            * Digitala signaturer
            * QR-kod signatur
            * Streckkodssignatur
            * Stämpel Signatur
            * Formfältsignatur
      
      ## TAB TWO ##
      tab_two:
        description: |
          Java elektroniskt signerings-API stöder [dokumentfilformat](https://docs.groupdocs.com/signature/java/supported-document-formats/) enligt listan nedan.

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
                * **Bärbar**: PDF
                * **Skalbar vektorgrafik**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Andra**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature för Java stöder följande operativsystem, ramar och pakethanterare:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operativsystem"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Ramar som stöds"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Utvecklingsmiljöer"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Bygg automationsverktyg"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature för Java-funktioner"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Skapa, läs, ändra, dölj och ta bort e-signaturer från dokumentformat som stöds"

      # feature loop
      - icon: "fas fa-eye"
        content: "Tillgång till ett signerat dokument från Stream, Relative Path eller Absolute Path"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Använd textsignatur på dokument, kalkylblad, presentationer, bilder och PDF-filer"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Lägg till textsignatur som anteckning, klistermärke, bild till PDF-filer Konfigurera även stil och färg"

      # feature loop
      - icon: "fas fa-code"
        content: "Signera PDF-dokument, bildfil och få utdata i olika filformat"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Signera bilder digitalt med textsignatur som vattenstämpel och lägg till transparens, rotation till e-signatur"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Sök efter certifikat och signera Microsoft Word-, Excel- och PDF-dokument med digitala certifikat"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Signera ordbehandlingsdokumentformat med inbyggda textvattenstämplar"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Använd QR-kod, streckkod för att signera Word-, Slide-, Cell-, PDF- och bildfiler"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Konfigurera och tillämpa stämpelsignaturer för att säkra filformat som stöds"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Konfigurera och tilldela bildsignaturer till dokument, kalkylblad, presentationer, bilder och PDF-filer"

      # feature loop
      - icon: "fas fa-columns"
        content: "Konfigurera signaturegenskaper, t.ex. utseende och känsla, marginaler, justering etc."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Använd digital signatur på lösenordsskyddat dokument"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Utför textverifiering av PDF-dokument med hjälp av signaturhanteraren"

      # feature loop
      - icon: "fas fa-print"
        content: "Digital verifiering av Word-, cell-, PDF-dokument med .CER- och .PFX-certifikatbehållare"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Ange olika måttenhetstyper (t.ex. millimeter, pixlar etc.) för PDF-textsignaturer"

      # feature loop
      - icon: "fas fa-lock"
        content: "Få dokumentinformation via fil eller URL - Lägg till formulärfältsignaturer till PDF-dokument"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Lägg till Custom Data Object, Embedded VCard, Email, EPC, MeCard eller Event Object till QR-koden"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Applicera olika borststilar på signaturer, t.ex. Gradient, Radial, Solid och Texture Brush"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Signera dokument som finns på FTP eller Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Ställ in textjustering i former för dokument, bilder, bilder och PDF-filer"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Sök, verifiera och signera PowerPoint-presentationsdokument digitalt"

      # feature loop
      - icon: "fas fa-cube"
        content: "Placera signatur med hjälp av pixlar i celldokument och textpositionering för stämpelsignaturer"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementera rektangelstämpelsignatur med rundade hörn"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Utöka streckkods- och QR-kodsignaturer med bilddatainnehåll"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Lägg till krypterade metadatasignaturer medan du arbetar med signerings- och sökalternativ"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Bädda in anpassade objekt till metadatasignaturer i Word, Excel och Presentationer"

    more_feature:
      # more_feature_loop
      - title: "Enkelt konfigurera och använda e-signaturer"
        content: |
          GroupDocs.Signature for Java API gör det möjligt att konfigurera och lägga till eSignaturer till dokumentformat som stöds. Följande är ett kodexempel som visar hur enkelt det är att applicera en textsignatur på en PDF-fil:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // ställ in signaturposition
          options.setLeft(100);
          options.setTop(100);
          
          // ange signatur rektangel
          options.setWidth(100);
          options.setHeight(30);

          // ställ in textfärg och teckensnitt
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // underteckna dokument till fil
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Stöd för streckkodskodningstyper för e-signatur"
        content: |
          Med hjälp av GroupDocs.Signature för Java API kan du använda streckkoder och QR-kodsignaturer på filformat som stöds. GroupDocs.Signature för Java stöder ett stort antal streckkodstyper för att tillgodose de flesta krav. De typer av streckkodskodning som stöds inkluderar kod 11, kod 128, kod 16K/32, datastreckkoder, GS1-kodblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard och Kod39 Utökad.

          På samma sätt låter GroupDocs.Signature för Java API använda QR-kodtyper, såsom QR, Aztec och Data Matrix. QR-kodstyper som stöds inkluderar Aztec, DataMatrix, GS1 DataMatrix och GS1 QR.

      # more_feature_loop
      - title: "Sök efter signaturer och certifikat"
        content: |
          Genom GroupDocs.Signature for Java API kan du söka efter QR-kod- och streckkodsignaturer i alla dokument, presentationer, kalkylblad, bilder, samt PDF-filer, och hämta sökresultatet. Du kan också söka efter anpassade dataobjekt från dokument signerade med QR-kodsignatur samt Sök efter standard VCard och e-postobjekt från dokument signerade med QR-kod. Verifiering av krypterad text av QR-kodsignaturer samt sökning efter metadatasignatur i PDF-dokument stöds också. Tillämpa ytterligare sökkriterier för digitala signaturer av Words & Cells-dokument.  

          Sökalternativ är också tillgängligt för metadatasignatur för word-dokument, bilder och kalkylblad, medan formulärfältssökning är tillgängligt för PDF-dokument.

      # more_feature_loop
      - title: "Konfigurera eSignature-egenskaper"
        content: |
          För att förbättra användarupplevelsen för slutanvändare tillhandahåller GroupDocs.Signature för Java API många egenskaper som kan konfigureras ganska enkelt. Du kan ställa in teckensnitt och färgalternativ (bakgrundsfärg, förgrundsfärg, fetstil, kursiv, understruken, teckensnittsfamilj, teckenstorlek etc.), bakgrunds- och ramalternativ (bakgrundsfärg, bakgrundstransparens, kantfärg, kantstreckstil, kantvikt, Kantgenomskinlighet etc.), Signaturmarginaler (vänster, topp, bredd, höjd, stoppning etc.), och ställ in bildsignaturområde & signaturjustering (horisontell justering, vertikal justering etc.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature erbjuder API:er för dokumentvisning för andra populära utvecklingsmiljöer"

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