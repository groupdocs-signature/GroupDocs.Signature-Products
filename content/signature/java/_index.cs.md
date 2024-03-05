---
############################# Static ############################
layout: "landing"
date: 2024-03-05T15:50:57
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: cs
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
head_title: ".NET, Java, Cloud API a online aplikace pro podpis dokumentů"
head_description: "Získejte komplexní řešení elektronického podpisu dokumentů pro .NET, Java a cloudové aplikace. Podepisujte běžné formáty dokumentů online pomocí jednoduché funkce drag and drop"

############################# Header ############################
title: "Podepisujte dokumenty<br>přes Java API"
description: "Podepisujte digitální dokumenty a obrázky na jakékoli platformě pomocí našich flexibilních rozhraní API a řešení založených na aplikacích pro programátory a koncové uživatele."
words:
  for: "pro"

actions:
  main: "Maven ke stažení zdarma"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licencování"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Jste připraveni začít?"
  description: "Vyzkoušejte funkce GroupDocs.Signature zdarma nebo si vyžádejte licenci"

release:
  title: "Vydána verze {0}"
  notes: "Podívejte se, co je nového"
  downloads: "Stahování"

code:
  title: "Podepisujte soubory PDF v Javě"
  more: "Další příklady"
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
    
    // Poskytněte text
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Podepište dokument a uložte do souboru
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Přehled GroupDocs.Signature"
  description: "API pro provádění podepisování dokumentů a souvisejících operací v aplikacích Java"
  features:
    # feature loop
    - title: "Vylepšené obchodní dokumenty s digitálními podpisy v Javě"
      content: "Rychlé a přizpůsobitelné podepisování: GroupDocs.Signature pro Java nabízí širokou škálu možností digitálního podpisu pro soubory PDF, obrázky a dokumenty Office. Můžete použít text, čárové kódy, QR kódy, digitální certifikáty, obrázky nebo skrytá metadata. Zpracování dokumentů je rychlé a efektivní."

    # feature loop
    - title: "Manipulace s podepsanými dokumenty"
      content: "Pokročilé zpracování dokumentů zahrnuje výkonné operace s podepsanými dokumenty pomocí GroupDocs.Signature for Java. Pomocí různých užitečných kritérií můžete vyhledávat a ověřovat podpisy, které byly přidány do obchodních dokumentů. Kromě toho můžete získat přístup k podrobným informacím o dokumentu nebo získat náhledy jeho stránek."

    # feature loop
    - title: "Různé možnosti výstupu"
      content: "Robustní možnosti podepisování vám umožňují přizpůsobit výstup pro dokumenty podepsané pomocí GroupDocs.Signature for Java. Jakýkoli podpis můžete přesně umístit na jakoukoli stránku dokumentu a různými způsoby nakonfigurovat jeho vzhled. Java API podporuje ukládání podepsaných obchodních dokumentů v mnoha podporovaných formátech a poskytuje možnosti pro jejich zabezpečení hesly."

############################# Platforms ############################
platforms:
  enable: true
  title: "Nezávislost na platformě"
  description: "GroupDocs.Signature for Java podporuje následující operační systémy, rámce a správce balíčků"
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
  title: "Podporované formáty souborů"
  description: |
    GroupDocs.Signature for Java podporuje operace s následujícími [formáty souborů](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
        ### Obrázky a další formáty
        * **Přenosný:** PDF
        * **snímky:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Jiné kancelářské formáty:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Jiné formáty
        * **Web:** HTML, MHTML
        * **Archiv:** ZIP, TAR, 7Z
        * **Certifikáty:** PFX

############################# Features ############################
features:
  enable: true
  title: "Funkce GroupDocs.Signature"
  description: "Podepisování PDF, Office dokumentů a obrázků pomocí digitálních podpisů"

  items:
    # feature loop
    - icon: "sign"
      title: "Přidávání podpisů"
      content: "Podepište dokument pomocí různých podporovaných typů podpisů umístěním digitálního podpisu přesně na libovolné místo na jakékoli stránce."

    # feature loop
    - icon: "custom"
      title: "Přizpůsobení výsledků"
      content: "Přizpůsobte si vzhled podpisu úpravou barvy, písma, ohraničení, otočení a dalších funkcí, abyste dosáhli požadovaného výsledku."

    # feature loop
    - icon: "password"
      title: "Zabezpečení dokumentů heslem"
      content: "U mnoha podporovaných typů dokumentů můžete podepsaný dokument chránit heslem."

    # feature loop
    - icon: "protect"
      title: "Zabránění neoprávněným změnám"
      content: "Chraňte důležité obchodní dokumenty podepsané digitálním certifikátem před neoprávněnými úpravami."

    # feature loop
    - icon: "convert"
      title: "Získání výsledků v požadovaných formátech"
      content: "Snadno získejte podepsané soubory výsledků v jakémkoli podporovaném formátu. Můžete také bez námahy převést dokumenty MS Word do PDF."

    # feature loop
    - icon: "preview"
      title: "Náhled dokumentu"
      content: "Uložte libovolnou stránku dokumentu jako obrázek pro budoucí zpracování."

    # feature loop
    - icon: "search"
      title: "Hledání podpisů"
      content: "Je možné získat informace o dříve přidaných podpisech v konkrétních dokumentech."

    # feature loop
    - icon: "validate"
      title: "Ověřování dokumentů"
      content: "Ověřte správnost podpisů na jakémkoli podepsaném dokumentu."

    # feature loop
    - icon: "update"
      title: "Správa podpisů"
      content: "Jakmile je podpis umístěn na stránku dokumentu, lze jej podle potřeby odstranit, přesunout nebo aktualizovat."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ukázky kódu"
  description: "Některé případy použití typických GroupDocs.Signature pro operace Java"
  items:
    # code sample loop
    - title: "Vylepšete dokument PDF pomocí QR kódu"
      content: |
        Vylepšení obchodních procesů přidáním [QR-kódů](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) na konkrétní stránky dokumentů PDF může být cenné. Existuje příklad, jak přidat QR kód pomocí GroupDocs.Signature pro Java.
        {{< landing/code title="Vylepšete dokument PDF pomocí QR kódu">}}
        ```java {style=abap}
        // Vložte dokument k podpisu
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Vytvořte možnosti QR kódu s předdefinovaným textem
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Nakonfigurujte typ kódování QR kódu a pozici na stránce
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Podepište dokument a uložte jej jako výsledný soubor
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Použijte digitální podpis k ochraně DOCX"
      content: |
        Můžete [Zabezpečit dokument](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) pomocí osobních nebo firemních podpisů uložených jako digitální certifikáty. Dokumenty zabezpečené certifikátem nelze měnit bez znehodnocení podpisu.
        {{< landing/code title="Použijte digitální podpis k ochraně DOCX">}}
        ```java {style=abap}   
        // Vložte dokument, který má být digitálně podepsán
        Signature signature = new Signature("file_to_sign.docx");
        
        // Zadejte možnosti digitálního podepisování a zadejte cestu k souboru certifikátu
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Nastavte heslo certifikátu
        options.setPassword("1234567890");

        // Podepište dokument a uložte jej na požadovanou cestu
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
