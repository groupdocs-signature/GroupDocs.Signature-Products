---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: cs
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
head_title: "Node.js Digital Signature API - GroupDocs.Signature"
head_description: "Integrujte zabezpečené elektronické podpisy v aplikacích Node.js s GroupDocs.Signature. Zjednodušte pracovní postupy podepisování dokumentů snadno a efektivně."

############################# Header ############################
title: "Podepisujte dokumenty<br>s Node.js API"
description: "Podepisujte digitální dokumenty a obrázky na jakékoli platformě pomocí našich flexibilních rozhraní API a řešení založených na aplikacích pro programátory a koncové uživatele."
words:
  for: "pro"

actions:
  main: "Stáhnout z NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licencování"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Jste připraveni začít?"
  description: "Vyzkoušejte funkce GroupDocs.Signature zdarma nebo si vyžádejte licenci"

release:
  title: "Vydána verze {0}"
  notes: "Podívejte se, co je nového"
  downloads: "Stahování"

code:
  title: "Podepisování souborů PDF pomocí Node.js"
  more: "Další příklady"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Vyberte dokument PDF
    let signature = new Signature("sample.pdf");
    
    // Poskytněte text
    let options = new TextSignOptions("John Smith");
    
    // Nastavit barvu
    options.ForeColor = Color.Red;
    
    // Podepište dokument a uložte do souboru
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Přehled GroupDocs.Signature"
  description: "Knihovna pro podepisování dokumentů připravená k použití v aplikacích Node.js"
  features:
    # feature loop
    - title: "Řešení digitálních podpisů pro obchodní dokumenty s Node.js"
      content: "GroupDocs.Signature for Node.js via Java nabízí komplexní sadu možností digitálního podpisu pro PDF, dokumenty Office a obrázky. K dispozici jsou texty, čárové kódy, obrázky, digitální certifikáty a metadata. Zjednodušené zpracování dokumentů zajišťuje efektivitu."

    # feature loop
    - title: "Pokročilá manipulace s podepsanými dokumenty"
      content: "GroupDocs.Signature vám umožňuje zpracovávat podepsané dokumenty. Vyhledávejte a ověřujte podpisy pomocí různých kritérií. Navíc extrahujte podrobné informace o dokumentu nebo generujte náhledové obrázky stránek."

    # feature loop
    - title: "Různé výstupní formáty"
      content: "Naše řešení poskytuje rozsáhlou kontrolu nad výstupním formátem podepsaných dokumentů. Přesně umístěte podpisy na jakoukoli stránku a přizpůsobte jejich vzhled. Ukládejte podepsané dokumenty v mnoha podporovaných formátech a volitelně je zabezpečte hesly."

############################# Platforms ############################
platforms:
  enable: true
  title: "Nezávislost na platformě"
  description: "GroupDocs.Signature for Node.js via Java provádí zpracování dokumentů s různými operačními systémy"
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
  title: "Podporované formáty souborů"
  description: |
    GroupDocs.Signature for Node.js via Java usnadňuje operace s [oblíbenými formáty souborů](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  description: "Podepisujte soubory PDF, dokumenty Office a obrázky digitálními podpisy"

  items:
    # feature loop
    - icon: "sign"
      title: "Obchodní podpisy"
      content: "K podepisování dokumentů používejte různé typy podpisů. Umístěte digitální podpisy přesně na jakékoli umístění stránky."

    # feature loop
    - icon: "custom"
      title: "Přizpůsobení vzhledu podpisu"
      content: "Přizpůsobte vizuální aspekty podpisů úpravou barvy, písma, ohraničení, rotace a dalších, abyste dosáhli požadovaného výsledku."

    # feature loop
    - icon: "password"
      title: "Dokumenty chráněné heslem"
      content: "U mnoha podporovaných formátů dokumentů chraňte podepsané dokumenty heslem pro větší zabezpečení."

    # feature loop
    - icon: "protect"
      title: "Prevence neoprávněných úprav"
      content: "Chraňte důležité obchodní dokumenty podepsané digitálními certifikáty před neoprávněnými změnami."

    # feature loop
    - icon: "convert"
      title: "Požadované výstupní formáty"
      content: "Bez námahy získejte podepsané dokumenty v jakémkoli podporovaném formátu. Snadno převádějte dokumenty MS Word do formátu PDF."

    # feature loop
    - icon: "preview"
      title: "Náhled dokumentů"
      content: "Uložte jednotlivé stránky dokumentu jako obrázky pro budoucí potřeby."

    # feature loop
    - icon: "search"
      title: "Vyhledávání podpisů"
      content: "Získejte informace o dříve přidaných podpisech ve svých dokumentech."

    # feature loop
    - icon: "validate"
      title: "Ověření dokumentu"
      content: "Ověřte pravost podpisů uvedených v jakémkoli dokumentu."

    # feature loop
    - icon: "update"
      title: "Správa podpisů"
      content: "Odstraňte, přemístěte nebo upravte jakékoli podpisy umístěné na jakékoli stránce dokumentu."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ukázky kódu"
  description: "Ilustrativní příklady ukazující typické operace GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Označte PDF pomocí QR kódů"
      content: |
        Začlenění [čárových kódů](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) do konkrétních stránek dokumentu PDF může zefektivnit obchodní procesy. Tato část poskytuje příklad přidání QR kódu pomocí GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Jak vložit QR kód do PDF.">}}
        ```javascript {style=abap}
        // Vložte dokument k podpisu
        let signature = new Signature("file_to_sign.pdf");
        
        // Vytvořte možnosti QR kódu s předdefinovaným textem
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Nakonfigurujte typ kódování QR kódu a pozici na stránce
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Podepište dokument a uložte jej jako výsledný soubor
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ochrana DOCX pomocí digitálního podpisu"
      content: |
        [Chraňte své dokumenty](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) pomocí podpisů založených na digitálních certifikátech. Digitální podpis chrání vaše obchodní dokumenty před změnou obsahu.
        {{< landing/code title="Zde je návod, jak zajistit integritu dokumentu.">}}
        ```javascript {style=abap}   
        // Vložte dokument, který má být digitálně podepsán
        let signature = new Signature("file_to_sign.docx");
        
        // Zadejte možnosti digitálního podepisování a zadejte cestu k souboru certifikátu
        let options = new DigitalSignOptions("certificate.pfx");

        // Nastavte heslo certifikátu
        options.Password = "1234567890";

        // Podepište dokument a uložte jej na požadovanou cestu
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
