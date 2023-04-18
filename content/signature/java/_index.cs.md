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
head_title: "Java Digital Signature API, přidání elektronického podpisu do PDF Word Excel obrázku"
head_description: "Java digitální podpis API. Knihovna elektronických podpisů pro digitální podepisování PDF, Microsoft Word, Excel, prezentací PowerPoint a formátů obrazových dokumentů."

############################# Header ############################
title: "Java API pro správu digitálních podpisů"
description: "Spravujte elektronický podpis obrázků, QR-kódů, čárových kódů, metadat, textů a typů razítek v aplikacích Java pro podepisování obrázků a formátů souborů digitálních dokumentů."
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
              text: "Přehled"

            # button loop
            - link: "#features"
              text: "Funkce"

            # button loop
            - link: "#support"
              text: "Podpěra, podpora"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Živá ukázka"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Ceny"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API vám pomáhá vyvíjet aplikace Java s funkcí elektronického podpisu pro podepisování digitálních dokumentů podporovaných formátů bez instalace jakéhokoli externího softwaru. Podporuje manipulaci a správu různých typů elektronických podpisů, jako je obrázek, čárový kód, QR-kód, razítko, text, optická a metadata. Všechny vaše elektronické obchodní dokumenty, jako jsou Microsoft Office Word, prezentace PowerPoint, tabulky Excel, obrázky a soubory PDF, lze digitálně podepsat přizpůsobením vlastností podpisu, např. stín, rozměry, zarovnání a další podle vašich požadavků. Knihovna digitálních podpisů je jednoduchá a nenáročná a skládá se z jediného souboru DLL, který lze snadno integrovat do nové nebo stávající aplikace Java.  

      Prostřednictvím GroupDocs.Signature for Java API můžete načíst všechny registrované certifikáty ze systému nebo vyhledat existující podpisy pomocí jednoduchého a pokročilého vyhledávání. Možnosti práce s dokumenty chráněnými heslem, specifikace běžných vlastností podpisu (velikost textu, neprůhlednost, otočení, ověření, vlastnosti písma, barevné možnosti, číslo stránky, šířka, nahoře, vlevo atd.) a podpora implementace různých typů elektronického podpisu z něj činí spolehlivý Řešení správy elektronických podpisů pro digitální dokumenty.  

      GroupDocs.Signature for Java je kompatibilní se všemi verzemi Java a podporuje oblíbené operační systémy (Windows, Linux, MacOS), které jsou schopny spouštět Java runtime
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Toto je přehled funkcí GroupDocs.Signature pro Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Typy podpisů"
          content: |
            * Textový podpis
            * Obrazový podpis
            * Digitální podpisy
            * Podpis QR kódu
            * Podpis čárového kódu
            * Razítko Podpis
            * Podpis pole formuláře
      
      ## TAB TWO ##
      tab_two:
        description: |
          Java pro elektronické podepisování API podporuje [formáty souborů dokumentů] (https://docs.groupdocs.com/signature/java/supported-document-formats/), jak je uvedeno níže.

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
                * **snímky**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Metasoubory**: EMF, WMF, CMX
                * **Přenosný**: PDF
                * **Škálovatelná vektorová grafika**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Ostatní**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java podporuje následující operační systémy, rámce a správce balíčků:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operační systémy"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Podporované rámce"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Vývojová prostředí"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Nástroj Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Signature for Java Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Vytvářejte, čtěte, upravujte, schovávejte a mažte elektronické podpisy z podporovaných formátů dokumentů"

      # feature loop
      - icon: "fas fa-eye"
        content: "Přístup k podepsanému dokumentu ze streamu, relativní cesty nebo absolutní cesty"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Použijte textový podpis na dokumenty, tabulky, prezentace, obrázky a soubory PDF"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Přidejte textový podpis jako anotaci, nálepku, obrázek do souborů PDF a konfigurujte styl a barvu"

      # feature loop
      - icon: "fas fa-code"
        content: "Podepište dokument PDF, soubor obrázku a získejte výstup v jiném formátu souboru"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Digitálně podepisujte obrázky textovým podpisem jako vodoznakem a přidejte průhlednost, otočení k elektronickému podpisu"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Vyhledávejte certifikáty a podepisujte dokumenty Microsoft Word, Excel a PDF pomocí digitálních certifikátů"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Podepisujte formáty dokumentů pro zpracování textu pomocí nativních textových vodoznaků"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Použijte QR kód, čárový kód k podepsání souborů Word, Slide, Buňka, PDF a obrázky"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Konfigurace a použití podpisů razítek na zabezpečené podporované formáty souborů"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Nastavení a přiřazení obrazových podpisů k dokumentům, tabulkám, prezentacím, obrázkům a souborům PDF"

      # feature loop
      - icon: "fas fa-columns"
        content: "Nakonfigurujte vlastnosti podpisu, např. vzhled a dojem, okraje, zarovnání atd."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Použijte digitální podpis na dokument chráněný heslem"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Proveďte ověření textu dokumentů PDF pomocí nástroje Signature Handler"

      # feature loop
      - icon: "fas fa-print"
        content: "Digitální ověřování dokumentů Word, Cell, PDF pomocí kontejnerů certifikátů .CER a .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Zadejte různé typy měrných jednotek (např. milimetry, pixely atd.) pro textové podpisy PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Získejte informace o dokumentu prostřednictvím souboru nebo adresy URL – přidejte do dokumentů PDF podpisy polí formuláře"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Přidejte vlastní datový objekt, vložený VCard, e-mail, EPC, MeCard nebo objekt události do QR-Code"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Použít různé styly štětců na podpisy, např. přechodový, radiální, plný a texturový štětec"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Podepište dokument umístěný na FTP nebo Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Nastavte zarovnání textu uvnitř Shapes pro dokumenty, snímky, obrázky a soubory PDF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Vyhledávejte, ověřujte a digitálně podepisujte prezentační dokumenty aplikace PowerPoint"

      # feature loop
      - icon: "fas fa-cube"
        content: "Umístěte podpis pomocí pixelů do dokumentů buňky a umístění textu pro podpisy razítka"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementujte podpis obdélníkového razítka se zaoblenými rohy"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Rozšiřte podpisy čárových kódů a QR kódů o obsah obrazových dat"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Přidejte šifrované podpisy metadat při práci s možnostmi podepisování a vyhledávání"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Vkládání vlastních objektů do metadatových podpisů ve Wordu, Excelu a prezentacích"

    more_feature:
      # more_feature_loop
      - title: "Snadná konfigurace a použití elektronických podpisů"
        content: |
          GroupDocs.Signature for Java API umožňuje konfigurovat a přidávat elektronické podpisy do podporovaných formátů dokumentů. Následuje příklad kódu, který ukazuje, jak jednoduché je použít textový podpis na soubor PDF:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // nastavit pozici podpisu
          options.setLeft(100);
          options.setTop(100);
          
          // nastavit obdélník podpisu
          options.setWidth(100);
          options.setHeight(30);

          // nastavit barvu textu a písmo
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // podepsat dokument do souboru
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Podporované typy kódování čárových kódů pro elektronický podpis"
        content: |
          Pomocí GroupDocs.Signature for Java API můžete použít podpisy čárových kódů a QR kódů na podporované formáty souborů. GroupDocs.Signature for Java podporuje širokou škálu typů kódování čárových kódů, aby vyhovovaly většině požadavků. Mezi podporované typy kódování čárových kódů patří, Code 11, Code 128, Code 16K/32, Databar codes, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard a Rozšířený kód 39.

          Podobně GroupDocs.Signature for Java API vám umožňuje používat typy QR kódů, jako jsou QR, Aztec a Data Matrix. Mezi podporované typy kódování QR-Code patří Aztec, DataMatrix, GS1 DataMatrix a GS1 QR.

      # more_feature_loop
      - title: "Hledat podpisy a certifikáty"
        content: |
          Prostřednictvím GroupDocs.Signature for Java API můžete vyhledávat podpisy QR-Code a Barcode v jakémkoli dokumentu, prezentaci, tabulce, obrázku i souboru PDF a získat výsledek vyhledávání. Můžete také vyhledávat vlastní datové objekty z dokumentů podepsaných podpisem QR-Code a také prohledávat standardní VCard a e-mailový objekt z dokumentů podepsaných QR-kódem. Podporováno je také ověřování zašifrovaného textu podpisů QR-Code a hledání podpisu metadat v dokumentech PDF. Použijte další vyhledávací kritéria pro digitální podpisy dokumentů Words & Cells.  

          Možnost vyhledávání je také dostupná pro podpis metadat pro dokumenty Word, snímky a tabulky, zatímco pro dokumenty PDF je k dispozici vyhledávání v poli formuláře.

      # more_feature_loop
      - title: "Nakonfigurujte vlastnosti elektronického podpisu"
        content: |
          Pro vylepšení uživatelského rozhraní koncových uživatelů GroupDocs.Signature for Java API poskytuje mnoho vlastností, které lze velmi snadno konfigurovat. Můžete nastavit možnosti písma a barvy (Barva pozadí, Barva popředí, Tučné, Kurzíva, Podtržení, Rodina písem, Velikost písma atd.), Možnosti pozadí a ohraničení (Barva pozadí, Průhlednost pozadí, Barva ohraničení, Styl čárky ohraničení, Tloušťka ohraničení, Průhlednost okrajů atd.), Okraje podpisu (vlevo, nahoře, šířka, výška, odsazení atd.) a nastavení oblasti podpisu obrazu a zarovnání podpisu (horizontální zarovnání, svislé zarovnání atd.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature nabízí rozhraní API pro prohlížení dokumentů pro další populární vývojová prostředí"

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