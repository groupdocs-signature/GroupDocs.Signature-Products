---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:02
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
platform: "Net"
platform_tag: "net"

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
title: "Podpíšte dokumenty<br>cez .NET API"
description: "Podpisujte digitálne dokumenty a obrázky na akejkoľvek platforme pomocou našich flexibilných rozhraní API a riešení založených na aplikáciách pre programátorov a koncových používateľov."
words:
  for: "pre"

actions:
  main: "Bezplatné stiahnutie NuGet"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licencovanie"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Ste pripravení začať?"
  description: "Vyskúšajte bezplatne funkcie GroupDocs.Signature alebo požiadajte o licenciu"

release:
  title: "Vydaná verzia {0}"
  notes: "Pozrite sa, čo je nové"
  downloads: "K stiahnutiu"

code:
  title: "Podpíšte súbory PDF v C#"
  more: "Viac príkladov"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Vyberte dokument PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Poskytnite text
        var options = new TextSignOptions("John Smith")
        {
            // Nastaviť farbu
            ForeColor = Color.Red
        };
        // Dokument podpíšte a uložte do súboru
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Prehľad GroupDocs.Signature"
  description: "API na vykonávanie podpisovania dokumentov a súvisiacich operácií v aplikáciách .NET"
  features:
    # feature loop
    - title: "Pridávanie podpisov do obchodných dokumentov v C#"
      content: "Podpisovanie dokumentov: Pomocou GroupDocs.Signature for .NET môžete do dokumentov PDF a balíka Office pridávať rôzne typy podpisov, ako sú text, obrázky, čiarové kódy a digitálne certifikáty. Toto rozhranie API vám umožňuje podpisovať dokumenty takmer akýmkoľvek typom údajov vrátane skrytých metadát."

    # feature loop
    - title: "Spracovanie podpísaných dokumentov"
      content: "Ďalšie spracovanie: Pomocou GroupDocs.Signature môžete vykonávať výkonné operácie s podpísanými dokumentmi. To zahŕňa vyhľadávanie existujúcich podpisov v obchodných dokumentoch a ich overovanie pomocou špecifických kritérií. Okrem toho môžete prostredníctvom tohto rozhrania .NET API získať informácie o dokumente a zobraziť náhľad stránok."

    # feature loop
    - title: "Prispôsobenie výsledkov"
      content: "GroupDocs.Signature for .NET ponúka rozsiahle možnosti prispôsobenia. Podpisy môžete presne umiestniť kdekoľvek na stránke dokumentu a upraviť ich vzhľad pomocou rôznych nastavení. Okrem toho toto API podporuje ukladanie spracovaných dokumentov v širokej škále podporovaných formátov."

############################# Platforms ############################
platforms:
  enable: true
  title: "Nezávislosť na platforme"
  description: "GroupDocs.Signature for .NET podporuje nasledujúce operačné systémy, rámce a správcov balíkov"
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
    GroupDocs.Signature for .NET podporuje operácie s nasledujúcimi [formátmi súborov](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Rýchle a presné podpisovanie súborov PDF, dokumentov balíka Office a obrázkov"

  items:
    # feature loop
    - icon: "sign"
      title: "Podpisovanie dokumentov"
      content: "Pridajte jeden alebo viacero podporovaných typov podpisov presne na ľubovoľné miesto v obchodných dokumentoch."

    # feature loop
    - icon: "custom"
      title: "Prispôsobte podpisy"
      content: "Na konfiguráciu vzhľadu podpisov použite funkcie, ako je farba, písmo, orámovanie, otočenie atď."

    # feature loop
    - icon: "password"
      title: "Ochrana dokumentov heslom"
      content: "Zabezpečte určité typy dokumentov nastavením hesla po podpísaní."

    # feature loop
    - icon: "protect"
      title: "Ochrana pred zmenami"
      content: "Zabráňte zmenám dôležitých obchodných dokumentov po pripojení podpisu pomocou digitálneho certifikátu."

    # feature loop
    - icon: "convert"
      title: "Konvertujte podpísané súbory do iných formátov"
      content: "Preveďte podpísané súbory do požadovaných formátov, ako je napríklad uloženie dokumentu programu Word vo formáte PDF."

    # feature loop
    - icon: "preview"
      title: "Extrahujte náhľady stránok"
      content: "Extrahujte strany z podpísaných dokumentov ako jednotlivé obrázky pre budúce spracovanie."

    # feature loop
    - icon: "search"
      title: "Vyhľadávanie podpisov v dokumentoch"
      content: "Získajte informácie o predtým pridaných podpisoch v konkrétnych dokumentoch."

    # feature loop
    - icon: "validate"
      title: "Overte podpísané dokumenty"
      content: "Overte správne podpisovanie dokumentov pomocou overovacích funkcií."

    # feature loop
    - icon: "update"
      title: "Aktualizujte alebo odstráňte podpisy"
      content: "Jednoducho premiestnite konkrétne podpisy na stránku, upravte ich text alebo ich bez problémov odstráňte."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Vzorky kódu"
  description: "Niektoré prípady použitia typických GroupDocs.Signature pre operácie .NET"
  items:
    # code sample loop
    - title: "Pridajte QR kód do PDF"
      content: |
        Pridanie [QR-kódov](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) na konkrétne stránky dokumentov PDF môže zlepšiť obchodné procesy. Nižšie je uvedený príklad, ako pridať QR kód pomocou GroupDocs.Signature.
        {{< landing/code title="Ako vložiť QR kód do PDF.">}}
        ```csharp {style=abap}
        // Vložte dokument, ktorý chcete podpísať
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Vytvorte možnosti QR kódu s preddefinovaným textom
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Nakonfigurujte typ kódovania QR kódu a pozíciu na stránke
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Podpíšte dokument a uložte ho ako výsledný súbor
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ochrana dokumentu DOCX pomocou digitálneho certifikátu"
      content: |
        Môžete [Chrániť dokument](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) pomocou osobných alebo firemných podpisov uložených ako digitálne certifikáty. Takto chránené dokumenty nie je možné upravovať bez toho, aby došlo k znehodnoteniu podpisu.
        {{< landing/code title="Tu je návod, ako zabezpečiť integritu dokumentu.">}}
        ```csharp {style=abap}   
        // Vložte dokument, ktorý sa má digitálne podpísať
        using (Signature signature = new Signature("file_to_sign.docx"))
        {
            // Zadajte voľby digitálneho podpisovania a zadajte cestu k súboru certifikátu
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Nastavte heslo certifikátu
                Password = "1234567890"
            };
            // Podpíšte dokument a uložte ho na požadovanú cestu
            signature.Sign("digitally_signed.docx", options);
        }
        ```
        {{< /landing/code >}}

---
