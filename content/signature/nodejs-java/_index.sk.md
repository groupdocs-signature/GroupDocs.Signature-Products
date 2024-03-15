---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: sk
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
head_title: "Node.js Digital Signature API – GroupDocs.Signature"
head_description: "Integrujte zabezpečené elektronické podpisy do aplikácií Node.js s GroupDocs.Signature. Zjednodušte pracovné postupy podpisovania dokumentov jednoducho a efektívne."

############################# Header ############################
title: "Podpíšte dokumenty<br>s Node.js API"
description: "Podpisujte digitálne dokumenty a obrázky na akejkoľvek platforme pomocou našich flexibilných rozhraní API a riešení založených na aplikáciách pre programátorov a koncových používateľov."
words:
  for: "pre"

actions:
  main: "Stiahnite si z NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licencovanie"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Ste pripravení začať?"
  description: "Vyskúšajte bezplatne funkcie GroupDocs.Signature alebo požiadajte o licenciu"

release:
  title: "Vydaná verzia {0}"
  notes: "Pozrite sa, čo je nové"
  downloads: "K stiahnutiu"

code:
  title: "Podpisovanie súborov PDF pomocou Node.js"
  more: "Viac príkladov"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Vyberte dokument PDF
    let signature = new Signature("sample.pdf");
    
    // Poskytnite text
    let options = new TextSignOptions("John Smith");
    
    // Nastaviť farbu
    options.ForeColor = Color.Red;
    
    // Dokument podpíšte a uložte do súboru
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Prehľad GroupDocs.Signature"
  description: "Knižnica na podpisovanie dokumentov, ktorá je pripravená na použitie v aplikáciách Node.js"
  features:
    # feature loop
    - title: "Riešenie digitálnych podpisov pre obchodné dokumenty s Node.js"
      content: "GroupDocs.Signature for Node.js via Java ponúka komplexnú sadu možností digitálneho podpisu pre PDF, dokumenty a obrázky balíka Office. K dispozícii sú texty, čiarové kódy, obrázky, digitálne certifikáty a metadáta. Efektívnosť zaisťuje efektívne spracovanie dokumentov."

    # feature loop
    - title: "Pokročilá manipulácia s podpísanými dokumentmi"
      content: "GroupDocs.Signature vám umožňuje spracovávať podpísané dokumenty. Vyhľadávajte a overujte podpisy pomocou rôznych kritérií. Okrem toho extrahujte podrobné informácie o dokumente alebo generujte ukážkové obrázky strán."

    # feature loop
    - title: "Rôzne výstupné formáty"
      content: "Naše riešenie poskytuje rozsiahlu kontrolu nad výstupným formátom podpísaných dokumentov. Presne umiestnite podpisy na ľubovoľnú stránku a prispôsobte si ich vzhľad. Uložte podpísané dokumenty v mnohých podporovaných formátoch a voliteľne ich zabezpečte heslom."

############################# Platforms ############################
platforms:
  enable: true
  title: "Nezávislosť na platforme"
  description: "GroupDocs.Signature for Node.js via Java vykonáva spracovanie dokumentov s rôznymi operačnými systémami"
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
  title: "Podporované formáty súborov"
  description: |
    GroupDocs.Signature for Node.js via Java uľahčuje operácie s [populárnymi formátmi súborov](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Funkcie služby GroupDocs.Signature"
  description: "Podpisujte súbory PDF, dokumenty balíka Office a obrázky digitálnymi podpismi"

  items:
    # feature loop
    - icon: "sign"
      title: "Obchodné podpisy"
      content: "Na podpisovanie dokumentov používajte rôzne typy podpisov. Umiestnite digitálne podpisy presne na akékoľvek umiestnenie stránky."

    # feature loop
    - icon: "custom"
      title: "Prispôsobenie vzhľadu podpisu"
      content: "Prispôsobte vizuálne aspekty podpisov úpravou farby, písma, okrajov, rotácie a ďalších, aby ste dosiahli požadovaný výsledok."

    # feature loop
    - icon: "password"
      title: "Dokumenty chránené heslom"
      content: "V prípade mnohých podporovaných formátov dokumentov zabezpečte podpísané dokumenty heslom, aby ste zvýšili bezpečnosť."

    # feature loop
    - icon: "protect"
      title: "Zabránenie neoprávneným úpravám"
      content: "Chráňte dôležité obchodné dokumenty podpísané digitálnymi certifikátmi pred neoprávnenými zmenami."

    # feature loop
    - icon: "convert"
      title: "Požadované výstupné formáty"
      content: "Bez námahy získajte podpísané dokumenty v akomkoľvek podporovanom formáte. Jednoducho konvertujte dokumenty MS Word do formátu PDF."

    # feature loop
    - icon: "preview"
      title: "Ukážka dokumentov"
      content: "Uložte jednotlivé strany dokumentu ako obrázky pre budúce potreby."

    # feature loop
    - icon: "search"
      title: "Vyhľadávanie podpisov"
      content: "Získajte informácie o predtým pridaných podpisoch vo svojich dokumentoch."

    # feature loop
    - icon: "validate"
      title: "Overenie dokumentu"
      content: "Overte si pravosť podpisov uvedených v akomkoľvek dokumente."

    # feature loop
    - icon: "update"
      title: "Správa podpisov"
      content: "Odstráňte, premiestnite alebo upravte všetky podpisy umiestnené na ľubovoľnej strane dokumentu."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Vzorky kódu"
  description: "Ilustratívne príklady znázorňujúce typické operácie GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Označte PDF pomocou QR kódov"
      content: |
        Začlenenie [čiarových kódov](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) do konkrétnych stránok dokumentu PDF môže zefektívniť obchodné procesy. Táto časť poskytuje príklad pridania QR kódu pomocou GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Ako vložiť QR kód do PDF.">}}
        ```javascript {style=abap}
        // Vložte dokument, ktorý chcete podpísať
        let signature = new Signature("file_to_sign.pdf");
        
        // Vytvorte možnosti QR kódu s preddefinovaným textom
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Nakonfigurujte typ kódovania QR kódu a pozíciu na stránke
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Podpíšte dokument a uložte ho ako výsledný súbor
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ochrana DOCX digitálnym podpisom"
      content: |
        [Chráňte svoje dokumenty](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) pomocou podpisov založených na digitálnych certifikátoch. Digitálny podpis chráni vaše obchodné dokumenty pred zmenou obsahu.
        {{< landing/code title="Tu je návod, ako zabezpečiť integritu dokumentu.">}}
        ```javascript {style=abap}   
        // Vložte dokument, ktorý sa má digitálne podpísať
        let signature = new Signature("file_to_sign.docx");
        
        // Zadajte voľby digitálneho podpisovania a zadajte cestu k súboru certifikátu
        let options = new DigitalSignOptions("certificate.pfx");

        // Nastavte heslo certifikátu
        options.Password = "1234567890";

        // Podpíšte dokument a uložte ho na požadovanú cestu
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
