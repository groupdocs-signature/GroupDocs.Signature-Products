---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:22
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, Cloud API a online aplikace pro podpis dokumentů"
head_description: "Získejte komplexní řešení elektronického podpisu dokumentů pro .NET, Java a cloudové aplikace. Podepisujte běžné formáty dokumentů online pomocí jednoduché funkce drag and drop"

############################# Header ############################
title: "Podepisujte dokumenty<br>přes .NET API"
description: "Podepisujte digitální dokumenty a obrázky na jakékoli platformě pomocí našich flexibilních rozhraní API a řešení založených na aplikacích pro programátory a koncové uživatele."
words:
  for: "pro"

actions:
  main: "NuGet ke stažení zdarma"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Licencování"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "Jste připraveni začít?"
  description: "Vyzkoušejte funkce GroupDocs.Signature zdarma nebo si vyžádejte licenci"

release:
  title: "Vydána verze {0}"
  notes: "Podívejte se, co je nového"
  downloads: "Stahování"

code:
  title: "Podepisování souborů PDF v C#"
  more: "Další příklady"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // Vyberte dokument PDF
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Poskytněte text
        var options = new TextSignOptions("John Smith")
        {
            // Nastavit barvu
            ForeColor = Color.Red
        };
        // Podepište dokument a uložte do souboru
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Přehled GroupDocs.Signature"
  description: "API pro provádění podepisování dokumentů a souvisejících operací v aplikacích .NET"
  features:
    # feature loop
    - title: "Přidávání podpisů do obchodních dokumentů v C#"
      content: "Podepisování dokumentů: Pomocí GroupDocs.Signature for .NET můžete do dokumentů PDF a Office přidávat různé typy podpisů, jako jsou text, obrázky, čárové kódy a digitální certifikáty. Toto rozhraní API vám umožňuje podepisovat dokumenty téměř jakýmkoli typem dat, včetně skrytých metadat."

    # feature loop
    - title: "Zpracování podepsaných dokumentů"
      content: "Další zpracování: Pomocí GroupDocs.Signature můžete provádět výkonné operace s podepsanými dokumenty. To zahrnuje vyhledávání existujících podpisů v obchodních dokumentech a jejich ověřování pomocí specifických kritérií. Prostřednictvím tohoto rozhraní .NET API můžete navíc načíst informace o dokumentu a zobrazit náhled stránek."

    # feature loop
    - title: "Přizpůsobení výsledků"
      content: "GroupDocs.Signature for .NET nabízí rozsáhlé možnosti přizpůsobení. Podpisy můžete přesně umístit kamkoli na stránku dokumentu a upravit jejich vzhled pomocí různých nastavení. Kromě toho toto API podporuje ukládání zpracovaných dokumentů v široké škále podporovaných formátů."

############################# Platforms ############################
platforms:
  enable: true
  title: "Nezávislost na platformě"
  description: "GroupDocs.Signature for .NET podporuje následující operační systémy, rámce a správce balíčků"
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
    GroupDocs.Signature for .NET podporuje operace s následujícími [formáty souborů](https://docs.groupdocs.com/signature/net/supported-document-formats/).
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
  description: "Rychlé a přesné podepisování PDF, Office dokumentů a obrázků"

  items:
    # feature loop
    - icon: "sign"
      title: "Podepisování dokumentů"
      content: "Přidejte přesně jeden nebo více podporovaných typů podpisů na libovolné zadané místo v obchodních dokumentech."

    # feature loop
    - icon: "custom"
      title: "Přizpůsobte podpisy"
      content: "Ke konfiguraci vzhledu podpisů využijte funkce, jako je barva, písmo, ohraničení, otočení atd."

    # feature loop
    - icon: "password"
      title: "Ochrana dokumentů heslem"
      content: "Zabezpečte určité typy dokumentů nastavením hesla po podpisu."

    # feature loop
    - icon: "protect"
      title: "Ochrana před změnami"
      content: "Zabraňte změnám důležitých obchodních dokumentů po připojení podpisu pomocí digitálního certifikátu."

    # feature loop
    - icon: "convert"
      title: "Převeďte podepsané soubory do jiných formátů"
      content: "Převeďte podepsané soubory do požadovaných formátů, jako je uložení dokumentu aplikace Word jako PDF."

    # feature loop
    - icon: "preview"
      title: "Extrahujte náhledy stránek"
      content: "Extrahujte stránky z podepsaných dokumentů jako jednotlivé obrázky pro budoucí zpracování."

    # feature loop
    - icon: "search"
      title: "Vyhledávání podpisů v dokumentech"
      content: "Získejte informace o dříve přidaných podpisech v konkrétních dokumentech."

    # feature loop
    - icon: "validate"
      title: "Ověřte podepsané dokumenty"
      content: "Ověřte správné podepisování dokumentů pomocí funkcí ověřování."

    # feature loop
    - icon: "update"
      title: "Aktualizujte nebo odstraňte podpisy"
      content: "Snadno přemístěte konkrétní podpisy na stránce, upravte jejich text nebo je bez problémů odstraňte."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Ukázky kódu"
  description: "Některé případy použití typických GroupDocs.Signature pro operace .NET"
  items:
    # code sample loop
    - title: "Přidejte QR kód do PDF"
      content: |
        Přidání [QR-kódů](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) na konkrétní stránky dokumentů PDF může zlepšit obchodní procesy. Níže je uveden příklad, jak přidat QR kód pomocí GroupDocs.Signature.
        {{< landing/code title="Jak vložit QR kód do PDF.">}}
        ```csharp {style=abap}
        // Vložte dokument k podpisu
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Vytvořte možnosti QR kódu s předdefinovaným textem
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // Nakonfigurujte typ kódování QR kódu a pozici na stránce
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Podepište dokument a uložte jej jako výsledný soubor
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ochrana dokumentu DOCX pomocí digitálního certifikátu"
      content: |
        Můžete [Chránit dokument](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/) pomocí osobních nebo firemních podpisů uložených jako digitální certifikáty. Takto chráněné dokumenty nelze upravovat bez znehodnocení podpisu.
        {{< landing/code title="Zde je návod, jak zajistit integritu dokumentu.">}}
        ```csharp {style=abap}   
        // Vložte dokument, který má být digitálně podepsán
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Zadejte možnosti digitálního podepisování a zadejte cestu k souboru certifikátu
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Nastavte heslo certifikátu
                Password = "1234567890"
            };
            // Podepište dokument a uložte jej na požadovanou cestu
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
