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
head_title: "Java Digital Signature API, pridanie elektronického podpisu do obrázka PDF Word Excel"
head_description: "Java digitálny podpis API. Knižnica elektronických podpisov na digitálne podpisovanie PDF, Microsoft Word, Excel, prezentácií PowerPoint a formátov obrázkových dokumentov."

############################# Header ############################
title: "Java API na správu digitálnych podpisov"
description: "Spravujte elektronický podpis obrázkov, QR-kódov, čiarových kódov, metadát, textov a typov pečiatok v aplikáciách Java na podpisovanie obrázkov a formátov súborov digitálnych dokumentov."
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
              text: "Prehľad"

            # button loop
            - link: "#features"
              text: "Vlastnosti"

            # button loop
            - link: "#support"
              text: "podpora"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Živá ukážka"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Stanovenie cien"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API vám pomáha vyvíjať Java aplikácie s funkciou elektronického podpisu na podpisovanie digitálnych dokumentov podporovaných formátov bez inštalácie akéhokoľvek externého softvéru. Podporuje manipuláciu a správu rôznych typov elektronických podpisov, ako sú obrázok, čiarový kód, QR kód, pečiatka, text, optické a metadáta. Všetky vaše elektronické obchodné dokumenty, ako sú Microsoft Office Word, prezentácie v PowerPointe, excelové tabuľky, obrázky a súbory PDF, možno digitálne podpísať prispôsobením vlastností podpisu, napr. tieň, rozmery, zarovnanie a ďalšie podľa vašich požiadaviek. Knižnica digitálnych podpisov je jednoduchá a nenáročná, pozostáva z jedného súboru DLL, ktorý možno ľahko integrovať do novej alebo existujúcej aplikácie Java.  

      Prostredníctvom GroupDocs.Signature for Java API môžete načítať všetky registrované certifikáty zo systému alebo vyhľadať existujúce podpisy pomocou jednoduchého a pokročilého vyhľadávania. Možnosti práce s dokumentmi chránenými heslom, špecifikácia bežných vlastností podpisu (veľkosť textu, nepriehľadnosť, otočenie, overenie, vlastnosti písma, farebné možnosti, číslo strany, šírka, hore, vľavo atď.) a podpora implementácie rôznych typov elektronického podpisu z neho robia spoľahlivý Riešenie správy elektronických podpisov pre digitálne dokumenty.  

      GroupDocs.Signature for Java je kompatibilný so všetkými verziami Java a podporuje populárne operačné systémy (Windows, Linux, MacOS), ktoré sú schopné spúšťať Java runtime
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Toto je prehľad funkcií GroupDocs.Signature pre Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Typy podpisov"
          content: |
            * Textový podpis
            * Obrazový podpis
            * Digitálne podpisy
            * Podpis QR kódu
            * Podpis čiarového kódu
            * Pečiatka Podpis
            * Pole formulára Podpis
      
      ## TAB TWO ##
      tab_two:
        description: |
          Rozhranie Java pre elektronické podpisovanie podporuje [formáty súborov dokumentov] (https://docs.groupdocs.com/signature/java/supported-document-formats/), ako je uvedené nižšie.

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
                * **Metasúbory**: EMF, WMF, CMX
                * **Prenosný**: PDF
                * **Škálovateľná vektorová grafika**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Iní**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java podporuje nasledujúce operačné systémy, rámce a správcov balíkov:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operačné systémy"
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
              title: "Vývojové prostredia"
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
        content: "Vytvárať, čítať, upravovať, skrývať a odstraňovať elektronické podpisy z podporovaných formátov dokumentov"

      # feature loop
      - icon: "fas fa-eye"
        content: "Prístup k podpísanému dokumentu z prúdu, relatívnej cesty alebo absolútnej cesty"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Použite textový podpis na dokumenty, tabuľky, prezentácie, obrázky a súbory PDF"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Pridajte textový podpis ako anotáciu, nálepku, obrázok do súborov PDF a tiež konfigurujte štýl a farbu"

      # feature loop
      - icon: "fas fa-code"
        content: "Podpíšte dokument PDF, obrazový súbor a získajte výstup v inom formáte súboru"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Digitálne podpisujte obrázky s textovým podpisom ako vodoznak a pridajte priehľadnosť, otočenie k elektronickému podpisu"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Vyhľadávajte certifikáty a podpisujte dokumenty Microsoft Word, Excel a PDF pomocou digitálnych certifikátov"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Podpíšte formáty dokumentov na spracovanie textu pomocou natívnych textových vodoznakov"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Použite QR-Code, čiarový kód na podpisovanie Word, Slide, Cell, PDF a obrázkových súborov"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Nakonfigurujte a použite podpisy pečiatok na zabezpečené podporované formáty súborov"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Nastavenie a priradenie obrázkových podpisov k dokumentom, tabuľkám, prezentáciám, obrázkom a súborom PDF"

      # feature loop
      - icon: "fas fa-columns"
        content: "Nakonfigurujte vlastnosti podpisu, napr. vzhľad a dojem, okraje, zarovnanie atď."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Použite digitálny podpis na dokument chránený heslom"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Vykonajte overenie textu dokumentov PDF pomocou nástroja Signature Handler"

      # feature loop
      - icon: "fas fa-print"
        content: "Digitálne overenie dokumentov Word, Cell, PDF pomocou kontajnerov certifikátov .CER a .PFX"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Zadajte rôzne typy merných jednotiek (napr. milimetre, pixely atď.) pre textové podpisy PDF"

      # feature loop
      - icon: "fas fa-lock"
        content: "Získajte informácie o dokumente prostredníctvom súboru alebo adresy URL – pridajte podpisy polí formulára do dokumentov PDF"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Pridajte do QR kódu vlastný dátový objekt, vložený VCard, e-mail, EPC, MeCard alebo objekt udalosti"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Použiť rôzne štýly štetca na podpisy, napr. štetec s prechodom, radiálnym, plným a textúrou"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Podpísať dokument umiestnený na FTP alebo Azure Cloud Storage"

      # feature loop
      - icon: "fas fa-heading"
        content: "Nastavte zarovnanie textu v rámci tvarov pre dokumenty, snímky, obrázky a súbory PDF"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Vyhľadávajte, overujte a digitálne podpisujte prezentačné dokumenty programu PowerPoint"

      # feature loop
      - icon: "fas fa-cube"
        content: "Umiestnite podpis pomocou pixelov v dokumentoch bunky a umiestnenie textu pre podpisy pečiatky"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Implementujte podpis obdĺžnikovej pečiatky so zaoblenými rohmi"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Rozšírte podpisy čiarových kódov a QR kódov o obsah obrazových údajov"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Pridajte šifrované podpisy metadát pri práci s možnosťami podpisovania a vyhľadávania"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Vložte vlastné objekty do metadátových podpisov v rámci Wordu, Excelu a prezentácií"

    more_feature:
      # more_feature_loop
      - title: "Jednoduchá konfigurácia a aplikácia elektronických podpisov"
        content: |
          GroupDocs.Signature for Java API umožňuje konfigurovať a pridávať elektronické podpisy do podporovaných formátov dokumentov. Nasleduje príklad kódu, ktorý ukazuje, aké jednoduché je použiť textový podpis na súbor PDF:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // nastaviť pozíciu podpisu
          options.setLeft(100);
          options.setTop(100);
          
          // nastaviť obdĺžnik podpisu
          options.setWidth(100);
          options.setHeight(30);

          // nastaviť farbu textu a písmo
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // podpísať dokument do spisu
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "Podporované typy kódovania čiarových kódov pre elektronický podpis"
        content: |
          Pomocou GroupDocs.Signature for Java API môžete použiť podpisy čiarových kódov a QR kódov na podporované formáty súborov. GroupDocs.Signature for Java podporuje širokú škálu typov kódovania čiarových kódov, aby vyhovovali väčšine požiadaviek. Medzi podporované typy kódovania čiarových kódov patria, Code 11, Code 128, Code 16K/32, Databar codes, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard a Kód 39 Rozšírený.

          Podobne GroupDocs.Signature for Java API vám umožňuje používať typy QR kódov, ako sú QR, Aztec a Data Matrix. Medzi podporované typy kódovania QR-Code patria Aztec, DataMatrix, GS1 DataMatrix a GS1 QR.

      # more_feature_loop
      - title: "Vyhľadajte podpisy a certifikáty"
        content: |
          Prostredníctvom GroupDocs.Signature for Java API môžete vyhľadávať podpisy QR-Code a čiarových kódov v akomkoľvek dokumente, prezentácii, tabuľke, obrázku, ako aj súbore PDF a získať výsledok vyhľadávania. Môžete tiež vyhľadávať vlastné dátové objekty v dokumentoch podpísaných podpisom QR-Code, ako aj v štandardných VCard a e-mailových objektoch v dokumentoch podpísaných QR-kódom. Podporované je aj overovanie zašifrovaného textu podpisov QR-Code, ako aj vyhľadávanie podpisu metadát v dokumentoch PDF. Použite dodatočné kritériá vyhľadávania pre digitálne podpisy dokumentov Words & Cells.  

          Možnosť vyhľadávania je k dispozícii aj pre podpis metadát pre dokumenty Word, snímky a tabuľky, zatiaľ čo vyhľadávanie v poli formulára je dostupné pre dokumenty PDF.

      # more_feature_loop
      - title: "Nakonfigurujte vlastnosti elektronického podpisu"
        content: |
          Na vylepšenie UX koncových používateľov GroupDocs.Signature for Java API poskytuje množstvo vlastností, ktoré sa dajú veľmi jednoducho nakonfigurovať. Môžete nastaviť možnosti písma a farieb (Farba pozadia, Farba popredia, Tučné, Kurzíva, Podčiarknutie, Rodina písma, Veľkosť písma atď.), Možnosti pozadia a orámovania (Farba pozadia, Priehľadnosť pozadia, Farba orámovania, Štýl pomlčky orámovania, Hrúbka orámovania, Priehľadnosť okrajov atď.), Okraje podpisu (vľavo, Hore, Šírka, Výška, Výplň atď.) a Nastavenie oblasti podpisu a zarovnania podpisu (horizontálne zarovnanie, zvislé zarovnanie atď.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature ponúka rozhrania API na prezeranie dokumentov pre ďalšie populárne vývojové prostredia"

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