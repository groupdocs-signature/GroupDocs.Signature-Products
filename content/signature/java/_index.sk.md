---
############################# Static ############################
layout: "landing"
date: 2024-02-29T14:43:06
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: sk
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
head_title: ".NET, Java, Cloud API a online aplikácie na podpisovanie dokumentov"
head_description: "Získajte komplexné riešenie elektronického podpisu dokumentov pre .NET, Java a cloudové aplikácie. Podpíšte bežné formáty dokumentov online pomocou jednoduchej funkcie drag and drop"

############################# Header ############################
title: "Podpíšte dokumenty<br>cez Java API"
description: "Podpisujte digitálne dokumenty a obrázky na akejkoľvek platforme pomocou našich flexibilných rozhraní API a riešení založených na aplikáciách pre programátorov a koncových používateľov."
words:
  for: "pre"

actions:
  main: "Maven na stiahnutie zadarmo"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licencovanie"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Ste pripravení začať?"
  description: "Vyskúšajte bezplatne funkcie GroupDocs.Signature alebo požiadajte o licenciu"

release:
  title: "Vydaná verzia {0}"
  notes: "Pozrite sa, čo je nové"
  downloads: "K stiahnutiu"

code:
  title: "Podpíšte súbory PDF v jazyku Java"
  more: "Viac príkladov"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Vyberte dokument PDF
    Signature signature = new Signature("sample.pdf");
    
    // Poskytnite text
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Dokument podpíšte a uložte do súboru
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Prehľad GroupDocs.Signature"
  description: "API na vykonávanie podpisovania dokumentov a súvisiacich operácií v aplikáciách Java"
  features:
    # feature loop
    - title: "Vylepšené obchodné dokumenty s digitálnymi podpismi v jazyku Java"
      content: "Rýchle a prispôsobiteľné podpisovanie: GroupDocs.Signature for Java ponúka širokú škálu možností digitálneho podpisu pre súbory PDF, obrázky a dokumenty balíka Office. Môžete použiť text, čiarové kódy, QR kódy, digitálne certifikáty, obrázky alebo skryté metadáta. Spracovanie dokumentov je rýchle a efektívne."

    # feature loop
    - title: "Manipulácia s podpísanými dokumentmi"
      content: "Pokročilé spracovanie dokumentov zahŕňa výkonné operácie s podpísanými dokumentmi pomocou GroupDocs.Signature pre Java. Pomocou rôznych užitočných kritérií môžete vyhľadávať a overovať podpisy, ktoré boli pridané do obchodných dokumentov. Okrem toho môžete získať prístup k podrobným informáciám o dokumente alebo získať ukážky obrázkov jeho strán."

    # feature loop
    - title: "Rôzne možnosti výberu výstupu"
      content: "Rozsiahle možnosti podpisovania vám umožňujú prispôsobiť výstup pre dokumenty podpísané pomocou GroupDocs.Signature for Java. Akýkoľvek podpis môžete presne umiestniť na akúkoľvek stránku dokumentu a rôznymi spôsobmi nakonfigurovať jeho vzhľad. Java API podporuje ukladanie podpísaných obchodných dokumentov v mnohých podporovaných formátoch a poskytuje možnosti na ich zabezpečenie heslom."

############################# Platforms ############################
platforms:
  enable: true
  title: "Nezávislosť na platforme"
  description: "GroupDocs.Signature for Java podporuje nasledujúce operačné systémy, rámce a správcov balíkov"
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
  title: "Podporované formáty súborov"
  description: |
    GroupDocs.Signature for Java podporuje operácie s nasledujúcimi [formátmi súborov](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formáty Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Obrázky a iné formáty
        * **Prenosný:** PDF
        * **snímky:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Iné kancelárske formáty:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Iné formáty
        * **Web:** HTML, MHTML
        * **Archívy:** ZIP, TAR, 7Z
        * **Certifikáty:** PFX

############################# Features ############################
features:
  enable: true
  title: "Funkcie GroupDocs.Signature"
  description: "Podpisovanie PDF, Office dokumentov a obrázkov digitálnymi podpismi"

  items:
    # feature loop
    - icon: "sign"
      title: "Pridávanie podpisov"
      content: "Podpíšte dokument pomocou rôznych podporovaných typov podpisov umiestnením digitálneho podpisu presne na ľubovoľné miesto na ľubovoľnej strane."

    # feature loop
    - icon: "custom"
      title: "Prispôsobenie výsledkov"
      content: "Prispôsobte si vzhľad podpisu úpravou farby, písma, orámovania, otočenia a ďalších funkcií, aby ste dosiahli požadovaný výsledok."

    # feature loop
    - icon: "password"
      title: "Zabezpečenie dokumentov heslom"
      content: "Pri mnohých podporovaných typoch dokumentov môžete podpísaný dokument chrániť heslom."

    # feature loop
    - icon: "protect"
      title: "Zabránenie neoprávneným zmenám"
      content: "Chráňte dôležité obchodné dokumenty podpísané digitálnym certifikátom pred neoprávnenými úpravami."

    # feature loop
    - icon: "convert"
      title: "Získanie výsledkov v požadovaných formátoch"
      content: "Ľahko získajte podpísané súbory výsledkov v akomkoľvek podporovanom formáte. Môžete tiež bez námahy previesť dokumenty MS Word do PDF."

    # feature loop
    - icon: "preview"
      title: "Ukážka dokumentu"
      content: "Uložte ľubovoľnú stranu dokumentu ako obrázok pre budúce spracovanie."

    # feature loop
    - icon: "search"
      title: "Hľadanie podpisov"
      content: "V konkrétnych dokumentoch je možné získať informácie o predtým pridaných podpisoch."

    # feature loop
    - icon: "validate"
      title: "Overovanie dokumentov"
      content: "Overte správnosť podpisov na akomkoľvek podpísanom dokumente."

    # feature loop
    - icon: "update"
      title: "Správa podpisov"
      content: "Po umiestnení podpisu na stranu dokumentu ho možno podľa potreby odstrániť, presunúť alebo aktualizovať."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Vzorky kódu"
  description: "Niektoré prípady použitia typických GroupDocs.Signature pre operácie Java"
  items:
    # code sample loop
    - title: "Vylepšite dokument PDF pomocou QR kódu"
      content: |
        Vylepšenie obchodných procesov pridaním [QR-kódov](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) na konkrétne strany dokumentov PDF môže byť cenné. Existuje príklad, ako pridať QR kód pomocou GroupDocs.Signature pre Java.
        {{< landing/code title="Vylepšite dokument PDF pomocou QR kódu">}}
        ```java {style=abap}
        // Vložte dokument, ktorý chcete podpísať
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Vytvorte možnosti QR kódu s preddefinovaným textom
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Nakonfigurujte typ kódovania QR kódu a pozíciu na stránke
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Podpíšte dokument a uložte ho ako výsledný súbor
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Použite digitálny podpis na ochranu DOCX"
      content: |
        Môžete [Zabezpečiť dokument](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) pomocou osobných alebo firemných podpisov uložených ako digitálne certifikáty. Dokumenty zabezpečené certifikátom nie je možné meniť bez znehodnotenia podpisu.
        {{< landing/code title="Použite digitálny podpis na ochranu DOCX">}}
        ```java {style=abap}   
        // Vložte dokument, ktorý sa má digitálne podpísať
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Zadajte voľby digitálneho podpisovania a zadajte cestu k súboru certifikátu
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Nastavte heslo certifikátu
        options.setPassword("1234567890");

        // Podpíšte dokument a uložte ho na požadovanú cestu
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
